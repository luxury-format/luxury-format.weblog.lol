Type: file
Content-Type: text/css
Title: Stylesheet
Location: /style.css

/* Weblog.lol/weblog/files/style.md */
@import url('https://fonts.bunny.net/css?family=atkinson-hyperlegible:400,400i,700,700i|source-code-pro:400,700');
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
  --input-bg: #FFFFFF;
  --input-text: #080808;
  --mark-text: #21222C;
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
    --input-bg: #333340;
    --input-text: #F8F8F2;
    --mark-text: #21222C;
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
  font-family: 'VC Honey Deck', Georgia, serif;
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
  font-family: 'VC Honey Deck', Georgia, serif;
  font-weight: bold;
  font-size: 90%;
  text-align: center;
  margin-top: 1em;
}

/* In footer: <p class="footer-weblog-p">Made with <a href="https://weblog.lol">Weblog.lol</a>.</p> */
.footer-weblog-p {
  font-family: 'VC Honey Black Banner', Georgia, serif;
}

i,
cite,
em {
  font-style: italic;
}

mark {
  color: var(--mark-text);
  background-color: var(--yellow);
}

s,
del {
  text-decoration: line-through;
  text-decoration-color: var(--red);
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

input {
  flex: 1;
  padding: 2px 10px;
  height: 30px;
  background-color: var(--input-bg);
  border-radius: 10px;
  border: 2px solid var(--purple);
  font-weight: bold;
  color: var(--input-text);
  width: 100%;
}

button {
  height: 30px;
  background-color: var(--purple);
  border-radius: 10px;
  border: 2px solid var(--background);
  font-weight: bold;
  color: var(--input-text);
  width: 100%;
  cursor: pointer;
}

button:hover {
  background-color: var(--background);
  border: 2px solid var(--purple);
  color: var(--foreground);
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
  color: var(--mark-text) !important;
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
  overflow-wrap: break-word;
}

pre {
  background: #000000;
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
  color: #FFFFFF;
  line-height: 1.5;
  margin: 2rem 0;
  overflow-wrap: normal;
  overflow-x: auto;
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
i[class^="omg-"] {
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

/* In Main & Page Templates: <body class="no-title-links"> <main class="no-title-link"> */
/* in configuration: Title format: <h1 class="no-links"><a href="$location">$title</a></h1> */
body.no-title-links main.no-title-link h1 > a {
  color: inherit;
  text-decoration: none;
  pointer-events: none;
  cursor: default;
}
