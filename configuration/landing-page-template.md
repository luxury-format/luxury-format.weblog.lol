---
Type: Template
Title: Landing Page Template
---

<!DOCTYPE html>
<html lang="en">
  <!-- Landing Page Template -->
  <!-- Weblog.lol/configuration/landing-page-template.md -->
  <!-- HEAD -->
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>{weblog-title}</title>
    <meta property="og:title" content="{weblog-title}">
    <meta name="description" content="{weblog-description}">
    <meta property="og:description" content="{weblog-description}">
    <meta property="og:type" content="article">
    <meta property="og:url" content="{permalink}">
    <meta property="og:image" content="https://profiles.cache.lol/luxury-format/picture.png">
    <meta name="fediverse:creator" content="@luxury_format@social.lol">
    <!-- FEEDS -->
    <link rel="alternate" type="application/atom+xml" title="{weblog-title} Atom Feed" href="">
    <link rel="alternate" type="application/rss+xml" title="{weblog-title} RSS Feed" href="">
    <link rel="alternate" type="application/json" title="{weblog-title} JSON Feed" href="">
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
    <header>
      <h1 class="weblog-title"><a href="/">{weblog-title}</a></h1>
      <a href="https://social.lol/@luxury_format"><i class="fa-brands fa-mastodon"></i></a>
      <a href="/feeds"><i class="fa-solid fa-rss"></i></a>
      {navigation}
      <hr>
    </header>
    <!-- MAIN -->
    <main>
      
      {body}
      
      <nav>
        {previous-page}
        {next-page}
      </nav>
      
      <span class="divider">&bull; &bull; &bull;</span>
    
    </main>
    
    <!-- FOOTER -->
    <footer>
      <hr>
      <p>&copy; {year} <a href="/">{weblog-title}</a></p>
      <p class="footer-weblog-p">Made with <a href="https://weblog.lol">Weblog.lol</a>.</p>
    </footer>
  
  </body>
</html>
