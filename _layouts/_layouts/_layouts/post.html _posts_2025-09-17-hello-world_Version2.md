<!DOCTYPE html>
<html lang="zh-CN">
  <head>
    <meta charset="UTF-8">
    <title>{{ page.title | default: site.title }}</title>
    <meta name="description" content="{{ site.description }}">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="/assets/css/minimal.css">
  </head>
  <body>
    <header>
      <h1><a href="{{ site.baseurl }}/">{{ site.title }}</a></h1>
      <p>{{ site.description }}</p>
      <nav>
        <a href="{{ site.baseurl }}/">Home</a>
        <a href="{{ site.baseurl }}/categories.html">分类 Categories</a>
        <a href="{{ site.baseurl }}/tags.html">标签 Tags</a>
      </nav>
    </header>
    <main>
      {{ content }}
    </main>
    <footer>
      <small>&copy; {{ site.time | date: '%Y' }} {{ site.author }}</small>
    </footer>
  </body>
</html>
