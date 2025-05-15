---
Type: Template
Title: Landing Page Template
---

<!DOCTYPE html>
<html lang="en">
<!-- Landing Page Template -->
<!-- Weblog.lol/configuration/landing-page-template.md -->
<head>
<title>{weblog-title}</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="preconnect" href="https://cdnjs.cloudflare.com">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css">
<link rel="stylesheet" href="/style.css">
</head>
<body>

<header>
<h1 class="weblog-title"><a href="/">{weblog-title}</a></h1> <a href="https://social.lol/@luxury_format"><i class="fa-brands fa-mastodon"></i></a> <a href="/feeds"><i class="fa-solid fa-rss"></i></a>
{navigation}
<hr>
</header>
<main>

{body}

<nav>
{previous-page}
{next-page}
</nav>

<span class="divider">&bull; &bull; &bull;</span>

</main>

<footer>
<hr>

<script src="https://status.lol/luxury-format.js?time&link&fluent&pretty"></script>

<hr>

<p>&copy; {year} <a href="/">{weblog-title}</a></p>

<p class="footer-weblog-p">Made with <a href="https://weblog.lol">Weblog.lol</a>.</p>
</footer>

</body>
</html>
