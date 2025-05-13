Type: file
Content-Type: text/css
Title: _highlight.css
Location: /_highlight.css

/* Weblog.lol/weblog/files/_highlight.md */
code[class*="language-"],
pre[class*="language-"] {
  text-align: left;
  white-space: pre;
  word-spacing: normal;
  word-break: normal;
  word-wrap: normal;
  color: #eee;
  background: #2f2f2f;
  font-family: var(--monospace);
  font-size: 0.9em;
  line-height: 1.5em;

  -moz-tab-size: 4;
  -o-tab-size: 4;

  tab-size: 4;

  -webkit-hyphens: none;
  -moz-hyphens: none;
  -ms-hyphens: none;
  hyphens: none;
}

code[class*="language-"]::-moz-selection,
pre[class*="language-"]::-moz-selection,
code[class*="language-"] ::-moz-selection,
pre[class*="language-"] ::-moz-selection {
  background: #faa2c1;
}

code[class*="language-"]::selection,
pre[class*="language-"]::selection,
code[class*="language-"] ::selection,
pre[class*="language-"] ::selection {
  background: #faa2c1;
}

:not(pre) > code[class*="language-"] {
  white-space: normal;
  border-radius: 0.2em;
  padding: 0.1em;
}

pre[class*="language-"] {
  overflow: auto;
  position: relative;
  margin: 0.5em 0;
  padding: 1.25em 1em;
}

.language-css > code,
.language-sass > code,
.language-scss > code {
  color: #fd9170;
}

[class*="language-"] .namespace {
  opacity: 0.7;
}

.token.atrule {
  color: #c792ea;
}

.token.attr-name {
  color: #ffcb6b;
}

.token.attr-value {
  color: #a5e844;
}

.token.attribute {
  color: #a5e844;
}

.token.boolean {
  color: #c792ea;
}

.token.builtin {
  color: #ffcb6b;
}

.token.cdata {
  color: #80cbc4;
}

.token.char {
  color: #80cbc4;
}

.token.class {
  color: #ffcb6b;
}

.token.class-name {
  color: #f2ff00;
}

.token.comment {
  color: #616161;
}

.token.constant {
  color: #c792ea;
}

.token.deleted {
  color: #ff6666;
}

.token.doctype {
  color: #616161;
}

.token.entity {
  color: #ff6666;
}

.token.function {
  color: #c792ea;
}

.token.hexcode {
  color: #f2ff00;
}

.token.id {
  color: #c792ea;
  font-weight: bold;
}

.token.important {
  color: #c792ea;
  font-weight: bold;
}

.token.inserted {
  color: #80cbc4;
}

.token.keyword {
  color: #c792ea;
}

.token.number {
  color: #fd9170;
}

.token.operator {
  color: #89ddff;
}

.token.prolog {
  color: #616161;
}

.token.property {
  color: #80cbc4;
}

.token.pseudo-class {
  color: #a5e844;
}

.token.pseudo-element {
  color: #a5e844;
}

.token.punctuation {
  color: #89ddff;
}

.token.regex {
  color: #f2ff00;
}

.token.selector {
  color: #ff6666;
}

.token.string {
  color: #a5e844;
}

.token.symbol {
  color: #c792ea;
}

.token.tag {
  color: #ff6666;
}

.token.unit {
  color: #fd9170;
}

.token.url {
  color: #ff6666;
}

.token.variable {
  color: #ff6666;
}

/* Dracula Syntax Highlighting */
/* The theme used by the syntax highlighting app */
.hljs {
  display: block;
  overflow-x: auto;
  background: #282a36;
  color: var(--white);
}

.hljs-comment,
.hljs-quote,
.hljs-variable {
  color: #50fa7b;
}

.hljs-keyword,
.hljs-selector-tag,
.hljs-built_in,
.hljs-name,
.hljs-tag {
  color: #8be9fd;}

.hljs-string,
.hljs-title,
.hljs-section,
.hljs-attribute,
.hljs-literal,
.hljs-template-tag,
.hljs-template-variable,
.hljs-type,
.hljs-addition {
  color: #ffb86c;
}

.hljs-deletion,
.hljs-selector-attr,
.hljs-selector-pseudo,
.hljs-meta {
  color: #2b91af;
}

.hljs-doctag {
  color: #808080;
}

.hljs-attr {
  color: #ff5555;
}

.hljs-symbol,
.hljs-bullet,
.hljs-link {
  color: #00b0e8;
}

.hljs-emphasis {
  font-style: italic;
}

.hljs-strong {
  font-weight: bold;
}

.hljs-number {
  color: var(--red);
}