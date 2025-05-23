Date: 2025-05-01 00:00
Type: Page
Title: All pages
Location: /all-pages
---

# All pages

---

<div id="pages-list"></div>

<script>
(function() {
    'use strict';
    
    // Configuration
    const CONFIG = {
        username: 'luxury-format',
        containerSelector: '#pages-list',
        listClass: 'all-pages'
    };
    
    function parseFrontMatter(content) {
        const frontMatterRegex = /^\s*---\s*\n([\s\S]*?)\n\s*---/;
        const match = content.match(frontMatterRegex);
        
        if (!match) return null;
        
        const frontMatter = {};
        const lines = match[1].split('\n');
        
        for (const line of lines) {
            const colonIndex = line.indexOf(':');
            if (colonIndex > -1) {
                const key = line.substring(0, colonIndex).trim();
                const value = line.substring(colonIndex + 1).trim();
                frontMatter[key] = value;
            }
        }
        
        return frontMatter;
    }
    
    async function fetchPageData(url) {
        try {
            const response = await fetch(url);
            if (!response.ok) throw new Error(`HTTP ${response.status}`);
            
            const content = await response.text();
            return parseFrontMatter(content);
        } catch (error) {
            console.warn(`Failed to fetch ${url}:`, error);
            return null;
        }
    }
    
    async function getAllPages() {
        try {
            const response = await fetch(`https://${CONFIG.username}.weblog.lol/`);
            if (!response.ok) throw new Error(`HTTP ${response.status}`);
            
            const html = await response.text();
            const parser = new DOMParser();
            const doc = parser.parseFromString(html, 'text/html');
            
            const links = Array.from(doc.querySelectorAll('a[href]'))
                .map(link => link.getAttribute('href'))
                .filter(href => href && href.startsWith('/') && !href.startsWith('//'))
                .filter(href => !href.includes('#') && href !== '/')
                .map(href => href.replace(/\/$/, ''));
            
            return [...new Set(links)];
        } catch (error) {
            console.error('Failed to get pages list:', error);
            return [];
        }
    }
    
    async function getCommonPages() {
        const commonPaths = [
            '/about', '/contact', '/projects', '/work', '/services',
            '/portfolio', '/resume', '/cv', '/bio', '/links',
            '/now', '/uses', '/colophon', '/privacy', '/terms'
        ];
        
        const existingPages = [];
        
        for (const path of commonPaths) {
            try {
                const response = await fetch(`https://${CONFIG.username}.weblog.lol${path}`);
                if (response.ok) {
                    existingPages.push(path);
                }
            } catch (error) {
            }
        }
        
        return existingPages;
    }
    
    async function generatePagesList() {
        const container = document.querySelector(CONFIG.containerSelector);
        if (!container) {
            console.error(`Container not found: ${CONFIG.containerSelector}`);
            return;
        }
        
        container.innerHTML = '<p>Loading pages...</p>';
        
        try {
            let pagePaths = await getAllPages();
            if (pagePaths.length === 0) {
                console.log('Falling back to common page detection...');
                pagePaths = await getCommonPages();
            }
            
            if (pagePaths.length === 0) {
                container.innerHTML = '<p>No pages found.</p>';
                return;
            }
            
            const pages = [];
            const fetchPromises = pagePaths.map(async (path) => {
                const url = `https://${CONFIG.username}.weblog.lol${path}`;
                const frontMatter = await fetchPageData(url);
                
                if (frontMatter && frontMatter.Type === 'Page' && frontMatter.Title) {
                    pages.push({
                        title: frontMatter.Title,
                        location: frontMatter.Location || path,
                        url: path
                    });
                }
            });
            
            await Promise.all(fetchPromises);
            
            if (pages.length === 0) {
                container.innerHTML = '<p>No pages with Type: Page found.</p>';
                return;
            }
            
            pages.sort((a, b) => a.title.localeCompare(b.title));
            
            const listItems = pages.map(page => 
                `<li><a href="${page.location}">${page.title}</a></li>`
            ).join('\n  ');
            
            const html = `<ul class="${CONFIG.listClass}">
  ${listItems}
</ul>`;
            
            container.innerHTML = html;
            
        } catch (error) {
            console.error('Error generating pages list:', error);
            container.innerHTML = '<p>Error loading pages. Please try again later.</p>';
        }
    }
    
    function init() {
        if (document.readyState === 'loading') {
            document.addEventListener('DOMContentLoaded', generatePagesList);
        } else {
            generatePagesList();
        }
    }
    
    window.WeblogPagesList = {
        generate: generatePagesList,
        config: CONFIG
    };
    
    init();
    
})();
</script>
