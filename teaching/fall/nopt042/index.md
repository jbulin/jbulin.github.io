---
title: "NOPT042 Constraint programming"
---

# NOPT042 Constraint programming (Fall 2025)

> In the tutorial we will be modeling constraint problems in the logic-based multi-paradigm language Picat 
    (<span style="color:fuchsia">**P**</span>attern-matching,
    <span style="color:fuchsia">**I**</span>ntuitive,
    <span style="color:fuchsia">**C**</span>onstraints,
    <span style="color:fuchsia">**A**</span>ctors,
    <span style="color:fuchsia">**T**</span>abling).


## Office hours during the teaching period:

<span style="color:red">**Oct 9: Today's office hours are postponed from 2pm to 5:15pm**</span>

* Monday 10:40am in S303
* Thursday 2pm in S303 (on Nov 20 cancelled due to a workshop)

or make an appointment (via email); two additional hours per week will be available.


## Credit requirements

There will be 12 homework assignments each of which is worth 1 point. In order to get the credit, you must gain at least 8 points, out of which at least 4 points must be from the second half of the semester (assignments 7-). Expect increasing complexity of the assignments as the semester progresses. There will be an additional option to get at most 4 points after the end of classes for solving somewhat harder problems.

The solutions to the homework assignments must be 100% your own work. Do not discuss them with anyone but me, do not search for solutions on the internet, and do not share your code.

## ReCodEx

Homework assignments will be posted in [ReCodEx](https://recodex.mff.cuni.cz/). The deadlines will be set to the beginning of the next tutorial, unless stated otherwise.

## GitHub and Binder

The source codes and live notebooks are available on GitHub, and hosted on Binder:

* [GitHub repository](https://github.com/jbulin-mff-uk/nopt042)
* [Binder docker](https://mybinder.org/v2/gh/jbulin-mff-uk/nopt042/HEAD) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jbulin-mff-uk/nopt042/HEAD)

The individual notebooks are also posted below as PDFs and HTML slides.

## Resources

* [Picat homepage](https://picat-lang.org)
* [Getting started with Picat](http://picat-lang.org/download/get_started.pdf)
* [Constraint solving and planning with Picat](https://picat-lang.org/picatbook2015.html)
* [Modeling and Solving AI Problems in Picat (tutorial by R. Barták and N. Zhou)](http://ktiml.mff.cuni.cz/~bartak/AAAI2017/)
* [CSPLib: A problem library for constraints](https://www.csplib.org)
* [Håkan Kjellerstrand's Picat page](https://hakank.org/picat)
* [The lecture by R. Barták](https://ktiml.mff.cuni.cz/~bartak/podminky)
* [Previous tutorial by R. Barták in SICStus Prolog](https://ktiml.mff.cuni.cz/~bartak/podminky/#cviceni)
* [Previous tutorial by me in MiniZinc](https://dl1.cuni.cz/course/view.php?id=10544)

## Tutorial schedule (will be updated)

### Before the first tutorial

* Install Picat and try it out. (See [Getting started with Picat](http://picat-lang.org/download/get_started.pdf).)
* Join our ReCodEx group. 
* Solve the (ungraded) "Hello, World!" assignment.
* Let me know if you encounter any issues!

### 1st tutorial (Sep 29)

* **Program:** Overview of Picat.
* **Notebook:** [tutorial1.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial1/tutorial1.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial1/tutorial1.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial1/tutorial1.slides.html))
* **Homework:** Leaves

### 2nd tutorial (Oct 6)

* **Program:** Intro to CP.
* **Notebook:** [tutorial2.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial2/tutorial2.ipynb)  ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial2/tutorial2.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial2/tutorial2.slides.html))
* **Homework:** Crypt-arithmetic

### 3rd tutorial (Oct 13)

* **Program:** Improving models, symmetry breaking, solvers.
* **Notebook:** [tutorial3.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial3/tutorial3.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial3/tutorial3.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial3/tutorial3.slides.html))
* **Homework:** Boardomino

### 4th tutorial (Oct 20)

* **Program:** Search space, search strategies.
* **Notebook:** [tutorial4.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial4/tutorial4.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial4/tutorial4.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial4/tutorial4.slides.html))
* **Homework:** Knapsack

### 5th tutorial (Oct 27)

* **Program:** Dual modeling, channeling. Assignment.
* **Notebook:** [tutorial5.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial5/tutorial5.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial5/tutorial5.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial5/tutorial5.slides.html))
* **Homework:** Stable marriage

### 6th tutorial (Nov 3)

* **Program:** Modeling functions. Scheduling, the cummulative constraint.
* **Notebook:** [tutorial6.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial6/tutorial6.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial6/tutorial6.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial6/tutorial6.slides.html))
* **Homework:** Moving

### 7th tutorial (Nov 10)

* **Program:** Rostering problems. Global constraints based on finite automata.
* **Notebook:** [tutorial7.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial7/tutorial7.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial7/tutorial7.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial7/tutorial7.slides.html))
* **Homework:** Feast

### November 17: No class, national holiday

### 8th tutorial (Nov 24)

* **Program:** Global constraints. Routing.
* **Notebook:** [tutorial8.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial8/tutorial8.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial8/tutorial8.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial8/tutorial8.slides.html))
* **Homework:** Routing

### December 1: Double lecture instead of the tutorial (stay in S9)


### 9th tutorial (Dec 8)

* **Program:** Implicit constraints.
* **Notebook:** [tutorial9.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial9/tutorial9.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial9/tutorial9.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial9/tutorial9.slides.html))
* **Homework:** Life

### 10th tutorial (Dec 15)

* **Program:** Modeling with sets.
* **Notebook:** [tutorial10.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial10/tutorial10.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial10/tutorial10.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial10/tutorial10.slides.html))
* **Homework:** Golfers

### 11th tutorial (Jan 5)
* **Program:** Tabling and planning with Picat.
* **Notebook:** [tutorial11.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial11/tutorial11.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial11/tutorial11.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial11/tutorial11.slides.html)), [tutorial12.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial12/tutorial12.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial12/tutorial12.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial12/tutorial12.slides.html))
* **Homework:** Triangle, Farmer
* **Additional homework problems:** Packing, MCSP, Digest, Hanoi (due end of March)

<!--
### 11th tutorial (Dec 15)
* **Program:** Tabling with Picat.

### 12th tutorial (Jan 5)

* **Program:** Planning with Picat
* **Notebook:** [tutorial12.ipynb](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial12/tutorial12.ipynb) ([pdf](https://github.com/jbulin-mff-uk/nopt042/raw/main/tutorial12/tutorial12.pdf), [html](https://rawcdn.githack.com/jbulin-mff-uk/nopt042/4e4a0b860cc58760990ba32aa21e15de4a05a6f1/tutorial12/tutorial12.slides.html))
* **Homework:** Farmer
* **Additional homework problems:** Packing, MCSP, Digest, Hanoi (due end of March)
-->
<!--
### 13th tutorial (Jan 9)

* **Program:** Q&A, Homework help
* **Additional homework problems:** Packing, MCSP, Digest, Hanoi (due end of March)
-->

## Frequently asked questions (FAQ)

* _What should I do if I have a question?_ --- Check the FAQ. If you don't see the answer here email me putting "nopt042" in the subject.
* _What if I want a consultation?_ --- Talk to me after class, come to the scheduled office hours, or email me to arrange an appointment.
