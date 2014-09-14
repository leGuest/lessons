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

---
file: variables.scss
location: <a href="#">./bootstrap/_variables.scss</a>
imported from: <a href="#">_bootstrap.scss</a>
---
