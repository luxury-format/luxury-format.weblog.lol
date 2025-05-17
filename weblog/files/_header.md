Type: file
Content-Type: text/css
Title: _header.css
Location: /_header.css

/* Weblog.lol/weblog/files/_header.md */
/* Header container with space-between  */
.site-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
  width: 100%;
  background-color: var(--accent);
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
}

.logo-title h1.weblog-title {
  margin: 0; 
/*  margin-top: 20px; */
  font-size: 125%;
  font-weight: bold;
}

/* Social icon container */
.social-icons {
  display: flex;
/*  margin-top: 20px; */
  gap: 10px;
}

/* Icon styling */
.social-icons a {
  text-decoration: none;
  color: #000000;
  font-size: 1.5rem;
  transition: color 0.3s ease;
}

/* Icon hover effects */
.social-icons a:hover {
  color: var(--link-hover);
}

/* Specific icon colors if needed */
.social-icons .fa-mastodon {
  color: #563ACC;
}

.social-icons .fa-rss {
  color: #F36B2B;
}

#navigation-bar {
  margin-top: 25px;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
  width: 100%;
}

#weblog-navigation ul {
  list-style-type: none;
  display: grid;
  grid-gap: 0.5rem;
  grid-template-columns: repeat(6, 1fr);
  margin: 0;
  padding: 0;
  max-width: 100%;
}

#weblog-navigation li {
  background: var(--grey);
  border: 1px solid var(--purple);
  border-radius: 0.5rem;
  padding: 0.5rem;
  font-size: 16px;
  display: flex;
  justify-content: space-evenly;
}

#weblog-navigation ul li a {
  font-weight: bold;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  color: var(--foreground) !important;
}

#weblog-navigation ul li a:hover,
#weblog-navigation ul li a:focus,
#weblog-navigation ul li a:active {
  text-decoration: none;
  color: var(--link) !important;
}

#weblog-navigation li a i {
  margin-right: 0.5rem;
}

@media (max-width: 500px) {
  #weblog-navigation ul {
    grid-template-columns: repeat(3, 1fr);
  }
}
