---
layout: post
title: "sass: good practises"
categories: sass
table of content: <a href="../README.md">index</a>
---

####[Sass](#sass)

####[Comments](#sass-comments)

There is two schools:

  + some developers thinks that the code should be enough readable to be
    understandable even without documenting the code,

  + others thinks that the code should be commented, even if understandable,
    for maintainability.

Since I think that commenting is good practise, let's comment our code.

A comment is a description of how will behave a line or a set of code.
It won't be interpreted or rendered.

In Sass a line of comments begins with ``//`` :

```
  //  Make linear-gradient available for all browsers
  //
  //  $fromColor is the top color
  //  $toColor is the bottom color
  @mixin linear-gradient($fromColor, $toColor) {
    [instructions..]
  }
```

You can do a block of comments like so:
```
  /*  Make linear-gradient available for all browsers
   *
   *  $fromColor is the top color
   *  $toColor is the bottom color
   */
  @mixin linear-gradient($fromColor, $toColor) {
    [instructions..]
  }
```

####[Sass-doc](#sass-doc)

[SassDoc](http://github.com/SassDoc/sassdoc) is a tool that permits
to make your comments in html, readable from a browser.
It also helps structuring your comments.

For example, given the previous code:

```
  /**
   * Make linear-gradient available for all browsers
   *
   *  @author leGuest
   *
   *  @param {Hexadecimal} $fromColor - top color
   *  @param {Hexadecimal} $toColor - bottom color
   */
  @mixin linear-gradient($fromColor, $toColor) {
    [instructions..]
  }
```

