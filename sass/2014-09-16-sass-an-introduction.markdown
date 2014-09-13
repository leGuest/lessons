---
layout: post
title: "sass: an introduction"
categories: sass
table of content: <a href="../README.md">index</a>
---

####[Sass](#sass)

####[Reusability](#reusability)

__DRY (Do not Repeat Yourself)__ is a very important concept
in programmation.

Developer is lazy, he does not want to do the write the 
same thing again and again.

So he will use tricks like store colors into variables,
seen in [this lesson](../css/2014-09-15-css-preprocessors.markdown#concrete-example).

This for __reusability__.

####[Reusing colors](#reusing-colors)

Taking back ``colors.sass``:

```
  $blue-primary: #2c9ab7;
  $green-primary: #449a88;
  $yellow-primary: #febe12;
  $orange-primary: #db3a1b;
  $grey-primary: #373737;
```

We can also make a file for font-size, line-height, font-family,
etc, in ``typography.sass``

```
  $width: 960px;
  $baseline: 20px;
  $base-font-size: 16px;
  $h1-font-size: font-size: 25.9px;
  $h2-font-size: 41.9px;
  $h3-font-size: 67.8px;
```

```
p{
  color: $grey-primary;
  font-size: $font-size;
  line-height: $baseline;
}

h1{
  color: $orange-primary;
  font-size: $h1-font-size;
}

h2, h3, h4, h5, h6{
  color: $green-primary;
}

h2 {
  font-size: $h2-font-size;
}

h3 {
  font-size: $h3-font-size;
}

ul{
  li{
    color: $grey-primary;
    font-size: $font-size;
    line-height: $baseline;
  }
}
```
