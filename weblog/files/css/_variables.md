Type: file
Content-Type: text/css
Title: _variables.css
Location: /_variables.css

/* weblog/files/css/_variables.md */
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
  --transition-speed: 0.3s;
  --spacing-unit: 1rem;
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

@media (prefers-reduced-motion: no-preference) {
  :root {
    scroll-behavior: smooth;
  }
}