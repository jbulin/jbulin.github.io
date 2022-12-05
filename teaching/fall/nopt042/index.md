---
title: "NOPT042 Constraint programming"
---

# NOPT042 Constraint programming

> In the tutorial we will be modeling constraint problems in the logic-based multi-paradigm language Picat 
    (<span style="color:fuchsia">**P**</span>attern-matching,
    <span style="color:fuchsia">**I**</span>ntuitive,
    <span style="color:fuchsia">**C**</span>onstraints,
    <span style="color:fuchsia">**A**</span>ctors,
    <span style="color:fuchsia">**T**</span>abling).

<!--
* [GitHub Classroom](https://classroom.github.com/classrooms/111507671-nopt042-tutorial) for classwork and homework assignments
-->

* [Github repository](https://github.com/jbulin-mff-uk/nopt042) for the tutorial
* Homework assignments on Github Classroom:
    - [test assignment](https://classroom.github.com/a/1ZJRMLa6) (not graded)
    - [Homework 1: leaves](https://classroom.github.com/a/SR6S7hUf) (due date extended by one week, until 2pm on Oct 14)
    - [Homework 2: crypt-arithmetic](https://classroom.github.com/a/vu6gMI8t) (due date 2pm on Oct 14)
    - [Homework 3: boardomino](https://classroom.github.com/a/grmdbx-S) (due date 2pm on Oct 21)
    - [Homework 4: knapsack](https://classroom.github.com/a/vZFFbU1t) (due date 2pm on Nov 4)
    - [Homework 5: stable-marriage](https://classroom.github.com/a/hB1TlTnz) (due date 2pm on Nov 11)
    - [Homework 6: moving](https://classroom.github.com/a/_Y3A7opJ) (due date 2pm on Nov 18)
    - [Homework 7: feast](https://classroom.github.com/a/MjThrY8R) (due date 2pm on Nov 25)
    - [Homework 8: routing](https://classroom.github.com/a/YPJdXoSh) (due date 2pm on Dec 2)
    - [Homework 9: life](https://classroom.github.com/a/gYNSo8NO) (due date 2pm on Dec 9)
    - [Homework 10: golfers](https://classroom.github.com/a/NCxkvoPf) (due date 2pm on Dec 16)
    - [Homework 11: triangle](https://classroom.github.com/a/6t1247tM) (due date 2pm on Jan 6)
    - [Homework 12: farmer](https://classroom.github.com/a/9HmbOiKX) (due date 2pm on Jan 13)
    - [Additional homework assignments for extra points: packing, mcsp, digest, hanoi](https://classroom.github.com/a/OGh06sW9) (due by end of March)

    
## Tutorial schedule

### Before the first tutorial

* Install Picat and try it out. (See [Getting started with Picat](http://picat-lang.org/download/get_started.pdf).)
* Solve the [test assignment](https://classroom.github.com/a/1ZJRMLa6). Push your solution to the repo, and check if it passed the tests.

### 1st tutorial (Sep 30)

* **Program:** Overview of Picat.
* **Homework:** [leaves](https://classroom.github.com/a/SR6S7hUf)

### 2nd tutorial (Oct 7)

* **Program:** Intro to CP.
* **Homework:** [crypt-arithmetic](https://classroom.github.com/a/vu6gMI8t)

### 3rd tutorial (Oct 14)

* **Program:** Improving models, symmetry breaking, solvers.
* **Homework:** [boardomino](https://classroom.github.com/a/grmdbx-S)

### 4th tutorial (Oct 21)

* **Program:** Search space, search strategies.
* **Homework:** [knapsack](https://classroom.github.com/a/vZFFbU1t) - due on Nov 4 (Oct 28 is a national holiday)

### 5th tutorial (Nov 4)

* **Program:** Dual modeling, channeling. Assignment.
* **Homework:** [stable-marriage](https://classroom.github.com/a/hB1TlTnz) due on Nov 11

### 6th tutorial (Nov 11)

* **Program:** Modeling functions. Scheduling, the cummulative constraint
* **Homework:** [moving](https://classroom.github.com/a/_Y3A7opJ) due on Nov 18

### 7th tutorial (Nov 18)

* **Program:** Rostering
* **Homework:** [feast](https://classroom.github.com/a/MjThrY8R) due Nov 25

### 8th tutorial (Nov 25 )

* **Program:** Routing
* **Homework:** [routing](https://classroom.github.com/a/YPJdXoSh) due Dec 2

### 9th tutorial (Dec 2)

* **Program:** Implicit constraints
* **Homework:** [life](https://classroom.github.com/a/gYNSo8NO) due Dec 9

### 10th tutorial (Dec 9)

* **Program:** Modeling with sets
* **Homework:** [golfers](https://classroom.github.com/a/NCxkvoPf) due Dec 16

### 11th tutorial (Dec 16)

* **Program:** Tabling
* **Homework:** [triangle](https://classroom.github.com/a/6t1247tM) due Jan 6

### 12th tutorial (Jan 6)

* **Program:** Planning
* **Homework:** [farmer](https://classroom.github.com/a/9HmbOiKX) due Jan 13
* **Additional homework problems:** [packing, mcsp, digest, hanoi](https://classroom.github.com/a/OGh06sW9) due end of March

## Resources

* [Picat homepage](https://picat-lang.org)
* [Getting started with Picat](http://picat-lang.org/download/get_started.pdf)
* [Constraint solving and planning with Picat](https://picat-lang.org/picatbook2015.html)
* [Modeling and Solving AI Problems in Picat
(tutorial by R. Barták and N. Zhou)](http://ktiml.mff.cuni.cz/~bartak/AAAI2017/)
* [CSPLib: A problem library for constraints](https://www.csplib.org)
* [Håkan Kjellerstrand's Picat page](https://hakank.org/picat)
* [The lecture by R. Barták](https://ktiml.mff.cuni.cz/~bartak/podminky)
* [Previous tutorial by R. Barták in SICStus Prolog](https://ktiml.mff.cuni.cz/~bartak/podminky/#cviceni)
* [Previous tutorial by me in MiniZinc](https://dl1.cuni.cz/course/view.php?id=10544)

## Credit requirements

There will be 12 homework assignments each of which is worth 1 point. In order to get the credit, you must gain at least 8 points, out of which at least 4 points must be from the second half of the semester (assignments 7-). Expect increasing complexity of the assignments as the semester progresses. There will be an additional option to get at most 4 points after the end of classes for solving somewhat harder problems.

The solutions to the homework assignments must be 100% your own work. Do not discuss them with anyone but me, do not search for solutions on the internet, and do not share your code.

## Frequently asked questions (FAQ)

* _What should I do if I have a question?_ --- Check the FAQ. If you don't see the answer here email me putting "nopt042" in the subject.
* _What if I want a consultation?_ --- Talk to me after class, come to the scheduled office hours, or email me to arrange an appointment.
