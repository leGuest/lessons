---
layout: post
title: "html: an introduction"
categories: html
---

####[HTML](#html)
====

####[Introduction](#html__introduction)


__HTML__ (Hyper Text Markup Langage) is a language that permits to format a content in the browser.
You can see it as a __text file with extended functionality__.

A browser is an internet naviguator (firefox, chrome, IE, etc are browsers).

If you try to read a text file (myfile.txt for example) within a browser, it will just __display raw text__. More than that, the browser won't even __understand when u put a new line__ : 
The browser will go at a new line when it can't see new space to insert the new word.

####[Create a tag](#html__introduction--createatag)



__HTML__ have a set of instruction to control the behavior of text, called __tags__.
Tags are __signs that will transforms the text in the format you want__.

There's lots of __tags__ : 

  *	You want the text bold? use ``<b>text``
  *	You want the text in italic? use ``<i>text``
  *	You want a text as a paragraph? use ``<p>text``
  *	and so on.

  ----

####[Close a tag](#html__introduction--closeatag)

However , if you do 
```
  <b> bolded text <i>italic text
```

the browser will show you "___italic text___". 
But you wanted the italic text to be only "italic", and not "bold and italic". 

That happens because the browser **don't know when to stop to bold text**, so the browser says "well, let's just bold the text until the end of document". 

It's why you need to tell him where to stop using a specific tag (here ``<b>``, bold). **You need to close the tag.**
In the case of ``<b>``, the __instruction to close it is__ ``</b>``. 

Take the example back, this is how you want to use it : 
```
<b>bolded text</b><i>italic text
```

---

So ``<b>`` to open a tag, ``</b>`` to close it. 

----

_What about_ ``<i>`` (italic)? 
To close it, use ``</i>``

```
<b>bolded text</b><i>italic text</i>
```

So you can see that to __open a tag__, you use ``<tag name>`` and to __close a tag__ :  ``</tag name>``.
This is the the same rule for almost all html tags.

####[Exercice](#html__introduction--exercice)


----

_Given:_

  * ``<u>`` is the tag for underline (<u>underline text</u>), 
  * ``<s>`` for stroke (<s> stroke text</s>), 
  *  ``<p>`` for paragraph text 

_Make this in HTML :_ 
<p>
	My name is Dyana. I am a <s>troll</s> lady.
</p>
<p>
	 I'm <u>selfish</u>, <u>impatient</u> and a <u>little insecure</u>. I make <s>always the righ thing</s><u>mistakes</u>, I am <s>temperated</s><u>out of control</u> and at times <s>easy peasy</s> <u>hard to handle</u>. But if you can't handle me at my worst, then you sure as hell don't deserve me at my best. 
</p>

_Soluce_ : http://jsfiddle.net/g0pzebnx/
