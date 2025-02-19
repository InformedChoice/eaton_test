<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>{{ .Title }}</title>
</head>
<body>
  <header>
    <h1>{{ .Title }}</h1>
    <p>Solomon, Christian, Miriam, and Shyloe Reading.</p>
  </header>
  
  <section>
    <h2>Chapters</h2>
    <ul>
      {{ range where .Site.RegularPages "Section" "post" }}
        <li>
          <a href="{{ .Permalink }}">{{ .Title }}</a>
        </li>
      {{ end }}
    </ul>
  </section>
</body>
</html>
