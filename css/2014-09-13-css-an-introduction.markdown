---
layout: post
title: "css: an introduction"
comments: true
categories: css
table of content: <a href="../README.md">index</a>
---

####[CSS](#css)
====

####[Introduction](#introduction)

HTML is a way to format text.
But what if we want to add colors and others fancy stuff?


####[ The old and deprecated way](#old-and-deprecated-way)

  + The very _old, deprecated way_, is to add a __property__ to a tag 
    that will add the so-call tag some fancyness.

    ```
      <p><font color="red">This is some text!</font></p>
    ```

    would result as:

    Result : http://jsfiddle.net/6dr78545/ 

    But it won't. The current version of HTML (HTML5) does not support this
    feature. Instead, you will see:

    <p>My text in red</p>
    
    =======

    It was used when CSS was not created yet (<1996) and should _never_ be used.
    Nobody uses that anymore, it just for your information and/or the very rare case
    you meet it.

####[CSS](#into-css)

CSS (Cascading Style Sheets) is a langage that permits to add colors, and many more
things to a formatted text.

let's take a look at this code:

```
  <p>
    i am a paragraph
  </p>
```

We want to color the text of this paragraph in purple, with CSS.
You can do CSS in 3 ways:

####[Inline CSS](#inline-css)

Directly in the ``<p>`` :
  ```
    <p style="color:purple;">
      i am a paragraph
    </p>
  ```

We __attach__ a CSS style to a paragraph with the __property__ style.
Then we do CSS: We assign ``purple`` __value__ to ``color`` __property__.

A __CSS property__ is a command which tell the tag what it should modify.

A __CSS value__ is a data that will be on set the CSS property.

__Example:__

> I want to add a yellow background on the ``<p>`` tag:

  ```
    <p style="background-color:yellow;">
      i am a paragraph
    </p>
  ```
result: [jsfiddle]

> I want to add space between lines in the ``<p>`` tag:

  ```
    <p style="line-height:200%">
      i am a paragraph
    </p>
  ```

result: [jsfiddle]

####[How much CSS do I have to learn](#how-much-css)

Like HTML, there is tons of tags in CSS, and there is a reference : [w3c/css](http://www.w3.org/Style/CSS).
The CSS Spec is even bigger than the HTML one.
I don't event know every CSS tags.

Like HTML, it wil comes with practise.
