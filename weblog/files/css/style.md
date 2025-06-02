Type: File
Content-Type: text/css
Title: Style.css
Location: /css/style.css

/* weblog/files/css/style.md */
@import url('https://fonts.bunny.net/css?family=atkinson-hyperlegible:400,400i,700,700i|source-code-pro:400,700');
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://omgalol.cache.lol/profiles/icons/omg.lol-icons.css');
@import "/css/includes/_wrapper.css";
@import "/css/includes/_variables.css";
@import "/css/includes/_base.css";

/* HEADER */

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

/* FOOTER SOCIALS ICONS */
ul.socials {
  list-style: none;
  margin: 0 auto;
  padding: 0;
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  max-width: calc(6 * 3rem + 5 * 0.5rem);
  justify-content: center;
}

ul.socials li {
  flex: 0 0 auto;
  margin: 0;
  padding: 0;
}

ul.socials li a {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 3rem;
  height: 3rem;
  font-size: 1.75rem;
  text-decoration: none;
}

/* .footer-hr {
  width: 100%; 
  border: 0;
  height: 5px;
  border-radius: 5px;
  background-color: #f8f8f2;
  margin-bottom: 10px;
  display: flex;
  margin: 1em 0;
} */

footer p {
  font-family: 'VC Honey Deck', serif;
/*  font-weight: bold; */
/*  font-size: 90%; */
  text-align: center;
  margin-top: 1em;
}

.footer-weblog-p {
  font-family: 'VC Honey Deck', serif;
  color: var(--text);
}

.footer-weblog-p a .logotype {
  font-family: 'VC Honey Black Banner', serif;
  color: #F783AC;
}

.footer-weblog-p a .logotype.dot {
  color: #F06595;
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

.fa-bluesky {
  color: #1185FE !important;
}

.fa-discord {
  color: #5865F2 !important;
}

.fa-github {
  color: #0d1117 !important;
}

/* .fa- {
  color: # !important;
} */

/* OMG LOL ICONS */
.omg-icon {
  color: var(--accent-1);
}

/* Individual OMG LOL ICONS */
.omg-proven {
  color: #FFD43D !important;
}

.omg-prami {
  color: #FF69AD !important;
}

.omg-verified {
  color: #FFD43D !important;
}

.omg-json-feed {
  color: #F36B2B !important;
}

/* .omg- {
  color: # !important;
} */
