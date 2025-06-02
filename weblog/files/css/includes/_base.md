Type: File
Content-Type: text/css
Title: _Base.css
Location: /css/includes/_base.css

/* GitHub file path:
weblog/files/css/includes/_base.md */
/* MAIN NO TITLE LINK */
/* In Main Template & Page Templates: <main class="no-title-link"></main> */
main.no-title-link h2 > a {
  color: inherit;
  text-decoration: none;
  pointer-events: none;
  cursor: default;
/*  text-shadow: rgba(10, 189, 240, 0.298039) 2px 2px 0px, rgba(254, 1, 1, 0.298039) -2px -2px 0px; */
}

/* .page-title {
  text-shadow: rgba(10, 189, 240, 0.298039) 1px 1px 0px, rgba(254, 1, 1, 0.298039) -1px -1px 0px;
}

.page-title + h6 {
  text-shadow: rgba(10, 189, 240, 0.298039) 1px 1px 0px, rgba(254, 1, 1, 0.298039) -1px -1px 0px;
} */

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: var(--title-font);
  text-align: center;
  margin: 0.5rem 0;
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
dt,
th {
  font-weight: 700;
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

li {
  font-family: var(--body-font);
}

li a {
  font-family: var(--title-font);
}

ul li::marker {
  color: var(--blue);
}

ol li::marker {
  color: var(--blue);
}

a:link,
a:visited {
  color: var(--link);
  text-decoration: none;
}

a:hover,
a:active {
  color: var(--link-hover);
  text-decoration: underline;
}

i,
cite,
em {
  font-style: italic;
}

mark {
  color: var(--text);
  background-color: var(--yellow);
}

s,
del,
strike {
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
  color: var(--red);
}

figure {
  padding: 0;
  margin: 0;
}

figcaption {
  background: var(--accent-1);
  border-radius: 0.6rem;
  color: var(--accent-3);
  display: block;
  font-size: 1.4rem;
  margin: -2rem 0 3rem;
  padding: .5rem 1.5rem;
  text-align: center;
}

blockquote {
  border-left: 3px solid var(--highlight);
  color: var(--accent-3);
  font-style: italic;
  margin: 2rem 0;
  padding: 0 2rem;
}

a.footnote-ref {
  color: var(--red);
}

.ol-footnote {
  font-size: 0.8em;
  padding-inline-start: 2em;
}

.hr-footnote {
  border-top: 1px solid var(--highlight);
  background-color: transparent;
  max-width: 100%;
  margin: 0;
}

pre {
  font-family: var(--code-font);
/*  background: var(--black); */
/*  color: var(--white); */
  font-size: 90%;
  line-height: 150%;
  box-shadow: var(--box-shadow);
  border-radius: var(--border-radius);
  overflow-wrap: normal;
/*  overflow-x: scroll; */
  white-space: pre;
  word-wrap: normal;
/*  padding: 1rem; */
}

code {
  font-family: var(--code-font);
  background: var(--black-black);
  color: var(--white-white);
  font-size: 75%;
  line-height: 150%;
/*  box-shadow: var(--box-shadow); */
  border-radius: var(--border-radius);
  white-space: pre-wrap;
  white-space: break-spaces;
  word-wrap: break-word;
  overflow-wrap: break-word;
}

pre code {
  background: none;
  border: none;
  color: inherit;
  white-space: pre;
}

img {
  display: block;
  max-width: 100%;
  margin-left: auto;
  margin-right: auto;
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
  border: 1px solid var(--black-white);
}

th {
  background: var(--accent-2);
  color: var(--blue);
  padding: 10px 5px;
}

td {
  padding: 5px 5px;
}

hr {
  border: 1px solid var(--highlight);
  width: 100%;
  margin: 1em 0;
}

p code,
li code {
  padding: 0.2rem;
}

form {
  display: flex;
  justify-content: space-evenly;
/*  width: 100%; */
}

form label {
  font-family: var(--title-font);
  text-align: center;
}

form input {
/*  width: 100%; */
  height: 30px;
  border-radius: var(--border-radius);
  font-weight: bold;
  background-color: var(--background);
  border: 2px solid var(--black-white);
  color: var(--text);
}

form button {
/*  width: 100%; */
  height: 30px;
  font-family: var(--title-font);
  font-weight: bold;
  color: var(--text);
  background-color: var(--link);
  border-radius: var(--border-radius);
  border: 2px solid var(--black-white);
}

form button:hover {
  background-color: var(--link-hover);
  border-color: var(--black-white);
}

.landing-post-info {
  font-family: var(--title-font);
  font-size: 85%;
  font-weight: bold;
  color: var(--text);
  text-align: right;
}

.page-post-info {
  font-family: var(--title-font);
  font-size: 85%;
  font-weight: bold;
  color: var(--text);
  text-align: right;
}

.post-tags {
  font-family: var(--title-font);
  font-size: 85%;
  font-weight: bold;
  color: var(--blue);
  text-align: right;
}

/* Margin on landing page */
.post-tags p {
  margin: 0;
}

.landing-post-info i {
  margin-right: 5px;
}

.page-post-info i {
  margin-right: 5px;
}

.tag {
  background: var(--link);
  color: var(--black-black) !important;
  padding: .3em .4em;
  margin: .8em 0 0 .4em;
  border-radius: .5em;
  text-decoration: none;
  display: inline-block;
}

.tag:hover {
  background: var(--link-hover);
}

.previous-page {
  margin-right: auto;
}

.next-page {
  margin-left: auto;
}

.previous-page:not(:empty) + .next-page:not(:empty)::before {
  font-family: "Font Awesome 6 Free";
  font-weight: 900;
  speak: none;
  font-style: normal;
  content: "\f0ec";
  color: var(--highlight);
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
}

.divider {
  display: flex;
  align-items: center;
  text-align: center;
  word-spacing: 1em;
  color: var(--text);
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
  background: var(--accent-5) !important;
  border-radius: 0.5em !important;
  border: 1px solid var(--highlight) !important;
}

.statuslol_content {
  color: var(--white-white) !important;
}

.statuslol_time a {
  opacity: 1 !important;
  color: var(--hihglight) !important;
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
  border: 1px solid var(--highlight);
  border-radius: 0.5em;
  overflow: hidden;
}

.somepics_container img {
  display: block;
  width: 100%;
  height: auto;
  border-radius: 4px;
}

.pagination {
  font-family: var(--title-font);
  display: flex;
  justify-content: space-between;
}
