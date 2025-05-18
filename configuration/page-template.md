---
Type: Template
Title: Page Template
---

<!DOCTYPE html>
<html lang="en">
  <!-- Page Template -->
  <!-- Weblog.lol/configuration/landing-page-template.md -->
  <!-- HEAD -->
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>{weblog-title}{separator}{post-title}</title>
    <meta property="og:title" content="{weblog-title}{separator}{post-title}">
    <meta name="description" content="{weblog-description}">
    <meta property="og:description" content="{weblog-description}">
    <meta property="og:type" content="article">
    <meta property="og:url" content="{permalink}">
    <!-- <meta property="og:url" content="{location}"> -->
    <meta property="og:image" content="https://profiles.cache.lol/luxury-format/picture.png">
    <!-- FEDIVERSE CREATOR -->
    <meta name="fediverse:creator" content="@luxury_format@social.lol">
    <!-- FEEDS -->
    <link rel="alternate" type="application/atom+xml" title="{weblog-title} Atom Feed" href="https://luxury-format.weblog.lol/atom.xml">
    <link rel="alternate" type="application/rss+xml" title="{weblog-title} RSS Feed" href="https://luxury-format.weblog.lol/rss.xml">
    <link rel="alternate" type="application/json" title="{weblog-title} JSON Feed" href="https://luxury-format.weblog.lol/feed.json">
    <!-- BLOGROLL -->
    <!-- <link rel="blogroll" type="text/xml" href="/blogroll/opml.xml" title="{weblog-title} blogroll"> -->
    <!-- ICONS -->
    <link rel="apple-touch-icon" sizes="180x180" href="https://profiles.cache.lol/luxury-format/picture.png">
    <link rel="icon" type="image/png" sizes="32x32" href="https://profiles.cache.lol/luxury-format/picture.png">
    <link rel="icon" type="image/png" sizes="16x16" href="https://profiles.cache.lol/luxury-format/picture.png">
    <!-- <link rel="manifest" href="/site.webmanifest">
    <link rel="mask-icon" href="/assets/icons/safari-pinned-tab.svg" color="#0080FF">
    <meta name="msapplication-TileColor" content="#0080FF"> -->
    <!-- THEME COLOR -->
    <meta name="theme-color" content="#0080FF">
    <!-- FAVICON.ICO -->
    <link rel='icon' type='image/x-icon' href='https://luxury-format.omg.lol/favicon.ico'>
    <!-- Font Awesome Icons -->
    <link rel="preconnect" href="https://cdnjs.cloudflare.com">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css" crossorigin="anonymous" referrerpolicy="no-referrer">
    <!-- /style.css -->
    <link rel="stylesheet" href="/style.css">
    <!-- Highlight Code Blocks - Dracula Theme v1.2.5 -->
    <link rel="stylesheet" href="/dracula.css">
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
            <h1 class="weblog-title">{weblog-title}</h1>
          </a>
        </div>
        <div class="header-icons">
          <a href="https://social.lol/@luxury_format" aria-label="Mastodon"><i class="fa-brands fa-mastodon"></i></a>
          <a href="/feeds" aria-label="RSS Feeds"><i class="fa-solid fa-rss"></i></a>
        </div>
        <!-- Second row: Navigation Menu -->
        <div class="weblog-navigation">
          {navigation}
        </div>
    </header>
    <hr>
    <!-- MAIN NO TITLE LINK -->
    <main class="no-title-link">
      {body}
    </main>
    <!-- FOOTER -->
    <footer>
      <hr>
      <p>&copy; {year} <a href="/">{weblog-title}</a></p>
      <p class="footer-weblog-p">Made with <a href="https://weblog.lol">Weblog.lol</a>.</p>
    </footer>
  </body>
</html>
