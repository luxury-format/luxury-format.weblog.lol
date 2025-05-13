Type: file
Content-Type: text/css
Title: _base.css
Location: /_base.css

/* Weblog.lol/weblog/files/_base.md */
* {
  box-sizing: border-box;
}

body {
  line-height: 1.6;
  padding: 0;
  margin: 0;
  font-family: var(--sans-serif);
  font-weight: normal;
  font-size: 1.2rem;
  color: var(--foreground);
  background-color: var(--background);
}

p {
  margin-bottom: 1rem;
  margin-top: 1rem;
  word-break: break-word;
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

a {
  color: var(--link);
  text-underline-offset: 2px;
}

a:hover {
  color: var(--white);
}

hr {
  border: 1px solid var(--pink);
  width: 100%;
  margin: 1rem auto;
  
}

code {
  white-space: break-spaces;
  margin: 0;
  color: var(--white);
  background: var(--black);
  border-radius: var(--border-radius);
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

img,
video {
  display: block;
  max-width: 100%;
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
}

blockquote {
  border-left: 3px solid var(--blue);
  color: var(--blue);
  font-style: italic;
  margin: 2rem 0;
  padding: 0 2rem;
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
  padding: .75em;
  text-align: left;
  border: 1px solid var(--selection);
}

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
