---
title: "NOPT061 Large-scale optimization: Metaheuristics"
---

# NOPT061 Large-scale optimization: Metaheuristics

* Home of the [tutorial](https://ktiml.mff.cuni.cz/~fink/teaching/large_scale_optimization/) by Jirka Fink is [here](https://ktiml.mff.cuni.cz/~fink/teaching/large_scale_optimization/).

The course is taught bi-yearly (in even-numbered years), alternating with the course [NOPT059 Large-scale optimization: Exact methods](../nopt059/).

The course will be scheduled in the beginning of the semester (probably during the first week). Classes start from the second week. If you are interested, please email me your time constraints.

## Schedule for Spring 2026

* Lecture: Friday, 9am in S1
* Practical: Friday, 10:40am in S4


## About this course

The aim of course is to introduce the main principles of various heuristic optimization methods based on convex optimization and artificial intelligence, with emphasis on large-scale instances. Moreover, during the accompanying tutorial you will gain experience in applying these methods in practice.

We expect you to be somewhat familiar with linear programming. Although certainly not necessary, a useful prerequisite is the course [NOPT048 Linear programming and combinatorial optimization](https://is.cuni.cz/studium/eng/predmety/index.php?do=predmet&kod=NOPT048).

## Resources

* [powerful] Blum, Raidl - Hybrid Metaheuristics: Powerful Tools for Optimization
* [emerging] Blum et al - Hybrid Metaheuristics: An Emerging Approach to Optimization
* [handbook] Gendreau, Potvin - Handbook of Metaheuristics (3rd edition)
* [comparing-memetic] Jiaojiao, Gulyás, Botzheim - Comparing Lamarckian and Baldwinian Approaches in Memetic Optimization
* [multi-depot-scheduling] Otsuki, Aihara - New variable depth local search for multiple depot vehicle scheduling problems
* [algorithms-for-optimization] Kochenderfer, Wheeler - Algorithms for Optimization
* [search-methodologies] Burke, Kendall - Search Methodologies: Introductory Tutorials in Optimization and Decision Support Techniques

## Tentative schedule

### Lecture 1 - Introduction, Heuristics, Metaheuristics

Combinatorial optimization
* Examples: Traveling Salesman Problem (TSP), Knapsack
* Exact method, heuristic, metaheuristic, hybrid metaheuristic

Basic heuristic methods
* Constructive heuristics (example: greedy)
* Local search (LS)
  * extension: Variable neighborhood descent

Metaheuristics
* Greedy randomized adaptive search procedure (GRASP)
* Iterated greedy algorithms
* Iterated local search
* Simulated annealing
* Tabu search
* Variable neighborhood search (VNS)
* Ant colony optimization (ACO)

#### Resources

* [powerful] Introduction, 1.1-1.2 (skip 1.2.8)

### Lecture 2 - Evolutionary and Memetic Algorithms, Exact Methods

Evolutionary and memetic algorithms
* Evolutionary algorithms
* Memetic algorithms
* Lamarckian vs. Baldwinian learning

Exact methods
* Tree search methods (Branch and Bound, example: Knapsack)
* Dynamic programming (example: Knapsack)
* Mixed integer programming (MIP) (review of LP, if necessary)
* Constraint programming (CP)

#### Resources

* [powerful] Subsection 1.2.8, Section 1.7
* [handbook] Chapter 9 (An Accelerated Introduction to Memetic Algorithms)
* [comparing-memetic] Section 2 (and the rest)

### Lecture 3 - Incomplete Solutions and Decoders

Incomplete/indirect solution representations

Decoder-based metaheuristics

Application: Generalized Minimum Spanning Tree
* Initial solutions
* Node set based VNS
* Global edge set based VNS
* Combined VNS

#### Resources

* [powerful] Chapter 2

### Lecture 4 - Problem Instance Reduction

Construct, Merge, Solve & Adapt Algorithm(CSMA)

Application: Minimum Common String Partition
* Probabilistic solution generation
* Solving reduced sub-instances

#### Resources

* [powerful] Chapter 3

### Lecture 5 - Large Neighborhood Search

MIP-based Large neighborhood search

Application: Minimum Weight Dominating Set
* initial solution (greedy heuristic)
* partial destruction of solutions

Application: Generalized Minimum Spanning Tree
* global subtree optimization neighborhood

#### Resources

* [powerful] Chapter 4

### Lecture 6 - Multi-depot Vehicle Scheduling

Single-depot vs. Multi-depot vehicle scheduling problem

Variable depth local search for MDVSP

#### Resources

* [multi-depot-scheduling] Sections 1, 2.1-2.5

### Lecture 7 - Parallel Non-independent Construction

General idea
Beam Search
Beam-ACO: Beam search + Ant Colony Optimization

Application: Multidimensional Knapsack (MK)
* greedy heuristic
* beam search for MK
* pure-ACO approach to MK
* Beam-ACO for MK

#### Resources

* [powerful] Chapter 5

### Lecture 8 - Construction and Constraint Programming

Hybrids of constructive metaheuristics and constraint programming

Ant-Colony optimization + constraint programming integration

Application: Machine Scheduling with Sequence-dependent Setup Times

#### Resources

*[emerging] Paper 6

### Lecture 9 - Complete solution archives

General idea

Trie-based archive

Application: Generalized Minimum Spanning Tree (GMST)

* Archive-Enhanced Evolutionary Algorithm for GMST

#### Resources

* [powerful] Chapter 6, Sections 6.1 & 6.3

### Lecture 10 - Surrogate models

Surrogate models

Probabilistic surrogate models

Surrogate optimization

#### Resources

* [algorithms-for-optimization] Chapters 14-16

### Lecture 11 - Hyper-heuristics

Introduction

Hyper-heuristics for

* Boolean Satisfiability
* Timetabling
* Packing

#### Resources

* [search-methodologies] Chapter 20

## Exam requirements

The exam is oral with written preparation. Requirements for the exam correspond to the syllabus of the course in the extent that has been covered in the lecture. Obtaining the credit from the tutorial is a necessary requirement for taking the exam.

## Frequently asked questions (FAQ)

* _I am interested in this course!_ --- That's not a question. But email me!
* _Where and when is the first class?_ --- The course will start in the second week of the semester. We will agree on the where and when by email during the first week.
* _What should I do if I have a question?_ --- Check the FAQ. If you don't see the answer here email me putting "nopt061" in the subject.
* _What if I want a consultation?_ --- Talk to me after class, come to the scheduled office hours, or email me to arrange an appointment.
