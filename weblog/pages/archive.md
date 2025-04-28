---
Type: Page
---

<!DOCTYPE html>
<html lang="en">
<head>
<title>{weblog-title}{separator}{post-title}</title>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#bd93f9" />
{feeds}
<style>
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/font-lato-regular.css');
@import url('https://static.omg.lol/type/font-lato-bold.css');
@import url('https://static.omg.lol/type/font-lato-italic.css');
@import url('https://static.omg.lol/type/font-md-io.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://cdn.cache.lol/profiles/icons/omg.lol-icons.css');
</style>
<!-- <link rel="apple-touch-icon" sizes="76x76" href="https://luxury-format.weblog.lol/favicons/apple-touch-icon.png" />
<link rel="icon" type="image/png" sizes="32x32" href="https://luxury-format.weblog.lol/favicons/favicon-32x32.png" />
<link rel="icon" type="image/png" sizes="16x16" href="https://luxury-format.weblog.lol/favicons/favicon-16x16.png" />
<meta property="og:image" content="https://luxury-format.weblog.lol/images/assets/social-card.png">
<link rel="webmention" href="https://webmention.io/luxury-format.weblog.lol/webmention" />
<link rel="pingback" href="https://webmention.io/luxury-format.weblog.lol/xmlrpc" /> -->
</head>
<body>

<header>
    <h1 class="weblog-title">
        <a href="/">
            <img src="https://profiles.cache.lol/luxory-format/picture" alt="{weblog-title}" />
            <span>{weblog-title}</span>
        </a>
    </h1>
    {navigation}
</header>

<main>
    <div id="status-container" class="container background-cyan">
        <script src="https://status.lol/luxory-format.js?link"></script>
    </div>
    <article>
        <h1><i class="fa-solid fa-archive"></i> {post-title}</h1>
        {post-list}
    </article>
    <hr />
    <div class="weblog-info">
        <div class="container background-orange">
            <h2><i class="fa-solid fa-clock"></i> Recent posts</h2>
            {recent-posts}
        </div>
        <div class="container background-pink">
            <h2><i class="fa-solid fa-fw fa-magnifying-glass"></i> Search</h2>
            <form class="weblog-search" action="?" method="get">
                <input placeholder="What are you looking for?" type="text" name="search">
                <div class="weblog-search--submit-wrap">
                    <button type="submit">Let's take a look!</button>
                </div>
            </form>
        </div>
    </div>
</main>

<footer>
    <p>Made with <a href="https://weblog.lol">weblog.lol</a>.</p>
</footer>

</body>
</html>
