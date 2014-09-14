---
layout: post
title: "sass: case study - bootstrap - part 2"
categories: sass
table of content: <a href="../README.md">index</a>
---

####[Sass](#sass)

####[Main file](#sass-main-file)

the main file,
[\_bootstrap.scss](https://githhub.com/twbs/bootstrap-sass/blob/master/assets/stylesheets/_bootstrap.scss),
is composed of imports files.

This __modular__ approach permits to know where an instruction for a specific CSS is. 
And so quickly be able to read, change, or delete when there is a bug, or a new feature.

Let's take this file and anlyze the imports, one by one.


####[Variables](#sass-variables)

| file            | location                                    | imported from                   |
|-----------------|---------------------------------------------|---------------------------------|
| variables.scss  |[./bootstrap/\_variables.scss][variables]    |[./\_bootstrap.scss][main]       |

[variables]: ../bower_components/bootstrap-sass-official/assets/stylesheets/bootstrap/\_variables.scss
[main]: ../bower_components/bootstrap-sass-official/assets/stylesheets/\_bootstrap.scss#L2

----

[L15](../bower_components/bootstrap-sass-official/assets/stylesheets/\_bootstrap.scss#L15) :
``$gray-darker: lighten(#000, 13.5%) !default; // #222``

3 things here:

  + ``lighten(color, percentage)`` takes a color and light this color by the given percentage. As you can see in the comment the resulted color is ``#222``
  
  + ``#000`` is the shortcut for ``#000000``
  
  + ``!default``: can be translated with an if:
  ```
    /**
     *  if the color $gray-darker does not exists
     *  set it to lighten(...)
     *  else let the value already assigned
     */
    if not (exists($gray-darker) {
      ``$gray-darker: lighten(#000, 13.5%) !default; // #222`
    }
  ```

