Type: file
Content-Type: text/css
Title: _base.css
Location: /_base.css

/* Weblog.lol/weblog/files/_base.md */
* {
  box-sizing: border-box;
}

body {
  padding: 0;
  margin: 0;
  font-family: var(--sans-serif);
  font-weight: normal;
  font-size: 115%;
  color: var(--foreground);
  background-color: var(--background);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

main {
  max-width: 60em;
  margin: 0.5em auto 1em;
  padding: 0 1em;
}

/* In Main & Page Templates: <main class="no-title-link"> */
/* In configuration: Title format: <h1 class="no-links"><a href="$location">$title</a></h1> */
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
  font-size: 2em;
}

h2 {
  font-size: 1.8em;
}

h3 {
  font-size: 1.6em;
}

h4 {
  font-size: 1.4em;
}

h5 {
  font-size: 1.2em;
}

h6 {
  font-size: 1em;
}

p {
  margin-bottom: 1rem;
  margin-top: 1rem;
  word-break: break-word;
}

p,
li {
  line-height: 150%;
}

ul li::marker {
  color: var(--green);
}

ol li::marker {
  color: var(--link);
}

a:link {
  color: var(--link);
  text-underline-offset: 2px;
  text-decoration: none;
}

a:visited {
  color: var(--link);
}

a:hover {
  color: var(--link-hover);
/*  text-decoration: underline; */
}

a:active {
  color: var(--link);
/*  text-decoration: underline; */
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
  font-size: 0.6em;
  vertical-align: sub;
  font-size: smaller;
  color: var(--red);
}

sup {
  font-size: 0.6em;
  vertical-align: super;
  font-size: smaller;
  color: var(--green);
}

blockquote {
  border-left: 3px solid var(--blue);
  color: var(--blue);
  font-style: italic;
  margin: 2rem 0;
  padding: 0 2rem;
}

a.footnote-ref {
  color: var(--green);
}

.ol-footnote {
  font-size: 0.8em;
  padding-inline-start: 2em;
}

.hr-footnote {
  border-top: 1px dashed var(--pink);
  background-color: transparent;
  width: 60%;
  margin: 0;
}

code,
pre {
  font-family: var(--monospace);
  font-size: 75%;
  line-height: 150%;
  box-shadow: var(--box-shadow);
  -webkit-box-shadow: var(--box-shadow);
  -moz-box-shadow: var(--box-shadow);
  border-radius: var(--border-radius);
  background: var(--black);
  color: var(--white);
}

pre {
  margin: 2rem 0;
  overflow-wrap: normal;
  overflow-x: scroll;
  padding: 2rem;
  white-space: pre;
  word-wrap: normal;
}

code {
  padding: 5px;
  margin: 0;
  white-space: pre-wrap;
  white-space: break-spaces;
  word-wrap: break-word;
  overflow-wrap: break-word;
}

pre code {
  background: none;
  border: none;
  color: inherit;
  padding: 0;
  white-space: pre;
}

img {
  display: block;
  max-width: 100%;
  margin-left: auto;
  margin-right: auto;
  border-radius: 1em;
  box-shadow: var(--box-shadow);
}

#profile-picture {
  display: block;
  margin: 0 auto;
}

table {
  border-collapse: collapse;
  width: 100%;
  margin-bottom: 0.5rem;
}

td,
th {
  padding: 0.75em;
  text-align: left;
  border: 1px solid var(--black);
}

th {
  background: var(--highlight);
  color: var(--purple);
  padding: 10px 5px;
}

td {
  padding: 5px 5px;
}

hr {
  border: 1px solid var(--blue);
  width: 100%;
  margin: 1em auto;
}

p code,
li code {
  padding: 0.2rem;
}

form.search {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  width: 100%;
}

form.search input {
  width: 100%;
  height: 40px;
  border-radius: var(--border-radius);
  font-weight: bold;
  background-color: var(--white);
  border: 2px solid var(--purple);
  color: var(--black);
}

form.search button {
  width: 100%;
  height: 40px;
  border-radius: var(--border-radius);
  font-weight: bold;
  background-color: var(--purple);
  border: 2px solid var(--white);
  color: var(--black);
}

form.search button:hover {
  background-color: var(--white);
  border-color: var(--purple);
}

.post-info,
.post-tags {
  font-size: 85%;
  color: var(--green);
  text-align: right;
}

.permalink {
  font-size: 85%;
  color: var(--yellow);
  text-align: right;
}

.post-info i:nth-child(2) {
  margin-left: .75em;
}

.tag {
  background: var(--green);
  color: var(--black) !important;
  padding: .3em .4em;
  margin: .8em 0 0 .4em;
  border-radius: .5em;
  text-decoration: none;
  display: inline-block;
}

.tag:hover {
  background: var(--grey);
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
  color: var(--black);
  gap: 1em;
  margin: 1em 0;
}

.divider::before,
.divider::after {
  content: "";
  flex: 1;
  border: 1px solid var(--blue);
}

.statuslol {
  background: #1c1c1e !important;
  border-radius: 0.5em !important;
  border: 1px solid #8e8e93 !important;
}

.statuslol_content {
  color: #f2f2f7 !important;
}

.statuslol_time a {
  opacity: 1 !important;
  color: #8E8E93 !important;
  border-bottom: none !important;
}

.statuslol_content p {
  font-size: 1em !important;
  text-align: left !important;
}

.statuslol_emoji {
  width: 1.5em !important;
}

.somepics_container {
  width: 100%;
  margin: 0 auto;
  border: 1px solid #8e8e93;
  border-radius: 0.5em;
  overflow: hidden;
}

.somepics_container img {
  display: block;
  width: 100%;
  height: auto;
  border-radius: 4px;
  transition: transform 0.3s ease;
}

.pagination {
  display: flex;
  justify-content: space-between;
  margin-bottom: 10px;
}
