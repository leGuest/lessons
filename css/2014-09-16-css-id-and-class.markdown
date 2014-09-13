---
layout: post
title: "css: id and classes"
comments: true
categories: css
table of content: <a href="../README.md">index</a>
---

####[CSS](#css)

####[Id](#css-identifier)

You can add a property to HTML to group or splits some HTML tag,
by _using an identifier called id_.

If we take a content like so:

```
  <p>content</p>
```

can be identified like so:

```
  <p id="articles">content</p>
```

This will not change the formatting of the content.

How ever you can use it in css. A set of instrucitons like so:

```
  p{
    color: red;
  }
```

will be:

```
  p#articles{
    color: blue;
  }
```

the ``#`` link the HTML id to the css instructions.

Result: [jsfiddle](http://jsfiddle.net/007tcjnu/)


