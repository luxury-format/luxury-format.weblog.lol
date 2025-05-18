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
<!-- Font Awesome Free via CDN -->
<link rel="preconnect" href="https://cdnjs.cloudflare.com">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css" crossorigin="anonymous" referrerpolicy="no-referrer">
<!-- /style.css -->
<link rel="stylesheet" href="/style.css">
<!-- JavaScripts -->
<!-- CODE HIGHLIGHTING -->
<!-- /dracula.css - Dracula Theme v1.2.5 -->
<link rel="stylesheet" href="/dracula.css">
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.4.0/highlight.min.js"></script>
<script>hljs.highlightAll();</script>
</head>
<!-- BODY -->
<body>
<a id="top"></a>

<!-- HEADER -->
<header class="site-header">
<div class="logo-title">
<a href="/">
<img src="https://profiles.cache.lol/luxury-format/picture.png" alt="LUXURY FORMAT Logo">
<h1 class="weblog-title">{weblog-title}</h1>
</a>
</div>
<div class="social-icons">
<a href="https://social.lol/@luxury_format" aria-label="Mastodon"><i class="fa-brands fa-mastodon"></i></a>
<a href="/feeds" aria-label="RSS Feeds"><i class="fa-solid fa-rss"></i></a>
</div>
</header>
<header>
{navigation}
</header>
<hr>
<!-- MAIN NO TITLE LINK -->
<main class="no-title-link">

{body}
<p><a htef="{permalink}">permalink</a></p>
</main>

<!-- FOOTER -->
<footer>
<hr>

<script src="https://status.lol/luxury-format.js?time&link&fluent&pretty"></script>

<hr>

<p>&copy; {year} <a href="/">{weblog-title}</a></p>

<p class="footer-weblog-p">Made with <a href="https://weblog.lol">Weblog.lol</a>.</p>
</footer>

</body>
</html>
