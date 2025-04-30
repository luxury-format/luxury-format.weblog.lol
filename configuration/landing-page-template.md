Type: Template
Title: Landing Page Template
Location: /configuration/landing-page-template.md

<!DOCTYPE html>
<html lang="en">
<!-- From GitHub repo -->
<head>
<title>{weblog-title}</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="preconnect" href="https://fonts.bunny.net">
<link href="https://fonts.bunny.net/css?family=atkinson-hyperlegible:400,400i,700,700i|source-code-pro:200,200i,300,300i,400,400i,500,500i,600,600i,700,700i,800,800i,900,900i" rel="stylesheet" />
<link rel="preconnect" href="https://omgalol.cache.lol" crossorigin>
<link rel="stylesheet" href="https://omgalol.cache.lol/profiles/icons/omg.lol-icons.css">
<link rel="preconnect" href="https://cdnjs.cloudflare.com">
<link rel="preconnect" href="https://kit.fontawesome.com">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css">
<!-- Minified version -->
<link rel="stylesheet" href="https://cdn.simplecss.org/simple.min.css">
<!-- Un-Minified version -->
<link rel="stylesheet" href="https://cdn.simplecss.org/simple.css">
</head>
<body>

<header>
<h1 class="weblog-title"><a href="/">{weblog-title}</a></h1>
{navigation}
</header>
<main>

<span class="divider">&bull; &bull; &bull;</span>
{body}

<nav>
{previous-page}
{next-page}
</nav>
<span class="divider">&bull; &bull; &bull;</span>
</main>

<footer>
  <hr>
  <p>&copy; {year} <a href="/">{weblog-title}</a></p>
  <p>Made with <a href="https://weblog.lol">weblog.lol</a>.</p>
</footer>

</body>
</html>