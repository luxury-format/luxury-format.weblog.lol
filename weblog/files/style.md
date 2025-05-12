Type: file
Content-Type: text/css
Title: Stylesheet
Location: /style.css

/* Weblog.lol/weblog/files/style.md */
@import url(https://fonts.bunny.net/css?family=atkinson-hyperlegible:400,400i,700,700i|source-code-pro:400,700);
@import url('https://static.omg.lol/type/font-honey.css');
@import url('https://static.omg.lol/type/font-md-io.css');
@import url('https://static.omg.lol/type/fontawesome-free/css/all.css');
@import url('https://omgalol.cache.lol/profiles/icons/omg.lol-icons.css');

:root {
  --foreground: #21222C;
  --background: #F8F8F2;
  --link: #0080FF;
  --accent: #C0C0C0;
  --icons: #000000;
  --highlight: #E3E3E6;
  --selection: #44475A;
  --blue: #6272A4;
  --red: #FF5555;
  --orange: #FFB86C;
  --yellow: #F1FA8C;
  --green: #50FA7B;
  --purple: #BD93F9;
  --cyan: #8BE9FD;
  --pink: #FF79C6;
  --border-radius: 0.5rem;
  --box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.75);
}

@media (prefers-color-scheme: dark) {
  :root {
    --foreground: #F8F8F2;
    --background: #21222C;
    --link: #7DF9FF;
    --accent: #E5E4E2;
    --icons: #FFFFFF;
    --highlight: #53565D;
    --blue: #6272A4;
    --selection: #44475A;
    --red: #FF5555;
    --orange: #FFB86C;
    --yellow: #F1FA8C;
    --green: #50FA7B;
    --purple: #BD93F9;
    --cyan: #8BE9FD;
    --pink: #FF79C6;
    --box-shadow: 0px 5px 10px 0px rgba(0, 0, 0, 0.7);
  }
}

* {
  box-sizing: border-box;
}

body {
  font-family: 'Atkinson Hyperlegible', -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  font-size: 120%;
  color: var(--foreground);
  background: var(--background);
}

header nav ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

header nav li {
  display: inline-block;
  font-family: 'Atkinson Hyperlegible', -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
}

header nav li a {
  display: block;
  text-decoration: none;
  font-weight: bold;
  margin-right: 1em;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'VC Honey Deck', serif;
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
strong,
  text-align: center;
  word-spacing: 1em;
  color: var(--purple);
  gap: 1em;
  margin: 1em 0;
}

.divider::before,
.divider::after {
  content: "";
  flex: 1;
  border: 1px solid var(--purple);
}

i[class^="fa-"],
i[class*=" fa-"],
i[class^="omg-"],
i[class*=" omg-"] {
  color: var(--icons);
}

.recent-played {
  background-color: var(--blue);
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
  color: var(--link);
  font-weight: bold;
  padding: 0.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
}

.recent-played-track {
  margin: 0.5rem;
}

.statuslol {
  background-color: var(--blue) !important;
  border-radius: var(--border-radius);
  box-shadow: var(--box-shadow);
}
