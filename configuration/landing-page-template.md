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
    <!-- <link rel="blogroll" type="text/xml" href="/blogroll/opml.xml" title="{blog-title} blogroll"> -->
    <!-- ICONS -->
    <link rel='icon' href='https://{address}.omg.lol/favicon.ico'>
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
    <!-- /style.css -->
    <link rel="stylesheet" href="/css/style.css">
  </head>
  
  <!-- BODY -->
  <body class="body">
    <!-- HEADER -->
    <header class="header">
      <div class="header-top-row">
        <div class="logo-title">
          <a href="/">
            <img src="https://profiles.cache.lol/{address}/picture.png" alt="{blog-title} Logo">
            <h1 class="blog-title">
              <span class="short">{blog-short-title}</span>
              <span class="long">{blog-title}</span>
            </h1>
          </a>
        </div>
        <div class="header-icons">
          <a href="{mastodon-url}"><i class="fa-brands fa-mastodon"></i><span>Mastodon</span></a>
          <a href="{base-path}/status"><i class="fa-solid fa-face-grin"></i><span>Status</span></a>
          <a href="{base-path}/subscribe"><i class="fa-solid fa-rss"></i><span>Subscribe</span></a>
        </div>
      </div>
      <div class="blog-navigation">
        {navigation}
      </div>
    </header>
    <!-- MAIN -->
    <main class="main">
      <span class="divider">&bull; &bull; &bull;</span>
      {body}
      <span class="top-pagination-divider"></span>
      <nav class="pagination">
        {previous-page}
        {next-page}
      </nav>
      <span class="bottom-pagination-divider"></span>
    </main>
    <!-- FOOTER -->
    <footer class="footer">
      <span class="divider">&bull; &bull; &bull;</span>
      <ul class="socials">
        <li>
          <a rel="me" href="https://social.lol/@luxury_format">
            <i class="fa-brands fa-mastodon"></i>
          </a>
        </li>
        <li>
          <a rel="me" href="https://bsky.app/profile/luxury-format.bsky.social">
            <i class="fa-brands fa-bluesky"></i>
          </a>
        </li>
        <li>
          <a rel="me" href="https://discordapp.com/users/434798061370474526">
            <i class="fa-brands fa-discord"></i>
          </a>
        </li>
        <li>
          <a rel="me" href="https://luxury-format.omg.lol">
            <i class="omg-icon omg-prami"></i>
          </a>
        </li>
        <li>
          <a rel="me" href="https://github.com/luxury-format">
            <i class="fa-brands fa-github"></i>
          </a>
        </li>
      </ul>
      <span class="divider">&bull; &bull; &bull;</span>
      <!-- STATUSLOG -->
      <script src="https://status.lol/{address}.js?time&link&fluent&pretty"></script>
      <span class="divider">&bull; &bull; &bull;</span>
      <p>&copy; {year} {blog-title}</p>
      <p class="footer-weblog-p">Made with <a href="https://home.omg.lol/referred-by/{address}"><span class="logotype">Weblog<span class="logotype dot">.</span>lol</span></a></p>
    </footer>
  </body>
</html>
