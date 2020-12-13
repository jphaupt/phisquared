---
layout: lecture
title: Introduction to Programming with Python
author: jph
init_date: 24 Nov 2020
---

There are _a lot_ of resources for Python out there. Simply search the web for "introduction to python" or "numpy" or "python for physicists" or similar. Because of this, I'll keep this section brief so that you may refer to it quickly when just starting. 

Here, as in the remainder of the course, I assume you have Python 3 installed along with packages from Anaconda (in particular, numpy, matplotlib, and scipy).

## My First Program

Let's start with the most typical first program written when learning a new language: simply outputting a string to the console. This is a common way to introduce a language's basic syntax, and is often called a ["Hello, World" program](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program). Save the following to a file with a `.py` extension (let's call it `hello.py`). 
```python 
print("Hello, World!")
```
You can run this by entering `python hello.py` (or whatever you called it) into a console (terminal), and you should get the output `Hello, World!` (if you are using an IDE, you can just press the run button to see the same result). 

Just for comparison, here is the same program written in Java (my first programming language). 

```java 
class hello{
    public static void main(String[] args) {
        System.out.println("Hello, World!"); 
    }
}
``` 

Again, here's the same program but in C++. 

```cpp
#include<iostream>
int main() {
   std::cout << "Hello, World!" << std::endl;
}
```

As you can see, Python stands out by being the simplest. In most other languages there are extra expressions as seen above that may seem arcane to a newcomer, but in Python it is straightforward. You take the built-in function `print` (which prints to console) and you input a _string_ (text, in quotation marks) to have the program _print_ the _string_ (in this case, "Hello, World") to the console. Much like in maths, a function (call it $f$, or `print`) is evaluated at a value (call it $a$ or `"Hello, World!"`) using parentheses as notation ($f(a)$, or `print("Hello, World!")`). 

And voilà, you have written your first program! Nifty, but not very useful. 

## Basic Operations in Python 

Python comes equipped with basic mathematical operations, like addition and subtraction, so if you want to work out what's 4+3, and then print it to screen, you can write `print(4+3)` and the output `7` will be printed to console. Similarly, you do subtraction `-`, multiplication `*`, and division `/`. Exponentiation is done with the `**` symbol, so $3^2$ is `3**2` (note, this is nonstandard notation). 

Another very important operation is _assignment_, for which we use the equals sign `=`. For this, we also need to introduce variables. We can define a variable, say `x` by the line `x=3` (sets the _variable_ `x` to 3). Note, however, that `x` is not fixed and we can later write `x=10` for example. Furthermore, we can do such operations like `x=x-2` meaning "subtract 2 from `x`" (there is also the shorthand `x-=2`). 

We are not just restricted to integers, however. We could just as easily have said `x=3.3` (a float) or even `x=True` (a _boolean_, either `True` or `False`). Some boolean operations you might recognise from logic are `and`, `or`, and `not` which do what you would expect (`True and False` evaluates to `True`, but `True or False` evaluates to `False` etc). You can also get a boolean from numbers by equality `==`, e.g. if you set `x=3` earlier then `x==3` evaluates to `True`, but `x==3.3` to `False`. (A shorthand for `not equals` is `!=`). 

Some other useful constructs are `if` statements and `for` loops. Both of these 

TODO the above 

TODO defining functions

TODO come back to this... Pretty boring to write about

## Linear Algebra in Python 

TODO important packages for scientists

TODO introduce things you _could_ do, then say just use numpy!

## Plotting in Python 

TODO introduce Matplotlib

<hr>

[Previous Lesson](intro)

[Next Lesson](sec1_2)

<hr> 
