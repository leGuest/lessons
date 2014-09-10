---
layout: post
title: "html: tag exception"
date: 2014-09-10 18:11:00 +0200
comments: true
categories: html
---

HTML
====

Autoclose tag
----

In the [previous lesson](previous_lesson), we talk about __tag rules__:


> So you can see that to __open a tag__, you use ``<tag name>`` and to __close a tag__ :  ``</tag name>``.
> This is the the same rule for almost all html tags.

In fact, __every tag need to be closed__.

But some tags dont have content in it.
For example, ``<br>`` is a tag to make a new line.

You can see it as :

  * I want a new line : ``<br>``
  * I want to stop new line: ``</br>``

----

So as an example:

```
  this is my first line <br></br>
  this is my secund line
```

For this kind of tags, there's is a __shortcut__:  ``<br/>``.

This will tell the browser to __open and close a tag at the same time__.

So when a tag have no content inside, it's better to use this shortcut :

``<tag name/>``

instead of:

``<tag name></tagname>``.


Tags like this are called __autoclose tags__.

Exercice
----
_With the ``<br>`` autoclose tag, make this in html :_

Favorite Books
<br/>
<br/>
<br/>
- Pride and prejudige!
<br/>
<br/>
<br/>
- Last night of love,
<br/>
<br/>
<br/>
- The first night of the war !

Soluce: https://jsfiddle.com/rt3b86e4/
