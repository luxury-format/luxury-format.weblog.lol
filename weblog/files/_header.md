Type: file
Content-Type: text/css
Title: _header.css
Location: /_header.css

/* Weblog.lol/weblog/files/_header.md */
/* Header structure */
.weblog-header {
  display: flex;
  flex-direction: column;
/*  width: 100%; */
  max-width: 100%;
  background-color: var(--accent);
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
/*  border-radius: var(--border-radius); */
}

.logo-title h1.weblog-title {
  margin: 0;
  font-size: 125%;
  font-weight: bold;
}

@media (max-width: 610px) {
    .weblog-title span.long {
        display: none;
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
  color: var(--black);
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
  color: var(--foreground);
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
    color: var(--foreground);
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
  background: var(--grey);
  border: 1px solid var(--purple);
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
  color: var(--foreground) !important;
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
