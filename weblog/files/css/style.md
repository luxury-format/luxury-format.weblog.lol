Type: file
Content-Type: text/css
Title: style.css
Location: /style.css

/* weblog/files/css/style.md */
@import "_reset.css";
@import url('https://fonts.bunny.net/css?family=atkinson-hyperlegible:400,400i,700,700i|source-code-pro:400,700');
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://omgalol.cache.lol/profiles/icons/omg.lol-icons.css');

/* VARIABLES */
:root {
  color-scheme: light dark;
  --background: #F2F2F7;
  --background-dracula: #F8F8F2;
  --text: #1C1C1E;
  --text-dracula: #21222C;
  --link: #0080FF;
  --link-hover: #0062FF;
  --selection-dracula: #44475A;
  --comment-dracula: #6272A4;
  --accent-1: #8E8E93;
  --accent-2: #AEAEB2;
  --accent-3: #C7C7CC;
  --accent-4: #D1D1D6;
  --accent-5: #E5E5EA;
  --white: #FFFFFF;
  --white-black: #FFFFFF;
  --black: #000000;
  --black-white: #000000;
  --red: #FF3B30;
  --red-dracula: #FF5555;
  --orange: #FF9500;
  --orange-dracula: #FFB86C;
  --yellow: #FFCC00;
  --yellow-dracula: #F1FA8C;
  --green: #34C759;
  --green-dracula: #50FA7B;
  --mint: #00C7BE;
  --teal: #30B0C7;
  --cyan: #32ADE6;
  --cyan-dracula: #8BE9FD;
  --blue: #007AFF;
  --indigo: #5856D6;
  --purple: #AF52DE;
  --purple-dracula: #BD93F9;
  --pink: #FF2D55;
  --pink-dracula: #FF79C6;
  --brown: #A2845E;
  --border-radius: 0.5em;
  --box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.75);
  --title-font: 'VC Honey Deck', Georgia, serif;
  --sans-serif: 'Atkinson Hyperlegible', -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  --monospace: 'Source Code Pro', ui-monospace, 'Cascadia Code', Menlo, Consolas, 'DejaVu Sans Mono', monospace, SFMono-Regular, Monaco, "Andale Mono", "Ubuntu Mono";
}

@media (prefers-color-scheme: dark) {
  :root {
    --background: #1C1C1E;
    --background-dracula: #282A36;
    --text: #F2F2F7;
    --text-dracula: #FFFFFF;
    --link: #0062FF;
    --link-hover: #0080FF;
    --selection-dracula: #505A76;
    --comment-dracula: #7086C1;
    --accent-1: #8E8E93;
    --accent-2: #636366; 
    --accent-3: #48484A;
    --accent-4: #3A3A3C;
    --accent-5: #2C2C2E;
    --white: #FFFFFF;
    --white-black: #000000;
    --black: #000000;
    --black-white: #FFFFFF;
    --red: #FF453A;
    --red-dracula: #FF6E6E;
    --orange: #FF9F0A;
    --orange-dracula: #FFC78E;
    --yellow: #FFD60A;
    --yellow-dracula: #FFFFA5;
    --green: #28D158;
    --green-dracula: #69FF94;
    --mint: #63E6E2;
    --teal: #40C8E0;
    --cyan: #64D2FF;
    --cyan-dracula: #A4FFFF;
    --blue: #0A84FF;
    --indigo: #5E5CE6;
    --purple: #BF5AF2;
    --purple-dracula: #D6ACFF;
    --pink: #FF375F;
    --pink-dracula: #FF92DF;
    --brown: #AC8E68;
    --box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.7);
  }
}

/* BASE */
* {
  box-sizing: border-box;
}

body {
  padding: 0;
  margin: 0;
  font-family: var(--sans-serif);
  font-weight: normal;
  font-size: 115%;
  color: var(--text);
  background-color: var(--background);
}

main {
  max-width: 60em;
  margin: 0.5em auto 0.5em;
  padding: 0 1em;
}

/* In Main & Page Templates: <main class="no-title-link"> */
main.no-title-link h2 > a {
  color: inherit;
  text-decoration: none;
  pointer-events: none;
  cursor: default;
  text-shadow: rgba(10, 189, 240, 0.298039) 2px 2px 0px, rgba(254, 1, 1, 0.298039) -2px -2px 0px;
}

/* h2.no-links > a {
  text-decoration: none;
} */

.page-title {
    text-shadow: rgba(10, 189, 240, 0.298039) 1px 1px 0px, rgba(254, 1, 1, 0.298039) -1px -1px 0px;
}

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

li {
  font-family: var(--sans-serif);
/*  font-weight: bold; */
}

li a {
  font-family: var(--title-font);
}

ul li::marker {
  color: var(--red);
}

ol li::marker {
  color: var(--red);
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
  color: var(--green);
}

blockquote {
  display: block;
  margin: 1.5rem 0;
  padding: 1rem 1rem 1rem 1.5rem;
  border-left: 4px solid;
  border-color: var(--red);
  background: var(--accent-4);
  color: var(--text);
/*  font-style: italic; */
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
}

/* blockquote {
  border-left: 3px solid var(--blue);
  color: var(--blue);
  font-style: italic;
  margin: 2rem 0;
  padding: 0 2rem;
} */

a.footnote-ref {
  color: var(--red);
}

.ol-footnote {
  font-size: 0.8em;
  padding-inline-start: 2em;
}

.hr-footnote {
  border-top: 1px solid var(--blue);
  background-color: transparent;
  max-width: 100%;
  margin: 0;
}

pre {
  font-family: var(--monospace);
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
  font-family: var(--monospace);
  background: #282A36;
  color: var(--white);
  font-size: 75%;
  line-height: 150%;
  box-shadow: var(--box-shadow);
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
  border: 1px solid var(--black);
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
  border: 1px solid var(--blue);
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
  border-color: var(--indigo);
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

/* Remove margin on landing page */
.post-tags p {
  margin: 0;
}

.landing-post-info i {
  margin-right: 5px;
}

.page-post-info i {
  margin-right: 5px;
}

/* .post-info i:nth-child(2) {
  margin-left: 0.75em;
} */

.tag {
  background: var(--link);
  color: var(--black) !important;
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
  content: "\21C4";
  color: var(--text);
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

.landing-page-pagination {
  font-family: var(--title-font);
  display: flex;
  justify-content: space-between;
}

/* CONTAINER */
/* .container {
  width: 100%;
  margin: 0 auto;
  padding: 0 15px;
  margin-bottom: 10px;
}

.container-m {
  width: 100%;
  max-width: 1200px;
}

.container-sm {
  width: 100%;
  max-width: 800px;
} */

/* HEADER */
/* Header structure */
.weblog-header {
  display: flex;
  flex-direction: column;
/*  width: 100%; */
  max-width: 100%;
  background-color: var(--accent-5);
  padding: 1rem;
  margin: 1rem;
  border-radius: var(--border-radius);
}

/* First row: Logo+Title and Social Icons */
.header-top-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  margin-bottom: 1rem;
}

/* Logo and title container */
.logo-title {
  display: flex;
  align-items: center;
}

.logo-title a {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: inherit;
}

.logo-title img {
  height: 40px;
  margin-right: 10px;
  margin-left: 0;
  border-radius: var(--border-radius);
}

.logo-title h1.weblog-title {
  margin: 0;
  font-size: 125%;
  font-weight: bold;
}

.weblog-title span.long {
  display: inline;
}

.weblog-title span.short {
  display: none;
}

@media (max-width: 610px) {
  .weblog-title span.long {
    display: none;
  }
  
  .weblog-title span.short {
    display: inline;
  }
}

/* Icons container */
.header-icons {
  display: flex;
  grid-gap: 10px;
}

/* Icons styling */
.header-icons a {
  text-decoration: none;
  color: var(--accent-1);
  font-size: 1.5rem;
  transition: color 0.3s ease;
}

/* Icons color */
.header-icons .fa-mastodon {
  color: #563ACC;
}

.header-icons .fa-rss {
  color: #F36B2B;
}

.header-icons span {
  font-family: var(--title-font);
  color: var(--text);
  font-size: 90%;
}

@media (max-width: 610px) {
    .header-icons span {
        display: none;
    }
}

.header-icons i {
    width: 1em;
    height: 1em;
    margin-right: 5px;
}

.header-icons a:hover {
    color: var(--text);
    border-color: var(--blue);
}

/* Navigation menu styling */
.weblog-navigation {
  width: 100%;
}

nav {
  width: 100%;
}

#weblog-navigation ul {
  list-style-type: none;
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  grid-gap: 0.5rem;
  margin: 0;
  padding: 0;
  width: 100%;
}

#weblog-navigation li {
  background: var(--accent-4);
  border: 1px solid var(--indigo);
  border-radius: 0.5rem;
  padding: 0.5rem;
  font-size: 16px;
  display: flex;
  justify-content: center;
  text-align: center;
}

#weblog-navigation ul li a {
  font-weight: bold;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  color: var(--text) !important;
}

#weblog-navigation li a i {
  margin-right: 0.5rem;
}

/* Mobile responsiveness */
@media (max-width: 500px) {
  #weblog-navigation ul {
    grid-template-columns: repeat(3, 1fr);
  }
}

.page-navigation {
  background: var(--accent-4);
  border: 1px solid var(--indigo);
  border-radius: var(--border-radius);
  padding: 0;
  margin-top: 0.5em;
/*  font-size: 16px; */
  display: flex;
  justify-content: center;
  text-align: center;
}

/* NAV */
/* weblog/files/css/_nav.md */
/* nav.main {
  height: auto;
  padding: 5px 0;
  overflow: auto;
}

nav.main .container {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  grid-gap: 7px;
  margin-bottom: 5px;
}

@media (max-width: 550px) {
  nav.main .container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }
}

.nav-link, 
nav.main a {
  text-decoration: none;
  background-color: var(--white);
  color: var(--grey);
  text-transform: lowercase;
  font-size: .9em;
  font-family: var(--sans-serif);
  text-align: center;
  border-bottom: none;
  border-radius: 5px;
  padding: 2px 0;
  text-decoration: none;
  box-shadow: var(--box-shadow);
  transition: box-shadow var(--transition-speed) ease-in-out, color var(--transition-speed) ease-in-out;
}

.nav-link:hover, nav.main a:hover {
  box-shadow: none;
}

nav.main a.active {
  padding-left: 5px;
}
nav.main a.active:after {
  content: '.';
  color: var(--pink);
} */

/* PAGE NAV */
/* .header-nav {
  width: 100%;
  margin-top: 10px;
  border-bottom: 1px solid var(--grey);
  border-top: 1px solid var(--grey);
}

.header-nav:empty {
  display: none;
}

.header-nav ul {
  display: flex;
  list-style-type: none;
  grid-gap: 5px;
  justify-content: center;
  align-items: center;
  margin-block-start: 0;
  padding-inline-start: 0;
  flex-wrap: wrap;
  font-size: 0.9em;
  margin-bottom: 0;
  padding: 7px 0 9px 0;
}

.header-nav ul:before {
  content: '☰';
  font-style: italic;
}

.header-nav li ul {
  display: none;
} */

/* DRACULA HIGHLIGHT */
/* Dracula Theme v1.2.5
 *
 * https://github.com/dracula/highlightjs
 *
 * Copyright 2016-present, All rights reserved
 *
 * Code licensed under the MIT license
 *
 * @author Denis Ciccale <dciccale@gmail.com>
 * @author Zeno Rocha <hi@zenorocha.com>
 */

.hljs {
  display: block;
  overflow-x: auto;
  padding: 0.5em;
  background: #282a36;
}

.hljs-built_in,
.hljs-selector-tag,
.hljs-section,
.hljs-link {
  color: #8be9fd;
}

.hljs-keyword {
  color: #ff79c6;
}

.hljs,
.hljs-subst {
  color: #f8f8f2;
}

.hljs-title,
.hljs-attr,
.hljs-meta-keyword {
  font-style: italic;
  color: #50fa7b;
}

.hljs-string,
.hljs-meta,
.hljs-name,
.hljs-type,
.hljs-symbol,
.hljs-bullet,
.hljs-addition,
.hljs-variable,
.hljs-template-tag,
.hljs-template-variable {
  color: #f1fa8c;
}

.hljs-comment,
.hljs-quote,
.hljs-deletion {
  color: #6272a4;
}

.hljs-keyword,
.hljs-selector-tag,
.hljs-literal,
.hljs-title,
.hljs-section,
.hljs-doctag,
.hljs-type,
.hljs-name,
.hljs-strong {
  font-weight: bold;
}

.hljs-literal,
.hljs-number {
  color: #bd93f9;
}

.hljs-emphasis {
  font-style: italic;
}

/* FOOTER */
/* footer.main {
  font-family: var(--cbr);
  overflow: auto;
  text-align: center;
  padding: 0 10px;
  font-size: 0.8em;
}

.footer-buttons {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(88px, 1fr));
  grid-gap: 10px;
  margin-bottom: 20px;
  justify-content: space-between;
}

.footer-buttons div {
  display: flex;
  justify-content: center;
} */

footer {
  text-align: center;
  max-width: 60em;
  margin: 1.5em 0;
  padding: 0 1em;
}

.footer-hr {
  width: 100%; 
  border: 0;
  height: 5px;
  border-radius: 5px;
  background-color: #f8f8f2;
  margin-bottom: 10px;
  display: flex;
  margin: 1em 0;
}

footer p {
  font-family: 'VC Honey Deck', serif;
/*  font-weight: bold; */
  font-size: 90%;
  text-align: center;
  margin-top: 1em;
}

/* In footer: <p class="footer-weblog-p">Made with <a href="https://weblog.lol">Weblog.lol</a>.</p> */
.footer-weblog-p {
  font-family: 'VC Honey Deck', serif;
}

.footer-weblog-p a {
  font-family: 'VC Honey Black Banner', serif;
}

/* HOME */
/* .home-projects {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 10px;
}

@media (max-width: 650px) {
  .home-projects {
    grid-template-columns: repeat(1, 1fr);
  }
}

.home-project {
  height: 200px;
  background-position: 50%;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

.home-project a {
  border-top: 1px solid var(--white);
  border-bottom: 1px solid var(--white);
  padding: 10px 0;
  font-family: var(--sans-serif);
  width: 100%;
  text-align: center;
  background: rgba(0, 0, 0, 0.7);
}

.home-project a:hover {
  color: var(--white);
  border-top: 1px solid var(--white);
  border-bottom: 1px solid var(--white);
}

.webring--navicon {
  width: 25px;
  height: 25px;
}

.webring--randomicon {
  width: 30px;
  height: 30px;
}

.entryitem--webringbuttons {
  display: flex;
  grid-gap: 10px;
  align-items: center;
  justify-content: center;
} */

/* ICONS */
/* Font Awesome ICONS */
.fa-solid, 
.fa-regular, 
.fa-brands,
.fa-light,
.fa-thin,
.fa-duotone {
  color: var(--accent-1);
}

/* Individual Font Awesome ICONS */
.fa-mastodon {
  color: #563ACC !important;
}

.fa-face-grin {
  color: #FFCC00 !important;
}

.fa-rss {
  color: #F36B2B !important;
}

.fa-atom {
  color: #F36B2B !important;
}

/* .fa- {
  color: # !important;
} */

/* OMG LOL ICONS */
.omg-icon {
  color: var(--accent-1);
}

/* Individual OMG LOL ICONS */
.omg-icon.omg-proven {
  color: #FFD43D !important;
}

.omg-icon.omg-verified {
  color: #FFD43D !important;
}

.omg-icon.omg-json-feed {
  color: #F36B2B !important;
}

/* .omg-icon.omg- {
  color: # !important;
} */
