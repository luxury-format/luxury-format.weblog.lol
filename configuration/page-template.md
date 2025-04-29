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
  --icons: #000000;
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
  --border-radius: 0.5rem;
  --box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.75);
}

@media (prefers-color-scheme: dark) {
  :root {
    --foreground: #F8F8F2;
    --background: #21222C;
    --link: #7DF9FF;
    --accent: #E5E4E2;
    --icons: #FFFFFF;
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
  font-family: 'Atkinson Hyperlegible', -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
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
  font-family: 'Atkinson Hyperlegible', -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
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
  font-family: 'VC Honey Deck', serif;
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

h1,
h2,
h3,
h4,
h5,
h6,
b,
strong,
th {
  font-weight: bold;
}

h1 {
  font-size: 2.4rem;
}

h2 {
  font-size: 2.2rem;
}

h3 {
  font-size: 2rem;
}

h4 {
  font-size: 1.8rem;
}

h5 {
  font-size: 1.6rem;
}

h6 {
  font-size: 1.4rem;
}

p,
li {
  line-height: 120%;
}

header,
main,
footer {
  max-width: 60em;
  margin: 2em auto;
  padding: 0 1em;
}

header {
  margin-top: 1em;
}

footer p {
  font-family: 'VC Honey Deck', serif;
  font-weight: bold;
  font-size: 90%;
  text-align: center;
  margin-top: 1em;
}

i,
cite,
em {
  font-style: italic;
}

highlight,
mark {
  color: #21222C;
  background-color: var(--yellow);
}

s,
del {
  text-decoration: line-through;
  text-decoration-color: #FF3B30;
  text-decoration-thickness: 1px;
}

sub {
  vertical-align: sub;
  font-size: smaller;
}

sup {
  vertical-align: super;
  font-size: smaller;
}

hr {
  border: 0;
  height: 1px;
  background: var(--pink);
  margin: 1rem 0;
}

blockquote {
  border-left: 3px solid var(--blue);
  color: var(--blue);
  font-style: italic;
  margin: 2rem 0;
  padding: 0 2rem;
}

a {
  text-decoration: none;
}

a:link,
a:visited {
  color: var(--link);
}

a:hover,
a:active {
  color: var(--link);
  text-decoration: underline;
}

form.search {
  display: flex;
  flex-direction: column;
  width: 100%;
  gap: 1rem;
}

input[type="date"],
input[type="email"],
input[type="number"],
input[type="search"],
input[type="tel"],
input[type="text"],
input[type="url"],
input[type="button"],
input[type="submit"],
input[type="text" i] {
  flex: 1;
  padding: 2px 10px;
  height: 30px;
  background-color: #FFFFFF;
  border-radius: 10px;
  border: 2px solid var(--purple);
  font-weight: bold;
  color: #080808;
}

button {
  height: 30px;
  background-color: var(--purple);
  border-radius: 10px;
  border: 2px solid #FFFFFF;
  font-weight: bold;
  color: #080808;
  width: 100%;
  cursor: pointer;
}

button:hover {
  background-color: #FFFFFF;
  border: 2px solid var(--purple);
}

ul li::marker {
  color: var(--green);
}

ol li::marker {
  color: var(--link);
}

.post-info,
.post-tags {
  font-size: 80%;
  color: var(--green);
  text-align: right;
}

.post-info i:nth-child(2) {
  margin-left: .75em;
}

.tag {
  background: var(--green);
  color: #21222C !important;
  padding: .3em .4em;
  margin: .8em 0 0 .4em;
  border-radius: .5em;
  text-decoration: none;
  display: inline-block;
}

code,
kbd,
pre,
tt {
  font-family: 'Source Code Pro', ui-monospace, SFMono-Regular, Monaco, 'Andale Mono', 'Ubuntu Mono', monospace;
  font-size: 90%;
}

code {
  background: #000000;
  color: #FFFFFF;
  border-radius: var(--border-radius);
  padding: 2px 4px;
  white-space: pre-wrap;
	word-wrap: break-word;
/*  overflow-wrap: break-word; */
}

pre {
  background: #000000;
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
  color: #FFFFFF;
  line-height: 1.5;
  margin: 2rem 0;
  overflow-wrap: normal;
  overflow-x: scroll;
  padding: 2rem;
  white-space: pre;
  word-wrap: normal;
}

pre code {
  background: none;
  border: none;
  color: inherit;
  padding: 0;
  white-space: pre;
}

img,
picture,
video {
  display: block;
  max-width: 100%;
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
}

table {
  border-collapse: collapse;
  width: 100%;
}

th {
  background: var(--highlight);
}

td,
th {
  padding: .75em;
  text-align: left;
  border: 1px solid var(--selection);
}

.weblog-title a {
  text-decoration: none;
  color: var(--foreground);
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
  width: 100%;
}

.previous-page {
  margin-right: auto;
}

.next-page {
  margin-left: auto;
}

.previous-page:not(:empty) + .next-page:not(:empty)::before {
  content: "\2022";
  color: var(--link);
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
}

.divider {
  display: flex;
  align-items: center;
  text-align: center;
  word-spacing: 1em;
  color: var(--purple);
  gap: 1em;
  margin: 1em 0;
}

.divider::before,
.divider::after {
  content: "";
  flex: 1;
  border: 1px solid var(--purple);
}

i[class^="fa-"],
i[class*=" fa-"],
i[class^="omg-"],
i[class*=" omg-"] {
  color: var(--icons);
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
  background-color: var(--blue) !important;
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