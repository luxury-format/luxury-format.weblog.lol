---
Type: Template
Title: Landing Page template
---

<!DOCTYPE html>
<html lang="en">
  <!-- Landing Page template -->
  <!-- GitHub file path: 
  configuration/landing-page-template.md -->
  <!-- HEAD -->
  <head>
    <!-- Primary metadata -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>{blog-title}</title>
    <meta name="description" content="{blog-description}">
    <meta name="author" content="{blog-author}">
    <!-- OpenGraph metadata -->
    <meta property="og:title" content="{blog-title}">
    <meta property="og:description" content="{blog-description}">
    <meta property="og:type" content="article">
    <meta property="og:url" content="{base-path}">
    <meta property="og:image" content="https://profiles.cache.lol/{address}/picture.png">
    <!-- Fediverse (Mastodon) -->
    <meta name="fediverse:creator" content="{fediverse-creator}">
    <link rel="me" href="{mastodon-url}">
    <!-- FEEDS -->
    <link rel="alternate" type="application/atom+xml" title="{blog-title} Atom Feed" href="{atom-url}">
    <link rel="alternate" type="application/rss+xml" title="{blog-title} RSS Feed" href="{rss-url}">
    <link rel="alternate" type="application/json" title="{blog-title} JSON Feed" href="{json-url}">
    <!-- BLOGROLL -->
    <!-- <link rel="blogroll" type="text/xml" href="/blogroll/opml.xml" title="{title} blogroll"> -->
    <!-- ICONS -->
    <!-- FAVICON.ICO -->
    <link rel='icon' href='https://{address}.omg.lol/favicon.ico'>
    <!-- FAVICON.ICO for older browsers/tools -->
    <link rel="shortcut icon" href="https://{address}.omg.lol/favicon.ico">
    <!-- APPLE-TOUCH-ICON.PNG -->
    <link rel="apple-touch-icon" href="https://profiles.cache.lol/{address}/picture.png">
    <meta name="apple-mobile-web-app-title" content="{blog-short-title}">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <!-- SITE.WEBMANIFEST -->
    <link rel="manifest" href="/site.webmanifest">
    <!-- COLOR SCHEME -->
    <meta name="color-scheme" content="light dark">
    <!-- THEME COLOR -->
    <meta name="theme-color" content="#FFFFFF" media="(prefers-color-scheme: light)">
    <meta name="theme-color" content="#000000" media="(prefers-color-scheme: dark)">
    <!-- STYLESHEET -->
    <link rel="stylesheet" href="/css/style.css">
  </head>
  <!-- BODY -->
  <body>
    <!-- HEADER -->
    <header class="weblog-header">
      <!-- FIRST ROW: [[LOGO][TITLE] LINK] + [[MASTODON ICON - LINK][STATUS.LOL ICON - LINK][SUBSCRIBE - ICON LINK]] -->
      <div class="header-top-row">
        <div class="logo-title">
          <a href="/">
            <img src="https://profiles.cache.lol/{address}/picture.png" alt="{title} Logo">
            <h1 class="weblog-title">
              <span class="short">{blog-short-title}</span>
              <span class="long">{blog-title}</span>
            </h1>
          </a>
        </div>
        <div class="header-icons">
          <a href="{mastodon-url}"><i class="fa-brands fa-mastodon"></i><span>Mastodon</span></a>
          <a href="https://{base-path}/status"><i class="fa-solid fa-face-grin"></i><span>Status</span></a>
          <a href="https://{base-path}/subscribe"><i class="fa-solid fa-rss"></i><span>Subscribe</span></a>
        </div>
      </div>
      <!-- Second row: Navigation Menu -->
      <div class="weblog-navigation">
        {navigation}
      </div>
    </header>
    <!-- MAIN -->
    <main>
      <span class="divider">&bull; &bull; &bull;</span>
      {body}
      <nav class="landing-page-pagination">
        {previous-page}
        {next-page}
      </nav>
    </main>
    
    <!-- FOOTER -->
    <footer>
      <hr>
      <!-- STATUSLOG -->
      <script src="https://status.lol/{address}.js?time&link&fluent&pretty"></script>
      <hr>
      <p>&copy; {year} {blog-title}</p>
      <p class="footer-weblog-p">Made with <a href="https://home.omg.lol/referred-by/{address}"><span class="logotype">Weblog<span class="logotype dot">.</span>lol</span></a></p>
    </footer>
  </body>
</html>
