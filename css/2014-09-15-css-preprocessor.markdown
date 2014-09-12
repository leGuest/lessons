---
layout: post
title: "css: preprocessor"
comments: true
categories: css
table of content: <a href="../README.md">index</a>
---

####[CSS](#css)
====

####[What is a CSS Preprocessor](#what-is-a-preprocessor)

A _preprocessor_ is language that will compile (transform) in
another langage.

Usually, preprocessors extends the _functionality of a langage_.
For example, we can store colors thanks to preprocessor, then 
reuse later, whenever we need it.

These storages will help to structure your files.
However, it's totally possible to use CSS without these preprocessors,
it depends on the project you're working on.

####[Current preprocessors](#current-preprocessors)

The current general ones are [lesscss](http://lesscss.org),
[stylus](http://learnboost.github.io/stylus), [sass](sass-lang.com).

There is also preprocessors for specifical needs like performance, but
we won't come to it.Just know that it exists.

We will use __sass__.
Sass files are just files with ``.sass`` extension.

####[Concrete example](#concrete-example)

Before we dive into it, just a simple example:

You can import files with sass,
thanks to [@import "file"](http://sass-lang.com/guide#topic-5).

We want to store colors.
we first create a file named ``colors.sass``,
like so :

```
  $blue-primary: #2c9ab7;
  $green-primary: #449a88;
  $yellow-primary: #febe12;
  $orange-primary: #db3a1b;
  $grey-primary: #373737;
```
_colors from [Mailchimp](http://mailchimp.com/about/brand-assets)_

To store a data, we declare a value where the data will be stored: it's
called a _variable_.

We name this variable $blue-primary instead of $blue because it's
a good practise. It helps _not being confused between the variable
and the color blue_ when we will use it.

The data is a color, exprimed in hexadecimal for _nuancing the color_.

Now, we create a main file, ``main.sass`` where
we will import the colors:

```
  import "colors";

  p{
    color: $blue-primary;
  }
```

Note that you dont need to tell the file extension when importing a sass file into
another. ``import "colors";`` is a shortcut for ``import "colors.sass"``.

The purpose of why structuring your css/sass files will be
approached later.

