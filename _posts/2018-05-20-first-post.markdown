---
title:  "Week 1: Getting started"
date:   2018-05-20
categories: [GSoC]
tags: [GSoC]
---
Hello everyone. I am Akash, and this is the first in the series of blogs where I'll be writing about my experience with the project on improving the SymPy stats module as a part of GSoC'18.

Before the coding period actually started, my mentors had discussed with me certain issues about how I approached stochastic processes in my proposal. We did not decided upon how exactly the implementation would look like, but I believe it will be sorted out before we get to that part of the summer project, which is supposed one of the later phases. After my exams ended on the 11th of May, I started working on the implementation of discrete random variables, and was able to implement some of the missing classes in the file drv.py in [#14218](https://github.com/sympy/sympy/pull/14218).
Here's a short example of what was implemented:

```
>>> from sympy.stats import Poisson, P
>>> Y = Poisson('Y', 1)
>>> P(Y > 5, Y > 3)
3*(-163/60 + E)/(-8 + 3*E)
```

Right now, I am working on the implementation of product probability spaces, and extending them for discrete random variables. All in all, I am very excited about the summer project, and hope to achieve the targets in the best way possible.
