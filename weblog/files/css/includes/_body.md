Type: File
Content-Type: text/css
Title: _Body.css
Location: /css/includes/_body.css

/* BODY CSS */
/* GitHub file path:
weblog/files/css/includes/_body.md */
* {
  box-sizing: border-box;
}

/* BODY */
.body {
  font-family: var(--body-font);
  font-weight: 400;
  font-size: 14px;
  overflow: auto;
  color: var(--text);
  background: var(--background);
  width: 100%;
  max-width: 1200px;
  margin: 1rem;
  border: 1px solid var(--red);
  border-radius: 0.5rem;
  padding: 1rem;
}

/* HEADER */
.header {
  display: flex;
  flex-direction: column;
  max-width: 100%;
  width: 1200px;
  background: var(--accent-5);
  margin: 1rem;
  border: 1px solid var(--yellow);
  border-radius: 0.5rem;
  padding: 1rem;
}

/* MAIN */
.main {
  width: 100%;
  max-width: 1200px;
  margin: 1rem;
  border: 1px solid var(--green);
  border-radius: 0.5rem;
  padding: 1rem;
}

/* FOOTER */
.footer {
  font-family: var(--title-font);
  font-weight: 700;
  font-size: 0.8em;
  overflow: auto;
  text-align: center;
  width: 100%;
  max-width: 1200px;
  margin: 1rem;
  border: 1px solid var(--pink);
  border-radius: 0.5rem;
  padding: 1rem;
}
