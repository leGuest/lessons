---
layout: post
title: "sass: mixins"
categories: sass
table of content: <a href="../README.md">index</a>
---

####[Sass](#sass)

####[Vendor](#sass-vendor)

In css, some rules are experimentals.
Since each browser (Chrome, Firefox, IE, Opera, Safari, etc)
experiments its own rules, you have the specify the so-rules
as experimental.

Each browser as it proper prefixes, called __vendor-prefixes__.
These prefixes go before the CSS property.

 + webkit (Chrome, Safari) : ``-webkit-rule``,

 + gecko (Firefox) : ``-moz-rule``,

 + old opera engine (Opera) : ``-o-rule``

These experiments are going directly in the specification
when enough stable, afterwards they become "normal" css property.

To display the CSS property on a maximum range of browsers and versions of its,
we need to include these vendors.

To know which version use the normalize version, [caniuse.com](http://caniuse.com)
is a usefull.

####[Mixins](#sass-mixins)

Mixins are a way of __grouping a set of properties__.
Since we [DRY](./sass/2014-09-16-sass-an-introduction),
we can regroup the vendor-prefixes for a specific property in
mixins.

An example with ``linear-gradient``.

  + [what is linear-gradient?](http://developer.mozilla.org/en-US/docs/Web/CSS/linear-gradient)

  + [caniuse - lineargradient](http://caniuse.com/#feat=css-gradients)

A mixin for it would be:

file: ``utils/gradient.sass``

```
  @mixin linear-gradient($fromColor, $toColor) {
    background-color: $toColor;
    background-image: -webkit-gradient(linear, left top, left bottom, from($fromColor), toColor($toColor));
    background-image: -webkit-linear-gradient(top,  $fromColor,   $toColor);
    background-image: -moz-linear-gradient(   top,  $fromColor,   $toColor);
    background-image: -ms-linear-gradient(    top,  $fromColor,   $toColor);
    background-image: -o-linear-gradient(     top,  $fromColor,   $toColor);
    background-image: linear-gradient(        top,  $fromColor,   $toColor);
    filter: progid:DXImageTransform.Microsoft.gradient(
      GradientType=0,
      StartColorStr='#{fromColor}',
      EndColorStr='#{$toColor}'
    );
  }
```

We declare that it's a mixin with ``@mixin``.
``$fromColor`` and ``$toColor`` are the data passed to the mixin.
That means that it will store into this variable the color we want to use.
This variable are called _parameters_

The ``filter`` property is for Internet Explorer.
We also provide a ``background-color`` in case the gradient is not supported.

Then we can use it in ``main.sass`` file:

```
  @import "utils/gradient";
  @import "colors";

  @include linear-gradient($green-primary, $orange-primary);
```

Result: [jsfiddle](http://jsfiddle.net/5jqztvqt/1/)

