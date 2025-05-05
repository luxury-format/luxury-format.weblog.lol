Type: Template
Title: Page Template

<!DOCTYPE html>
<html lang="en">
<!-- From GitHub repo -->
<head>
<title>{weblog-title}{separator}{post-title}</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="preconnect" href="https://fonts.bunny.net">
<link href="https://fonts.bunny.net/css?family=atkinson-hyperlegible:400, 400i, 700, 700i | source-code-pro: 400, 400i, 700, 700i" rel="stylesheet" />
<link rel="preconnect" href="https://omgalol.cache.lol" crossorigin>
<link rel="stylesheet" href="https://omgalol.cache.lol/profiles/icons/omg.lol-icons.css">
<link rel="preconnect" href="https://cdnjs.cloudflare.com">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css">
</head>
<body>

<header>
  <h1 class="weblog-title"><a href="/">{weblog-title}</a></h1>
  {navigation}
</header>

<main>

{body}

</main>

<footer>
  <hr>
  <p>&copy; {year} <a href="/">{weblog-title}</a></p>
  <p>Made with <a href="https://weblog.lol">Weblog.lol</a>.</p>
</footer>

</body>
</html>