---
layout: post
title: "sass: manipulating data"
categories: sass
table of content: <a href="../README.md">index</a>
---

####[Sass](#sass)

####[Introduction](#sass-introduction)

Storing data is a cool thing, but what about manipulating it?

The more basic manipulation is to change the value of a data stored in
a variable :

```
  /**
   *  @property {Hexadecimal} $red-secundary secundary color
   */
  $red-secundary: #ff2200;

  /**
   *  Change the nuance of red secundary color
   */
  $red-secundary: #ff6600;

```

And now we have a more orange-red as a secundary red color.

We can also do mathematicals operations (add, subsitute, multiply, divide).
Example:

```
  /**
   *  @property {Integer} $adder - variable to do the math operation on
   */
  $adder = 1;

  /**
   *  Add 1 to $adder.
   *  In informatics, adding an integer (a whole number) is called
   *  incrementing.
   *  In this case, we __increments $adder by 1__
   *
   *  @property {Integer} $adder - variable to do the math operation on
   *  @return {Integer} $adder - the variable vis now equals to 2
   */
   $adder = $adder + 1;
```


####[Conditions](#sass-conditions)

We can put conditions on a variable. That mean that we can change a variable
depending on its value.

```
  /**
   *  @property {Hexadecimal} $red-secundary - secundary color
   */
  $blue-primary: #0066ff;

  /**
   *  In the condition that $blue-secundary equals
   *  to #0066ff, change it to #0088ff
   *
   *  @property {Hexadecimal} $blue-secundary - secundary color
   *  @return {Hexadecimal} $blue-secundary - new blue color
   */
  if ($blue-secundary == #0066ff) {
    $blue-secundary = #0088ff;
  }
```

####[Explanations of the if condition](#sass-explanations-if)

__if__ $blue-secundary is equals to (``==``)  the value "#0066ff" 
then do the instruction (``{``) :
store ``#0088ff`` variable in ``$blue-secundary`` and
end the instruction (``}``)

Obviously, this condition will always be met, since we declare (store the data in)
the ``$blue-secundary`` variable.

####[Loops](#sass-loops)

Now, what if we could change the variable over time?

This variable would take different value depending
on the given time ``t``.

Let's say we have a variable ``$counter`` that will add 1 to itself
over time like so :

```
  $counter = $counter + 1
```

To make a variable incrementing over time, we will use a __loop__:

```
  /*
   *  Increments the counter by 1 until $counter is
   *  equals to 200
   *
   *  @property {Hexadecimal} $counter - incrementing variable
   */
  for ($counter = 1; $counter < 200; $counter++) {

  }
```

####[Explanations of the for loop](#sass-explanations-for)

__For__ is the word to begin the loop,
it takes three parameters :

  + An __assignment__ of the counter variable. An assignment is the algorithmic way to say
    "I store the value in the variable": ``$counter = 1``

  + A __condition__: it works like __if__ condition, excepted it's reversed.
    It will do the instructions of the for loop __unless__ the condition is met:
    ``$counter < 200 ``

  + A __incrementation__: We add 1 to counter. the ``++`` expression is a shortcut to say
    ``add 1 to the current variable``.
    Since in many loops, there will be a lot of incrementing just by 1.
    It's better to know this shortcut.
    so we could have wrote ``$counter + 1`` as ``$counter++``.
    The loop will assign this incrementation to the current counter, so you don't need
    to write ``$counter = $counter + 1``.

The for loop will repeat itself unless the condition is met.
So ``counter`` equals 1, __the instructions will be run__.

Once the instruction are finished (expressed by ``}``), the __computer will back to the first line
of the for loop__, check if the condition ``$counter < 200 `` is met, then increments the variable ``$counter``
by one ``$counter++``. Then the __instruction are runned again, and again until the condition is met__.

When the condition ``$counter < 200 `` (that is ``$counter == 200``, $counter equals 200) is met, 
the __for__ loop will stop running.
