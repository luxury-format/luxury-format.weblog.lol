Type: Template
Title: Page Template
Location: /configuration/page-template.md

<!DOCTYPE html>
<html lang="en">
<!-- Page Template from GitHub repo -->
<head>
<title>{weblog-title}{separator}{post-title}</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta property="og:title" content="{weblog-title}">
<meta name="description" content="{weblog-description}">
<meta property="og:description" content="{weblog-description}">
<meta property="og:type" content="article">
<meta property="og:url" content="https://luxury-format.weblog.lol">
<a style="display: none;" rel="me" href="https://social.lol/@luxury_format">Mastodon</a>
<a style="display: none;" href="https://github.com/LUXURYFORMAT" rel="me">github.com/LUXURYFORMAT</a>
<a style="display: none;" href="https://proven.lol/f6c7ca">proven.lol/f6c7ca</a>
<meta name="fediverse:creator" content="@luxury_format@social.lol">
<link rel="alternate" type="application/atom+xml" title="LUXURY FORMAT Atom Feed" href="https://luxury-format.weblog.lol/atom.xml">
<link rel="alternate" type="application/rss+xml" title="LUXURY FORMAT RSS Feed" href="https://luxury-format.weblog.lol/rss.xml">
<link rel="alternate" type="application/json" title="LUXURY FORMAT JSON Feed" href="https://luxury-format.weblog.lol/feed.json">
<link rel="preconnect" href="https://fonts.bunny.net">
<link href="https://fonts.bunny.net/css?family=atkinson-hyperlegible:400,400i,700,700i|source-code-pro:200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i,900,900i" rel="stylesheet" />
<link rel="preconnect" href="https://omgalol.cache.lol" crossorigin>
<link rel="stylesheet" href="https://omgalol.cache.lol/profiles/icons/omg.lol-icons.css">
<link rel="preconnect" href="https://cdnjs.cloudflare.com">
<link rel="preconnect" href="https://kit.fontawesome.com">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css">
<style>
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/font-md-io.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://omgalol.cache.lol/profiles/icons/omg.lol-icons.css');

:root {
  --foreground: #21222C;
  --background: #F8F8F2;
  --link: #0080FF;
  --accent: #C0C0C0;
  --highlight: #E3E3E6;
  --selection: #44475A;
  --blue: #6272A4;
  --red: #FF5555;
  --orange: #FFB86C;
  --yellow: #F1FA8C;
  --green: #50FA7B;
  --purple: #BD93F9;
  --cyan: #8BE9FD;
  --pink: #FF79C6;
  --sans-serif-font: 'Atkinson Hyperlegible', -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  --mono-space-font: 'Source Code Pro', ui-monospace, SFMono-Regular, Monaco, 'Andale Mono', 'Ubuntu Mono', monospace;
  --display-font: 'VC Honey Deck', serif;
  --border-radius: 0.5rem;
  --box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.75);
}

@media (prefers-color-scheme: dark) {
  :root {
    --foreground: #F8F8F2;
    --background: #21222C;
    --link: #7DF9FF;
    --accent: #E5E4E2;
    --highlight: #53565D;
    --blue: #6272A4;
    --selection: #44475A;
    --red: #FF5555;
    --orange: #FFB86C;
    --yellow: #F1FA8C;
    --green: #50FA7B;
    --purple: #BD93F9;
    --cyan: #8BE9FD;
    --pink: #FF79C6;
    --box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.7);
  }
}

* {
  box-sizing: border-box;
}

body {
  font-family: var(--sans-serif-font);
  font-size: 120%;
  color: var(--foreground);
  background: var(--background);
}

header nav ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

header nav li {
  display: inline-block;
  font-family: var(--sans-serif-font);
}

header nav li a {
  display: block;
  text-decoration: none;
  font-weight: bold;
  margin-right: 1em;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: var(--display-font);
  text-align: center;
  margin: 1rem 0;
}

h1,
h2,
h3,
h4,
h5,
h6,
p {
  overflow-wrap: break-word;
}

}

i[class^="fa-"],
i[class*=" fa-"],
i[class^="omg-"],
i[class*=" omg-"] {
  color: var(--accent);
}

.recent-played {
  background-color: var(--blue);
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
  color: var(--link);
  font-weight: bold;
  padding: 0.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
}

.recent-played-track {
  margin: 0.5rem;
}

.statuslol {
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
}

body.no-title-links main h1.content-title > a.content-link {
  color: inherit;
  text-decoration: none;
  pointer-events: none;
  cursor: default;
}

</style>
</head>
<body class="no-title-links">

<header>
  <h1 class="weblog-title"><a href="/">{weblog-title}</a></h1>
  {navigation}
</header>

<main>

{body}

</main>

<footer>
  <hr>
  <p>&copy; {year} <a href="/">{weblog-title}</a></p>
  <p>Made with <a href="https://weblog.lol">weblog.lol</a>.</p>
</footer>

</body>
</html>