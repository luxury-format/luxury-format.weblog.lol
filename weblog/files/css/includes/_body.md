Type: File
Content-Type: text/css
Title: _Body.css
Location: /css/includes/_body.css

/* GitHub file path:
weblog/files/css/includes/_body.md */

/* BODY CSS */
* {
  box-sizing: border-box;
}

/* BODY */
.body {
  font-family: var(--body-font);
  font-weight: 400;
  font-size: 14px;
  color: var(--text);
  background: var(--background);
  width: 100%;
  max-width: 1200px;
  margin: 1rem;
  padding: 0;
  overflow: auto;
}

/* HEADER */
.header {
  display: flex;
  flex-direction: column;
  max-width: 100%;
  width: 1200px;
  background-color: var(--accent-5);
  padding: 1rem;
  margin: 0;
  border-radius: 0.5rem;
}

/* MAIN */
.main {
  width: 100%;
  max-width: 1200px;
  margin: 0;
  padding: 0;
}

/* FOOTER */
.footer {
  font-family: var(--title-font);
  font-size: 0.8em;
  overflow: auto;
  text-align: center;
  width: 100%;
  max-width: 1200px;
  margin: 0.5rem 0;
  padding: 0.5rem 0;
}
