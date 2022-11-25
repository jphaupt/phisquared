---
layout: lecture
# "non-specific tag" YAML syntax
title: ! 'Tutorial: The Logistic Map'
author: jph
init_date: 16 Dec 2020
---

In this section, we will be discussing an unassuming sequence, the _logistic map_: 

$$
x_{n+1} = rx_n(1-x_n)
$$

where $r$ is just a preset parameter (called the _growth rate_). You can consider $x_n$ to be the population of the system at time step $n$. $r$ then describes how the population changes based on its previous value. You can therefore imagine this to be a simple model for some kind of population dynamics problem. 

More than that, however, we will find that this is one of the simplest examples of a _chaotic system_! 

## Exploratory Analysis 

We won't always do this in these tutorials, but now is a good time to play around with the function. Write a function in Python (or whatever language you are using) for the logistic map, and generate sequences $x_0, x_1, x_2, ...$ and plot $x$ against $n$. Try this for $r=0,0.5,1,2,3,4$. What do you see? 

TODO maybe put this in some kind of "answer" section? I included 0 above
As you might expect, if $r$ is small, the population decreases to zero (certainly this is true for $r=0$). As a sanity check, evaluate $x_n$ for $n=1,...,N$ for some large $N$ (say, $N=100$). 

TODO outline idea 

- complete motivation 
- explorative analysis (just check some r values) 
- bifurcation maps
- zoom in to show fractal 
- Poincare plot (compare to randomness)

- consequences 
    - fundamental limits of human understanding (compare to randomness)
    - super sensitive to initial conditions
        - butterfly effect

- what you learned 
    - congrats, you just solved your first physics problem on a computer! 


--

TODO explain some motivation for it (population dynamics)

TODO https://geoffboeing.com/2015/03/chaos-theory-logistic-map/

TODO maybe actually do the Lorenz attractor, just to be different? I think there was a nice Julia implementation on the plotting package

<hr> 

In addition to the usual citations, a good chunk of what I wrote here also comes from [this webpage](https://geoffboeing.com/2015/03/chaos-theory-logistic-map/) and its corresponding paper: Boeing, G. 2016. “Visual Analysis of Nonlinear Dynamical Systems: Chaos, Fractals, Self-Similarity and the Limits of Prediction.” Systems, 4 (4), 37. doi:10.3390/systems4040037

In particular, a lot of the values I chose come from this page. 

I also referred to Strogatz's _Nonlinear Dynamics and Chaos_ a few times, which I strongly recommend reading if you find this topic interesting. 