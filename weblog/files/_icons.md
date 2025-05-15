Type: file
Content-Type: text/css
Title: _icons.css
Location: /_icons.css

/* Weblog.lol/weblog/files/_icons.md */
/* Color for all Font Awesome icons */
.fa-solid, 
.fa-regular, 
.fa-brands,
.fa-light,
.fa-thin,
.fa-duotone {
  color: var(--icons);
}

/* Individual icons color */
.fa-rss {
  color: #F36B2B !important;
}

/* Icons hover effects */
a:hover .fa-solid,
a:hover .fa-regular,
a:hover .fa-brands,
a:hover .fa-light,
a:hover .fa-thin,
a:hover .fa-duotone {
  color: var(--icons);
}

/* Keep individual icon color on hover */
a:hover .fa-rss {
  color: #F36B2B !important;
}

i[class*="omg-"] {
  color: var(--icons) !important;
}
