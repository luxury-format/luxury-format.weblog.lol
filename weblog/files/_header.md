Type: file
Content-Type: text/css
Title: _header.css
Location: /_header.css

/* Weblog.lol/weblog/files/_header.md */
header {
  max-width: 60em;
  margin: 0 auto;
  padding: 0 1em;
}

/* Top row: logo/title on left, social icons on right */
.weblog-title {
  display: flex;
  justify-content: space-between;
  width: 100%;
  padding-top: 20px; /* 40px? */
}

.weblog-title a {
  text-decoration: none;
  color: var(--foreground);
}

.title-full {
  display: inline;
}

.title-short {
  display: none;
}

.header-logo {
  position: absolute;
  height: 75px;
  width: 75px;
  top: 20px;
}

.weblog-logo {
  display: flex;
  align-items: center;
}

.weblog-logo img {
  height: 2.5rem;
  gap: 0.5rem;
}

.weblog-logo h1 {
  margin: 0;
  font-size: 1.5rem;
  font-weight: 800;
}

/* Social icons next to logo */
.social a {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  color: var(--black);
  font-size: 1.2rem;
  text-decoration: none;
  margin-left: 0.75rem;
  transition: transform 0.1s;
}

.social a:hover {
  transform: translateY(-2px);
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

#header-hr {
  background-image: linear-gradient(to right, #bd93f9, #bd93f9, #44475a);
  border-radius: 5px;
  height: 2px;
  margin-bottom: 10px;
}

@media (max-width: 500px) {
  .title-full {
    display: none;
  }
  
  .title-short {
    display: inline;
  }
  
  #weblog-navigation ul {
    grid-template-columns: repeat(3, 1fr);
  }
}
