---
layout: post
title: "html: meta tags"
categories: html
table of content: <a href="../README.md">index</a>
---

####[HTML](#html)
====

####[Meta tags](#meta-tags)

####[How to make an html document?](#how-to-make-a-html-document-?)
-----

To make an html document, simply make a file with the extension ``.html``
That will tell the browser that the file should be interpreted as html.

####[Meta-tag](#Meta-tag)
----

However, we need to give him additional information:

  + The _version_ of html we're using : It's currently HTML5.
    This will be important for the future

  + The _title_ of the document : So it can be displayed in the browser window:
    ```
      <title>title of the document</title>
    ```

    ![window browser title](../assets/images/html__metatag--browsertitle.jpg)

  + A _favicon_ which is an icon (a little image) that be displayed in the browser window:
    ```
      <link rel="icon" type="image/x-icon" href="../assets/images/favicon.ico"/>
    ```
    ![favicon](../assets/images/html__metatag--favicon.jpg)

  + The _character encoding_: to be sure that character we type will be well interpreted,
    we need a character encoding. The international norm is ``utf-8``.
    As an example, if we don't use a character encoding, the text ``éèô`` will appears like ``Ã©Ã¨Ã´``.

  + The _description_: Description of the website, usefull for Search Engines like Google.
    SEO (Search Engin Optimization) is a big domain, and there's even job specialized in it.
    It's basically displaying content, adding specified keywords, and use some tricks, to have the best results
    in Searcg Engine (mostly google)

  + The _viewport_: A pixel is a little square on the monitor of your computer.

    Actually, there are millions of squares on yr monitor, and by adjustment of your pc, they display
    what you actually see on your monitor.

    When pluging-in your monitor to your computer, the computer will know how many pixels your monitor have.
    The computer will adjust your monitor and then display anything.

    On mobile browsers, some monitors are lying. It results in a bad adjustment of your website.

    To fix this, the viewport have been created. It helps adjusting the display of your website on mobile.


