---
Type: Template
Title: Landing Page template
---

<!DOCTYPE html>
<html lang="en">
  <!-- Landing Page template -->
  <!-- weblog/templates/landing-page-template.md -->
  <!-- HEAD -->
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>{weblog-title}{separator}Blog</title>
    <meta property="og:title" content="{weblog-title}">
    <meta name="description" content="{weblog-description}">
    <meta property="og:description" content="{weblog-description}">
    <meta property="og:type" content="article">
    <meta property="og:url" content="{permalink}">
    <meta property="og:image" content="https://profiles.cache.lol/luxury-format/picture.png">
    <!-- FEDIVERSE CREATOR -->
    <meta name="fediverse:creator" content="@luxury_format@social.lol">
    <a style="display: none;" rel="me" href="https://social.lol/@luxury_format">Mastodon</a>
    <!-- AUTHOR -->
    <meta name="author" content="{author}">
    <!-- FEEDS -->
    <link rel="alternate" type="application/atom+xml" title="{weblog-title} Atom Feed" href="https://luxury-format.weblog.lol/atom.xml">
    <link rel="alternate" type="application/rss+xml" title="{weblog-title} RSS Feed" href="https://luxury-format.weblog.lol/rss.xml">
    <link rel="alternate" type="application/json" title="{weblog-title} JSON Feed" href="https://luxury-format.weblog.lol/feed.json">
    <!-- BLOGROLL -->
    <!-- <link rel="blogroll" type="text/xml" href="/blogroll/opml.xml" title="{weblog-title} blogroll"> -->
    <!-- ICONS -->
    <!-- FAVICON.ICO -->
    <link rel='icon' href='https://luxury-format.omg.lol/favicon.ico'>
    <!-- FAVICON.ICO for older browsers/tools -->
    <link rel="shortcut icon" href="https://luxury-format.omg.lol/favicon.ico">
    <!-- iOS Home‑Screen icon -->
    <link rel="apple-touch-icon" href="https://profiles.cache.lol/luxury-format/picture.png">
    <meta name="apple-mobile-web-app-title" content="LF.">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <!-- Safari pinned tab -->
    <!-- A monochrome SVG icon that adapts to Safari’s toolbar theme
    <link rel="mask-icon" href="https://profiles.cache.lol/luxury-format/picture.png" color="#0062FF"> -->
    <!-- Tile color in Windows/Edge
    <meta name="msapplication-TileColor" content="#F2F2F7">
    <meta name="msapplication-TileImage" content="https://profiles.cache.lol/luxury-format/picture.png"> -->
    <link rel="manifest" href="/site.webmanifest">
    <!-- <meta name="msapplication-TileColor" content="#F2F2F7"> -->
    <!-- COLOR SCHEME: LIGHT DARK -->
    <meta name="color-scheme" content="light dark">
    <!-- THEME COLOR -->
    <meta name="theme-color" content="#F2F2F7" media="(prefers-color-scheme: light)">
    <meta name="theme-color" content="#1C1C1E" media="(prefers-color-scheme: dark)">
    <!-- FONTS: Atkinson Hyperlegible and Source Code Pro -->
    <!-- <link rel="preconnect" href="https://fonts.bunny.net" crossorigin="anonymous" referrerpolicy="no-referrer">
    <link rel="stylesheet" href="https://fonts.bunny.net/css?family=atkinson-hyperlegible:400,400i,700,700i|source-code-pro:400,700&display=swap" crossorigin="anonymous" referrerpolicy="no-referrer"> -->
    <!-- Font Awesome Icons -->
    <!-- <link rel="preconnect" href="https://cdnjs.cloudflare.com" crossorigin="anonymous" referrerpolicy="no-referrer">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css" crossorigin="anonymous" referrerpolicy="no-referrer"> -->
    <!-- /style.css -->
    <link rel="stylesheet" href="/style.css">
  </head>
  <!-- BODY -->
  <body>
    <!-- HEADER -->
    <header class="weblog-header">
      <!-- First row: Logo+Title and Social Icons -->
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
          <a href="https://social.lol/@luxury_format" aria-label="Mastodon"><i class="fa-brands fa-mastodon"></i><span>Mastodon</span></a>
          <a href="https://luxury-format.weblog.lol/status" aria-label="Status"><i class="fa-solid fa-face-grin"></i><span>Status</span></a>
          <a href="https://luxury-format.weblog.lol/subscribe" aria-label="Subscribe"><i class="fa-solid fa-rss"></i><span>Subscribe</span></a>
        </div>
      </div>
      <!-- Second row: Navigation Menu -->
      <div class="weblog-navigation">
        {navigation}
      </div>
      <div class="page-navigation">
        <h6><a href="/">Weblog</a> • All posts</h6>
      </div>
    </header>
    <!-- MAIN -->
    <main>
      <h2 class="page-title">Weblog</h2>
      <hr>
      {body}
      <nav class="landing-page-pagination">
        {previous-page}
        {next-page}
      </nav>
    </main>
    <!-- FOOTER -->
    <footer>
      <hr>
      <p>&copy; {year} {weblog-title}</p>
      <p class="footer-weblog-p">Made with <a href="https://home.omg.lol/referred-by/luxury-format">Weblog.lol</a></p>
    </footer>
  </body>
</html>
