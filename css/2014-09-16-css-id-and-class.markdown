---
layout: post
title: "css: id and classes"
comments: true
categories: css
table of content: <a href="../README.md">index</a>
---

####[CSS](#css)

####[Identifier](#css-identifier)

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

####[Class](#css-class)

A class is very similar to identifier. To declare a class, just replace
``id`` with ``class``:

```
  <p class="article">content</p>
```

The main difference is an identifier will declare a group of content.
It can be the menu, the articles content block, etc.
A class will be more specific to an item of this content, like a
articles' post.

Some css conventions, like [BEM](http://bem.info/), don't use identifier, but only class.




