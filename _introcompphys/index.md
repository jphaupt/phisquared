---
layout: post 
title: Introduction to Computational Physics
init_date: 19 Nov 2020
author: jph
---

Welcome to my introductory "course" (notes) on computational physics! This is my first attempt at writing such a "course," so it might not be as complete as it should be. Please do not hesitate to email me about mistakes or something that is not entirely clear. The syllabus and appropriate links are below. 

In this course, I will be focusing on scientific computing methods useful for physicists (which by extension should be useful to other quantitative science fields). I will start with an introduction to one of the easiest languages out there to learn: Python (which is still very powerful and extremely popular!). Next, by considering topics of interest for physicists, you will learn techniques for solving problems computationally, culminating in the solution of partial differential equations. I will try to present different subfields, but as I am just doing this in my spare time chances are I will mostly be presenting problems from my own field or of interest specifically to me. 

I will deviate slightly from the typical presentation of a "computational physics" course by emphasising details usually seen in a computer science class, such as modularity and good coding practices, as well as error and run-time analysis. While these topics might not be the most interesting to physicists, I think they are very important to learn early on. I will try to integrate them into the greater framework of the course to make learning them not so mind-numbing. That said, I will not go so much in detail as would be done in a computer science (or worse yet, maths) course. 

Elementary knowledge of calculus (up to Taylor series) and some knowledge of linear algebra is assumed, though you might be able to study these in parallel. Knowledge of physics is not necessary but beneficial, at least for understanding motivations and examples. 

My goal is to be informal and pragmatic. 

# SYLLABUS FOR INTRODUCTION TO COMPUTATIONAL PHYSICS "COURSE"

Main sources/references (all worth checking out!):
- _A First Course in Numerical Methods_ by Uri M Ascher and Chen Greif.
    - Fairly straightforward textbook focused on the more mathematical side of things. 
- _Computational Physics_ by Mark Newman.
    - I would describe this book as introductory. It goes in more depth on mostly the same topics as I am covering, so it is probably the best supplementary text. 
- _Computational Physics_ by Steven E Koonin and Dawn C. Meredith.
    - I would describe this book as intermediate in difficulty. Certainly nice to check out; I especially like the format involving projects. 
- [PHY407 lecture notes on github](https://github.com/PHY407-UofT/lectures-2020), by Nicolas Grisouard. 
    - I do not have any connection with the course, I just like his notes. 
- [CPSC303 lecture notes, by Jessica Bosch](https://www.cs.ubc.ca/~jbosch/courses/2016-17/CPSC303/schedule/index.html). 
    - I personally took this course, and can say the notes are a very nice distillation of the Ascher and Greif textbook that gets all the important bits. However, most of the material probably won't be so interesting/useful for physics students (if you're interested in details about different techniques and error analysis, it is worth a look). 
- _Computational Physics_ by Jos Thijssen. 
    - This textbook is _much_ more advanced than the presentation I am going for. However, it is probably my favourite textbook on the topic and it has some very interesting problems, so I will be taking some ideas from there, mostly in the later sections of the course. Definitely worth a read if you find the material here interesting. 
- My noggin, mostly stuff from my undergraduate computer science studies (disclaimer: I only did a _Minor_ in computer science!). 

## Lessons
[Introduction](intro)

Introduction to Scientific Computing 
- [Introduction to Programming with Python](sec1_1) 
- [Introduction to Numerics](sec1_2) TODO case study with linear regression
- [Good Programming Habits](sec1_3)
- [Tutorial](sec1_tut) TODO data fit to nuclear decay? Bonus: why is the exponential not sufficient? 

## TODO coming soon (everything below!)

Introduction to Python 
- Basics, as well as some packages like numpy and matplotlib

Introduction to Programming and Numerics 
- catastrophic cancellation error, other error analysis
- also introduce basic not-so-important methods like interpolation
    - use as an entry point into modularity and git, proper Python documentation
- first application: least squares
- TDD
    - try to encourage good practice throughout the rest of the "course" as well 

Root finding 
- use as a basic starting place for error and runtime analysis
- conditioning

Derivatives 

Integrals

ODES 
- some interesting applications, like 

PDEs (application to fluid dynamics/Navier-Stokes)

Improving your code, parallelisation (Numba)

Extra topics
- Monte Carlo (do classical, but mention QMC)
    - be sure to mention setting a seed for testing purposes!
    - application to the Ising model
- some matrix algebra, eigenvalue problem (mostly just introduce packages)
- non-technical overview of machine learning in physics 
    - some optimisation?
    - knowing Python sets you right up for this
    - neural networks, gaussian processes
    - really nice for experimentalists
- symbolic computing (sympy)
- link to more advanced course (focused on condensed matter and chemistry)
- what next? (mention algorithms and data structures books, not directly useful for physicists but the ideas could be useful). I plan on doing an intro to algorithms course some time anyway, though it's not high on my list.