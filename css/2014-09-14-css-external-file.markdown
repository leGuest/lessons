---
layout: post
title: "external css file"
comment: true
categories: css
table of content: <a href="../README.md">index</a>
---

####[CSS](#css)
====

####[External CSS file](#external-css-file)

Bigger project, bigger ``style`` instructions bloc.

To prevent the html file to be unreadable due to this bloc, a file with extension ``.css``
can be created.

This file has the same instruction and behave exactly like the ``style`` instruction block; with
the exception that we dont need the ``style`` tag since the ``.css`` extension already tell the browser
that it's CSS.

However, the html file need to know that the css file exists, else it won't load.
To link the css from html, we put in the ``<head>`` :

```
  <head>
    [other informations...]
    <link rel="stylesheet" href="myexternalcsse.css" title="stylesheet" type="text/css" />
  </head>
```

Then create a file named ``myexternalfile.css``.

This way of inmplementing css is the current good practise.

