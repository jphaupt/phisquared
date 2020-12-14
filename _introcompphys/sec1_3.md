---
layout: lecture
title: Best Coding Practices
author: jph
init_date: 13 Dec 2020
---

It is my experience that many physicists, as well as other scientists and engineers are often bad programmers. Often, they can write programs (sometimes even rather complicated ones) and have them run and solve a problem of interest, but they do not properly document or modularise their code. This is not usually a problem with small code snippets that you write once and never think about again, but that is rarely ever the case. 

Scientific software can be large, complicated, and subtle. If you want to share your code with collaborators, or look at it a few months down the line and your code does not follow decent coding practices, you are likely to get someone very frustrated. Perfect, fast code that no one can understand is not nearly as good as slower not-quite-there code with excellent documentation, modularity, with thorough testing. You are likely to recall old code, especially if in the context of a larger project, or build on it later. These things are difficult to predict. 

In section I shall briefly outline some of the most important coding practices, which will help you organise your work, and systemically approach tasks, in addition to having your code legible by not just yourself but other people. 

At first, many of these techniques may seem like a painful waste of time, but as your code gets more complex being familiar with these will become invaluable. Not only will you be able to write more reliable, understandable code, but chances are you will also be able to code faster and will run into fewer road bumps. Future you will be thankful for learning this. 

## Pseudocode 

To start, it is generally advisable to first solve your problem in _pseudocode_. As you gain more experience programming, you may no longer find it so helpful to use for small tasks, but I think it is a good habit to get into early on. 

Pseudocode doesn't have an exact definition, but it is essentially a description of your algorithm in plain English (i.e. not a programming language). Pseudocode is typically quite personalised (and not always consistent), and that's okay as long as your pseudocode is legible to someone who speaks English (but not necessarily, for example, Python). 

Pseudocode is basically the "blueprint" for the code you will be writing later, and I would recommend using pseudocode before starting any code. Keep it concise, logical (i.e. keep reasonable variable names) and systematic. Once done, keep a copy with you as you start your code. 

For example, if I have a file with a list of numbers $\bm x:=(x_1,...,x_N)^T$ and I want to calculate the alternating sum of all these numbers 
$\\sum\_{j=1}^{N}(-1)^{j-1}x\_j$, 
I may write pseudocode like 
```
LET x <- READ input file
LET N <- length(x) 
LET sum <- 0
FOR j=1 to N 
DO 
    add (-1)^(j-1) x_j to sum
END DO
return sum
```

## Documentation 

Perhaps the most important "best practice" is proper documentation. You should always try to document work, even if you are in a rush. Bad documentation is better than no documentation. Sometimes even the most unlikely pieces of code can end up being reused, and if it is obscure and poorly documented, you're going to have a rough time, so try to have at least a little bit of documentation. 

Some approaches: 
- "Self-documenting" code. By this, I mean writing the code itself (not comments) clearly. This means write logical variable names (e.g. `num_atoms` is probably a better variable name that `x`) and present the solution in a way that is easy to understand. I think you should always seek to make your code self-documenting, however it is never a good idea to rely on this alone. Combine this with comments.  
- Comments that explain the code, especially the more difficult parts, functions, etc. If this code is being read by someone much less experienced with the problem and your algorithm, then what comments would help them understand? If you were in this situation, what would help you? 
- [Auto-generated documentation](https://en.wikipedia.org/wiki/Documentation_generator). By this, I mean following a pattern of commenting in a specific way so as to be understood by a programming tool called a documentation generator. There are many options out there, and it seems the most popular (for Python) is [Sphinx](https://www.sphinx-doc.org/en/master/). However, I shall be using [Doxygen](https://www.doxygen.nl/manual/docblocks.html) just because that is what I'm used to (most of my programming is done in C++ and Fortran, which Doxygen also supports). Not only does a tool like Doxygen systematise your commenting, but you can also use it to generate an interactive webpage where you can read the documentation in a pleasant fashion. I shall use this in the next section (tutorial). While not really necessary most of the time, I find it helpful and suggest at least exploring it as an option. 
- User manuals. This is usually a lot more work, but for complex code (and especially if you plan on monetising this code) you may want to write a user (and developer) manual, where you explain in some detail how to use your code and what it does. This generally isn't necessary, but it's usually nice to include at least a few paragraphs of explanation in a `README` file for more complex projects. 

Always have at least the first two. The other two are bonus. Also, remember to update your documentation whenever you update the relevant code! 

## Modularity 

After documentation, in my opinion the most important practice to learn is modularising your code. Modularity basically just means breaking your code into sections (called _modules_) which do not depend on the internal details of other sections. 

TODO maybe just do the tutorial first, then come back to explain these 

TODO 
clarity, better compilation (not really relevant for Python), better version control (see below), easier testing and reuse (see below)

## Debugging 
TODO 
debugging

## Version Control 
TODO 
git/version control 

## Unit Tests and Integration Tests 
TODO 
software is constantly evolving, want to make sure that it is robust to change (sometimes an edit might inadvertently change an old feature you want to keep)

explain unit tests 

TDD 

<hr>

[End of Section Tutorial](sec1_tut)

[Previous Lesson](sec1_2)

<hr> 


[^1]: TODO