---
layout: lecture
title: Introduction
author: jph
init_date: 19 Nov 2020
---

## So what's all the fuss about?
When I was just starting my undergraduate physics and mathematics degree, I didn't really "believe in" computational physics. That is, I considered "real" physics to be the pen-and-paper hard-maths techniques found in old theory papers, or how (elementary) physics is often presented in textbooks and media. If you didn't find a general analytical expression that can predict any case, you're not really doing physics.[^1] Perhaps you are like this as well.

Nowadays, computational methods in physics are not only increasingly indispensible and unavoidable for both theorists and experimentalists alike, it is also growing to be its own field (kind of in between theory and experiment). For example, many-body theorists use advanced computational techniques, such as [density functional theory](https://en.wikipedia.org/wiki/Density_functional_theory), to study the structure of solids and other condensed systems. Experimental particle physicists often use machine learning models to quickly, and more efficiently than can ever be done by a human, screen data and detect particles of interest in their experiments. To emphasise how computation not only changed theory and experiment for good, but is also budding into its own field, the development of the aforementioned density functional theory won Walter Kohn and Lu Jeu Sham the 1998 Nobel prize in chemistry.[^2]

Hence, not only is it vital for any physicist to learn the fundamentals of computational methods (in much the same way as it is necessary for them to learn the fundamentals of calculus), it is a legitimate field of research in and of itself (in much the same way as mathematical physics is its own field).

## Okay, but what will you teach me?
It would be impossible for anyone to summarise all of computational physics (or numerical analysis) in one course. It is a huge and constantly growing field. However, I will focus on what I consider the most important building blocks to make you a successful scientific programmer.

In the course homepage, you can see the list of topics to be explored. I will start with the basics on how to code, move on to the basics of how to solve physics problems (and in so doing develop a "physicist's survival toolbox"), some basics of how numerical methods work and how they are derived, along with some analysis of their error and runtime. I'll also discuss good coding practices, which I think is something often neglected in programming-for-scientists courses. The start may be a little slow because of it, but I think it is worth learning early in your career. I will try to make the introduction of these topics not too overwhelming, and hope the readers learn it as we go along, as I use these topics throughout. Finally, I hope to cover how to make your code a little more efficient, and some parallel programming.

This is catered to physicists, but I think it might benefit anyone who wants to learn how to solve physical problems on a computer. I am doing a PhD in computational quantum chemistry. This material is the backbone of what I do. This "course," I hope, should be useful for budding physics, chemists, computer scientists (interested in numerics), and mathematicians alike.

In exploring these topics, I will be using Python, but the presentation will be reasonably language agnostic.

## All the cool kids use C++; why do you use Python?
There are a couple of reasons to use Python. First, it is easy to learn and easy to implement, allowing you to set up your solution faster than most other languages. It doesn't require you to worry about messy details like memory access, [and many advanced functions are already done for you](https://xkcd.com/353/) (you just call a library originally written in a faster language). For most people this is usually good enough.

Another nice thing about Python is that it is very popular with lots of support. It is also general purpose, which means that if you like you can easily use it to make programs unrelated to physics (there's _a lot_ more to programming than solving physics problems; perhaps these might interest you: Python is great for other applications, too!). This also means that it probably has a higher employability than many other languages. It is also the _de facto_ language for applied machine learning (though I suspect this may change), and is usually used for interacting with databases, which is becoming increasingly relevant for many fields.

Languages like C++ and Fortran are very fast, but also quite a bit harder to learn (and Fortran in particular is not very popular outside high performance computing). These two languages are very useful to learn if you want to do method development or high performance computing. Because of their steeper learning curves, and because most physicists won't need their high performance (and if you are an inexperienced programmer, you might not even see much of a performance boost), I do not think they are appropriate first languages. That said, if you find yourself working in a group that develops high-performance software (like I do), then you will almost definitely need to learn one (or both) of these.

Another language worth looking at in my opinion is Julia, but it is young and not particularly popular. However, it is on the rise, it is very fast, and has syntax similar to Matlab (making it easy to code in). It doesn't have nearly as much support as other languages, and it is more focused on numerics (like Fortran), though. While I really like Julia, for these reasons I do not think it's a great first language. That said, if you already know Python or if you're confident you're going to work with numerics 95% of the time then I would encourage you to try to follow along with Julia!

I will explicitly use Python code, but I hope to present it in a way that it's perfectly possible to follow along in another language if you prefer.

## Resources
In the main page you will see a list of sources/references. These are nice if you want to learn more or if what I wrote doesn't make sense.

To install Python, I recommend using an [Anaconda](https://docs.anaconda.com/anaconda/install/) installation.

To code, you could just use any text editor (notepad, gedit, vim, emacs, etc) and a terminal, but it would probably be easier if you use a simple IDE like [Spyder](https://www.spyder-ide.org/) (which comes with Anaconda). I also really like [Visual Studio Code](https://code.visualstudio.com/), though it requires more configuring as it is more general purpose.[^3]

Some IDEs also make good practices like documentation and version control easier. Speaking of version control, use of [Github](https://github.com/) is also generally helpful (though not necessary).

<hr>

[Next Lesson](sec1_1)

<hr>

[^1]: I would now argue that experimentalists are the only ones doing "real" science; I just happen to find theory/computation more interesting. That said, "real" is not well defined here.
[^2]: Interestingly, both Kohn and Sham were trained as physicists.
[^3]: I am actually using Visual Studio Code to help write this website.