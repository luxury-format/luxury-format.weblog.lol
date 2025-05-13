Type: file
Content-Type: text/css
Title: _base.css
Location: /_base.css

/* Weblog.lol/weblog/files/_base.md */
@import url('https://fonts.bunny.net/css?family=atkinson-hyperlegible:400,400i,700,700i|source-code-pro:400,700');
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/font-md-io.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://omgalol.cache.lol/profiles/icons/omg.lol-icons.css');

* {
  box-sizing: border-box;
}

body {
  line-height: 1.6;
  padding: 0;
  margin: 0;
  font-family: var(--sans-serif);
  font-weight: normal;
  font-size: 1.8rem;
  color: var(--foreground);
  background-color: var(--background);
}

main {
  max-width: 60em;
  margin: 2em auto;
  padding: 0 1em;
}

i[class^="fa-"],
i[class^="omg-"] {
  color: var(--icons);
}

/* In Main & Page Templates: <main class="no-title-link"> */
/* in configuration: Title format: <h1 class="no-links"><a href="$location">$title</a></h1> */
main.no-title-link h1.no-links > a {
  color: inherit;
  text-decoration: none;
  pointer-events: none;
  cursor: default;
}

h1.no-links > a {
  text-decoration: none;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: var(--title-font);
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
strong {
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

p {
  margin-bottom: 1rem;
  margin-top: 1rem;
  word-break: break-word;
}

p,
li {
  line-height: 1.2rem;
}

ul li::marker {
  color: var(--green);
}

ol li::marker {
  color: var(--link);
}

a {
  color: var(--link);
  text-underline-offset: 2px;
  text-decoration: none;
}

a:hover {
  color: var(--white);
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

i,
cite,
em {
  font-style: italic;
}

mark {
  color: var(--mark);
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

blockquote {
  border-left: 3px solid var(--blue);
  color: var(--blue);
  font-style: italic;
  margin: 2rem 0;
  padding: 0 2rem;
}

code,
kbd,
pre,
tt {
  font-family: var(--monospace);
  font-size: 0.9rem;
}

code {
  white-space: break-spaces;
  margin: 0;
  pading: 0; /* 2px, 4px; */
  color: var(--white);
  background: var(--black);
  border-radius: var(--border-radius);
  white-space: pre-wrap;
  word-wrap: break-word;
  overflow-wrap: break-word;
}

pre {
  background: var(--black);
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
  color: var(--white);
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
  margin-bottom: 0.5rem;
}

th {
  background: var(--highlight);
}

td,
th {
  padding: 0.75em;
  text-align: left;
  border: 1px solid var(--selection);
}

hr {
  border: 1px solid var(--pink);
  width: 100%;
  margin: 1rem auto;
}

p code,
li code {
  padding: 0.2rem;
}

input,
textarea {
  border: 1px solid #4a4a4a;
}

input:focus,
textarea:focus {
  border: 1px solid #1d7484;
}

textarea {
  width: 100%;
}

form.search {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  width: 100%;
}

form.search input,
form.search button {
  width: 100%;
  height: 1.2rem;
  padding: 2px 10px;
  border-radius: 10px;
  font-weight: bold;
}

form.search input {
  background-color: var(--white);
  border: 2px solid var(--purple);
  color: var(--foreground);
}

form.search button {
  background-color: var(--purple);
  border: 2px solid var(--white);
  color: var(--foreground);
}

form.search button:hover {
  background-color: var(--white);
  border-color: var(--purple);
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
  color: var(--foreground) !important;
  padding: .3em .4em;
  margin: .8em 0 0 .4em;
  border-radius: .5em;
  text-decoration: none;
  display: inline-block;
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

/* .statuslol {
  background-color: var(--blue) !important;
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
} */

@media (max-width: 650px) {
  body {
    font-size: 1rem;
  }
}

.pagination {
  display: flex;
  justify-content: space-between;
  margin-bottom: 10px;
}
