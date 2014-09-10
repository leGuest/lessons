---
layout: post
title: "html: good practises part 2"
date: 2014-09-10 18:11:00 +0200
comments: true
categories: html
---

HTML
====

good practises part 2
----
#### What are good practises in general?

There's a lot of good practises.
I will only cover the basic parts of it.

#### Indent

Basically you won't write like this:

```
<p> <b>Meaning of life</b><br/> Be surrounded by people who makes u happy.<br/> People who makes u laugh, which helps you when u need it.<br/> People who will never take advantage of u.<br/> People who always care.<br/> They are the Ones who deserves to Keep them into ur life<br/> The others are just passing by.<br/> Do not get where the path may lead,<br/> go instead where there is no path and leave a trail. </p>
```

This is not readable.
Put lines instead to make it more readable.

```
<p>
<b>Meaning of life</b><br/>
Be surrounded by people who makes u happy.<br/>
People who makes u laugh, which helps you when u need it.<br/>
People who will never take advantage of u.<br/>
People who always care.<br/>
They are the Ones who deserves to Keep them into ur life<br/>
The others are just passing by.<br/>
Do not get where the path may lead,<br/>
go instead where there is no path and leave a trail.
</p>
```

To improve this readibility further, you can use code indenting:

```
<p>
  <b> Meaning of life</b><br/>
  Be surrounded by people who makes u happy.<br/>
  People who makes u laugh, which helps you when u need it.<br/>
  People who will never take advantage of u.<br/>
  People who always care.<br/>
  They are the Ones who deserves to Keep them into ur life<br/>
  The others are just passing by.<br/>
  Do not get where the path may lead,<br/>
  go instead where there is no path and leave a trail.
</p>
```

Here I have indent each line by one tab below the ``<p>`` tag and 
until the end of it ``</p>``, make it more readable.

When and where to indent comes with practise.
Code, read what you coded, and ask yourself if it's readable.
If it's readable, then let it. If not try to indent in a
better way.

As an example, the indented code of the example before is indented.
Yet I am not sure it's very readable. It appears for me as a big 
block, so:

```
<p>
  <b>
    Meaning of life
  </b>
  <br/>
    Be surrounded by people who makes u happy.
  <br/>
    People who makes u laugh,
    which helps you when u need it.
  <br/>
    People who will never take advantage of u.
  <br/>
    People who always care.
  <br/>
    They are the Ones who deserves to Keep them into ur life
  <br/>
    The others are just passing by.
  <br/>
    Do not get where the path may lead,
  <br/>
    go instead where there is no path and leave a trail.
</p>
```

#### Exercice

_Make this text readable:_

  * You can also format the text using tags, check previous lessons to see
  some of them.

  * Indent is always perfectible. To know when to stop indenting, just read your code
  and ask yourself "Is it readable?". If it is, stop here, you're done.

  * Dont pass too much time on indenting. If you pass more than 15 minutes on this, stop
  where you are.

```
Turn Ons/Off:
turn on well no one can turn me on turn off everyone(liars, cheaters, people who think i
am playing with i am not, and if u think u can trick me well u dont!)...most are doing a
good job. Some people confuse freedom of expression, with the right to eat SHIT! Dont talk
to me because your bored,or some other girl told u to go away, dont come to me only when
you nedd a favor.I dont like being used.
```

_soluce_ : http://jsfiddle.net/6orcf637/

### Good practises in HTML

#### Deprecated tags

HTML is kind of old (30 years old or so) and web development is always changing.

Web development is all programing that turn around the web.
Basically, website, but also webapp, mails, some servers, etc...
Just to give you an approxmative idea on how the web is changing, a website
which have 6 years is old, and a 10 years old one is an ancester.

Since the HTML is old, some tag who was used before are not longer used.
Yet they reminds in the langage, to permits old website to still work.

As an example of deprecated tag:

```
<b>my scrolling text</b>
```

will result of:

<b>my scrolling text</b>

Why ``<b>`` is deprecated : http://stackoverflow.com/a/271776

