---
Type: Template
Title: Landing Page template
---

<!DOCTYPE html>
<html lang="en">
  <!-- Landing Page Template -->
  <!-- GitHub file path: 
  configuration/landing-page-template.md -->
  <!-- HEAD -->
  <head>
    <!-- METADATA -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>{weblog-title}</title>
    <meta name="description" content="{weblog-description}">
    <meta name="author" content="{author}">
    <!-- OpenGraph METADATA -->
    <meta property="og:title" content="{weblog-title}">
    <meta property="og:description" content="{weblog-description}">
    <meta property="og:type" content="article">
    <meta property="og:url" content="{permalink}">
    <meta property="og:image" content="https://profiles.cache.lol/luxury-format/picture.png">
    <!-- FEDIVERSE (Mastodon) -->
    <meta name="fediverse:creator" content="@luxury_format@social.lol">
    <link rel="me" href="https://social.lol/@luxury_format">
    <!-- FEEDS -->
    <link rel="alternate" type="application/atom+xml" title="{weblog-title} Atom Feed" href="{atom-url}">
    <link rel="alternate" type="application/rss+xml" title="{weblog-title} RSS Feed" href="{rss-url}">
    <link rel="alternate" type="application/json" title="{weblog-title} JSON Feed" href="{json-url}">
    <!-- BLOGROLL -->
    <!-- <link rel="blogroll" type="text/xml" href="/blogroll/opml.xml" title="{weblog-title} blogroll"> -->
    <!-- ICONS -->
    <link rel='icon' href='https://luxury-format.omg.lol/favicon.ico'>
    <!-- APPLE-TOUCH-ICON.PNG -->
    <link rel="apple-touch-icon" href="https://profiles.cache.lol/luxury-format/picture.png">
    <meta name="apple-mobile-web-app-title" content="{weblog-short-title}">
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
            <img src="https://profiles.cache.lol/luxury-format/picture.png" alt="{weblog-title} Logo">
            <h1 class="weblog-title">
              <span class="short">{weblog-short-title}</span>
              <span class="long">{weblog-title}</span>
            </h1>
          </a>
        </div>
        <div class="header-icons">
          <a href="https://social.lol/@luxury_format"><i class="fa-brands fa-mastodon"></i><span>Mastodon</span></a>
          <a href="https://luxury-format.weblog.lol/status"><i class="fa-solid fa-face-grin"></i><span>Status</span></a>
          <a href="https://luxury-format.weblog.lol/subscribe"><i class="fa-solid fa-rss"></i><span>Subscribe</span></a>
        </div>
      </div>
      <div class="weblog-navigation">
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
      <h3>Socials</h3>
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
      <script src="https://status.lol/luxury-format.js?time&link&fluent&pretty"></script>
      <span class="divider">&bull; &bull; &bull;</span>
      <p>&copy; {year} {weblog-title}</p>
      <p class="footer-weblog-p">Made with <a href="https://home.omg.lol/referred-by/luxury-format"><span class="logotype">Weblog<span class="logotype dot">.</span>lol</span></a></p>
    </footer>
  </body>
</html>
