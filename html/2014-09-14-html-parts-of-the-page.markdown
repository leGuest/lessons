---
layout: post
title: "html: an introduction"
categories: html
table of content: <a href="../README.md">index</a>
---

####[HTML](#html)
====

####[How to group a page?](#html-group-a-page)

Content of a page can be splitted in different elements.
Some does not usually change, like the _header_, other does, like the _container_.

A HTML5 page is usually regrouped like this:

```
  <!DOCTYPE html>
  <html>
    <head>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width">
      <title></title>
    </head>
    <body>
      <header id="header">
        logo + slogan + menu
      </header>
      <section id="content">
        content of a specific page
      </section>
      <footer id="footer">
        foot of the page
      </footer>
    </body>
  </html>
```

Sometimes ``header``, ``section``, and ``footer`` can be seen as ``div``:

```
  <!DOCTYPE html>
  <html>
    <head>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width">
      <title></title>
    </head>
    <body>
      <div id="header">
        logo + slogan + menu
      </div>
      <div id="content">
        content of a specific page
      </div>
      <div id="footer">
        foot of the page
      </div>
    </body>
  </html>
```

Don't worry about this ``id`` property yet, we'll come back later on it.

####[Schema](#html-schema)

<img src="../assets/images/html__layout--schema.png" width="400" alt="common html layout" />

