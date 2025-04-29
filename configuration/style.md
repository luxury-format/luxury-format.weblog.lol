Type: Template
Title: style.css
Location: /

@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/font-lato-regular.css');
@import url('https://static.omg.lol/type/font-lato-bold.css');
@import url('https://static.omg.lol/type/font-lato-italic.css');
@import url('https://static.omg.lol/type/font-md-io.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');

:root {
  --foreground: #21222C;
  --background: #F8F8F2;
  --link: #0080FF;
  --accent: #C0C0C0;
  --box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.75);
}

@media (prefers-color-scheme: dark) {
  :root {
    --foreground: #F8F8F2;
    --background: #21222C;
    --link: #7DF9FF;
    --accent: #E5E4E2;
    --box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.7);
  }
}

* {
  box-sizing: border-box;
}

body {
  font-family: 'Lato', sans-serif;
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

p,
li {
  line-height: 160%;
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
  margin-top: 1em;
  font-size: 90%;
  text-align: center;
}

a:link {
  color: var(--link);
  text-decoration: none;
}

a:visited {
  color: var(--link);
}

a:hover {
  color: var(--link);
}

a:active {
  color: var(--link);
}

.post-info,
.post-tags {

code {
  padding: .2em .3em;
  border: 1px solid var(--accent);
  white-space: pre-wrap;
  word-wrap: break-word; 
}

pre,
code {
  font-family: 'MD IO 0.4';
  font-size: 90%;
}

pre code {
  background: #000;
  color: #eee;
  display: inline-block;
  padding: 1em;
  white-space: pre-wrap;
  word-wrap: break-word;
}

img {
  max-width: 100%;
  border-radius: 0.5rem;
  box-shadow: var(--box-shadow);
}

table {
  border-collapse: collapse;
}

td,
th {
  padding: .75em;
  text-align: left;
  border: 1px solid var(--accent);
}

.weblog-title a {
  text-decoration: none;
  color: var(--foreground);
}

.previous-page + .next-page::before {
  content: "\2022";
  color: #ccc;
  margin: 0 0.75em;
}

.divider {
  display: flex;
  align-items: center;
  text-align: center;
  word-spacing: 1em;
  color: #ccc;
  gap: 1em;
  margin: 1em 0;
}

.divider::before,
.divider::after {
  content: "";
  flex: 1;
  border: 1px solid #ccc;
}

i[class^="fa-"],
i[class*=" fa-"],
i[class^="omg-"],
i[class*=" omg-"] {
  color: var(--accent);
}
