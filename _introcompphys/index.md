---
layout: post 
title: Introduction to Computational Physics
init_date: 19 Nov 2020
author: jph
---

Welcome to my introductory "course" (notes) on computational physics! This is my first attempt at writing such a "course," so it might not be as complete as it should be. Please do not hesitate to email me about mistakes or something that is not entirely clear. The syllabus and appropriate links are below. 

In this course, I will be focusing on scientific computing methods useful for physicists (which by extension should be useful to other quantitative science fields). I will start with an introduction to one of the easiest languages out there to learn: Python (which is still very powerful and extremely popular!). Next, by considering topics of interest for physicists, you will learn techniques for solving problems computationally, culminating in the solution of partial differential equations. 

I will deviate slightly from the typical presentation of a "computational physics" course by emphasising details usually seen in a computer science class, such as modularity and good coding practices, as well as error and run-time analysis. While these topics might not be the most interesting to physicists, I think they are very important to learn early on. I will try to integrate them into the greater framework of the course to make learning them not so mind-numbing. That said, I will not go so much in detail as would be done in a computer science (or worse yet, maths) course. 

# SYLLABUS FOR INTRODUCTION TO COMPUTATIONAL PHYSICS "COURSE"

Main sources/references (all worth checking out!):
- _A First Course in Numerical Methods_ by Uri M Ascher and Chen Greif.
- _Computational Physics_ by Mark Newman.
- _Computational Physics_ by Steven E Koonin and Dawn C. Meredith.
- [PHY407 lecture notes on github](https://github.com/PHY407-UofT/lectures-2020), by Nicolas Grisouard. 
    - I do not have any connection with the course, I just like his notes. 
- [CPSC303 lecture notes, by Jessica Bosch](https://www.cs.ubc.ca/~jbosch/courses/2016-17/CPSC303/schedule/index.html). 
    - I personally took this course, and can say the notes are a very nice distillation of the textbook that gets all the important bits. However, most of the material is not really so interesting/useful for pure physics students (if you're interested in details about different techniques and error analysis, it is worth a look). 
- _Computational Physics_ by Jos Thijssen. 
    - This textbook is _much_ more advanced than the presentation I am going for. However, it is my favourite textbook on the topic and it has some very interesting problems, so I will be taking some ideas from there, mostly in the later sections of the course. 
- My noggin, mostly stuff from my undergraduate computer science studies (disclaimer: I only did a _Minor_ in computer science!). 

[Introduction](intro)

## TODO coming soon (everything below!)

Introduction
- Why do we care? 
    - Why do we solve things on a computer? 
    - It's interesting! (I hope...)
    - It could get you a job
- What will we learn? 
    - How to code, particularly in Python (but the concepts are more general!)
    - How to solve interesting physics problems ("the physicist's survival toolbox")
    - How numerical methods work, and how they are derived
    - Error and runtime analysis
    - Good coding practices (modularity, version control)
        - Heads up: I think this is something very important often neglected in programming-for-scientists courses, so there will be a lot more of this than you will find elsewhere! The start might seem a little slow because of it, but I believe it is worth it. I will try to make the introduction of these topics not too overwhelming, and hope the readers learn it as we go along, as I use these topics throughout. 
    - How to make your code a little more efficient (towards the end)
    - This is catered to physicists, but I think it might benefit anyone who wants to learn how to solve physical problems on a computer. I am doing a PhD in computational quantum chemistry. This material is the backbone of what I do. This "course" should be useful for budding physics, chemists, computer scientists (interested in numerics), and mathematicians alike. 
- Why Python? 
    - It's (very) popular
    - Easy to learn, etc. Contrast to FORTRAN and C++, compare to Matlab and Julia
    - Python can do anything, easily (see XKCD comic)
- Brief discussion on installation, IDEs, etc.
    - Software like VSCode makes git a lot easier imo

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

Improving your code, parallellisation (Numba)

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
