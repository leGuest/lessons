---
layout: post
title: "css: an introduction"
comments: true
categories: css
table of content: <a href="../README.md">index</a>
---

####[CSS](#css)
====

####[Block style CSS](#block-css)

If I want to put a colored set of text, I would do like so:

```
  <p style="color:red;">
    I am red paragraph
  </p>
  <h1 style="color:red;">
    I am red title
  </h1>
  <h2 style="color:purple;">
    I am purple title
  </h2>
  <h3 style="color:purple;">
    I am purple title
  </h3>
  <ul style="color:red;">
    <li style="color:blue;">
      I am blue item A
    </li>
    <li style="color:blue;">
      I am blue item B
    </li>
    <li style="color:blue;">
      I am blue item C
    </li>
  </ul>
```

This might be boring to repeat each time
the same CSS property.

You can regroup these CSS property by instructions, like this:
```
  <style type="text/css" media="all">
    p, h1{
      color: red;
    }
    h2{
      color: purple;
    }
    ul{
      color:red;
    }
    li{
      color: blue
    }
  </style>

  <p>
    I am red paragraph
  </p>
  <h1>
    I am red title
  </h1>
  <h2>
    I am purple title
  </h2>
  <h3>
    I am purple title
  </h3>
  <ul>
    <li>
      I am blue item A
    </li>
    <li>
      I am blue item B
    </li>
    <li>
      I am blue item C
    </li>
  </ul>
```
And this will have the same result.

Inline css result: http://jsfiddle.net/6p5vfgg6/

Block css result: http://jsfiddle.net/6p5vfgg6/1/

At first line of the ``style`` tag,
I have ``p, h1{``. This telling the browser that every ``<p>`` _and_ ``<h1>``
that it will encounter will follow the instruction between brackets (``{}``).

``color:red;`` is the same instrution as inline CSS, so it will change the text inside
``p`` and ``h1`` tag to red color.

You can see that block css is nothing more than grouping inline css styles by tag.
