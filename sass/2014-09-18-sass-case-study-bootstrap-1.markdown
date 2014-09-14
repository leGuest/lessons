---
layout: post
title: "sass: case study - bootstrap - part 1"
categories: sass
table of content: <a href="../README.md">index</a>
---

####[Sass](#sass)

####[What is bootstrap?](#sass-what-is-bootstrap-?)

[Bootstrap](http://getbootstrap.com), from [twitter](https://www.twitter.com), is a popular css framework written in less
and sass.

It have a set of already stored data, and instruction that you can use to make your own UI.

Let's take an example, in ``bootstrap/_variables.scss``,
[from line 21 to line 25](https://github.com/twbs/bootstrap-sass/blob/master/assets/stylesheets/bootstrap/_variables.scss#L21):

```
  $brand-primary:         #428bca !default;
  $brand-success:         #5cb85c !default;
  $brand-info:            #5bc0de !default;
  $brand-warning:         #f0ad4e !default;
  $brand-danger:          #d9534f !default;
```

These variables are used to store the notifications color:

  + if it's a success action, then it's a green nuanced color  - ``$brand-success``,

  + if it's an information, then it's a blue nuanced color - ``$brand-info``,

  + etc

If we want to do a paragraph to inform a success action with ``$brand-success``,
in ``utils/notifications.sass``:

```
  /**
   *  import the variables file
   */
   @import "bootstrap/_variables.scss"


  /**
   *  Make a paragraph notificiation when successfull
   */
   p.success{
    color: $brand-success
   }
```

Result: [jsfiddle](http://jsfiddle.net/xpoyoz5f/)
