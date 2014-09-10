---
layout: post
title: "html: meta tags"
categories: html
table of content: <a href="../README.md">index</a>
---

####[HTML](#html)
====

####[Structure of a html document](#structure-of-a-html-document)

First, we need to tell the browser the version of html we using.
We will use the last version (5):

_Note_ : this is the only tag that does not need auto-close.
```
<!doctype html>
```

Then, we need to group all the html page under a ``<html>`` tag, to
tell the browser that what we're coding inside is html.

```
<html></html>
```

Then comes the [meta-tags](./2014-09-13-html-meta-tags.markdown).
They are grouped under the ``<head>`` tag :

```
<head>
  <title>title of the document</title>
  <link rel="icon" type="image/x-icon" href="../assets/images/favicon.ico"/>
  <meta-charset="utf-8"/>
  <meta name="description" content="website lessons"/>
  <meta name="viewport" content="width=device-width, initial-scale=1"/>
</head>
```

Finally, the content of the document:

```
<body>
  <b>my bolded text</b>
  <br/>
  <ul>
    <li>learn html</li>
    <li>learn css</li>
    <li>learn js</li>
    <li>learn how backend and backend langages works</li>
    <li>learn how to setup a server</li>
    <li>learn how database works</li>
    <li>make something with all this</li>
  </ul>
</body>
```

And what the whole html page looks like:

```
<!doctype html>
<head>
  <title>title of the document</title>
  <link rel="icon" type="image/x-icon" href="../assets/images/favicon.ico"/>
  <meta-charset="utf-8"/>
  <meta name="description" content="website lessons"/>
  <meta name="viewport" content="width=device-width, initial-scale=1"/>
</head>
<body>
  <b>my bolded text</b>
  <br/>
  <ul>
    <li>learn html</li>
    <li>learn css</li>
    <li>learn js</li>
    <li>learn how backend and backend langages works</li>
    <li>learn how to setup a server</li>
    <li>learn how database works</li>
    <li>make something with all this</li>
  </ul>
</body>
```
