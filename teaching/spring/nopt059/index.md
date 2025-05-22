---
title: "NOPT059 Large-scale optimization: Exact methods"
---

# NOPT059 Large-scale optimization: Exact methods

The course is taught bi-yearly (in odd-numbered years), alternating with the course [NOPT061 Large-scale optimization: Metaheuristics](../nopt061/).

The course will be scheduled in the beginning of the semester (probably during the first week). If you are interested, please email me your time constraints.

## About this course

The aim of course is to introduce the main principles of various exact optimization methods based on linear programming and combinatorial optimization with emphasis on large-scale instances. Moreover, during the accompanying tutorial you will gain experience in applying these methods in practice.

We expect you to be somewhat familiar with linear programming. Although certainly not necessary, a recommended prerequisite is the course [NOPT048 Linear programming and combinatorial optimization](https://is.cuni.cz/studium/eng/predmety/index.php?do=predmet&kod=NOPT048).

## Resources

* [Webpage of the tutorial](https://ktiml.mff.cuni.cz/~fink/teaching/) (taught by Jirka Fink)
* [This course in the SIS](https://is.cuni.cz/studium/eng/predmety/index.php?do=predmet&kod=NOPT059)
* [wolsey](https://onlinelibrary.wiley.com/doi/10.1002/9781119606475.oth1) The book __Laurence Wolsey, Integer programming, 2nd edition, Wiley 2020__ covers a majority of the course material.
* [lagrange](https://www.ens-lyon.fr/DI/wp-content/uploads/2012/01/LagrangianRelax.pdf) Lecture notes on Lagrangian relaxation.
* [matousek](https://link.springer.com/book/10.1007/978-3-540-30717-4) If you need a referecne for basics of Linear programming theory, you can refer to, for example, __Jiří Matoušek, Bernd Gärtner, Understanding and Using Linear Programming, Springer 2007__.


## Tentative schedule

### Lecture 0 - Linear programming basics

Linear programs

* systems of linear equations vs. linear programs
* canonical and equational form
* geometry of linear programs
* convexity, polyhedron, polytope
* Minkowski-Weyl Theorem

Simplex method

* geometric intuition
* basic feasible solutions

Duality of linear programming

* intuition
* primal and dual programs
* weak and strong duality theorems
* complementary slackness
* weak/strong-dual pair of problems in general
* example: maximum cardinality matching vs. minimum cardinality covering

__Resources:__ any textbook on linear programming (e.g. [matousek]), [wolsey] 2.5-6, for the simplex method: [video tutorial](https://www.youtube.com/watch?v=9YKLXFqCy6E&t=757s&ab_channel=JoshuaEmmanuel)

### Lecture 1 - Introduction. Modeling using Integer programming

Introduction

* Discrete optimization, examples
* Exact methods vs. metaheuristics

Modeling using Integer programming

* integer linear program, mixed integer program, 0-1 integer program
* modeling fixed costs, disjunction
* good, better, ideal formulation _(later: lazy constraint generation)_
* example: Travelling salesman problem (subtour elimination constraints)

__Resources:__ [wolsey] 1.1-1.7

### Lecture 2 - Branch and bound

Optimality and relaxation

* primal and dual bounds
* relaxation
* droping constraints (example: knapsack)
* linear programming relaxation
* _(later: Lagrangian relaxation)_

Branch and bound

* divide and conquer, branching, search tree
* pruning (by optimality, by bounds)
* example: knapsack (primal bound: greedy heuristic, dual bound: drop weight constraint/LP-relaxation)
* node selection: DFS, BFS, best-first, least-discrepancy
* implementation: store list of active nodes, global bounds

LP-based B&B

* branching strategy (most fractional variable, estimating pseudocosts)
* store dual basis, after adding branching inequality still dual-feasible, easy to reoptimize
* example

__Resources:__ [wolsey] 2.1-2.3, 7.1-4

### Lecture 3 - Cutting plane algorithms, Gomory's algorithm

Lazy constraint generation

* example: travelling salesman problem (eliminate subtour)

Valid inequalities

* given vs. ideal formulation
* geometric intuition
* the separation problem
* examples

Cutting planes

* generic cutting planes algorithm
* Gomory cuts
* Gomory fractional cutting planes algorithm
* example, using dual simplex method
* Chvátal-Gomory procedure to construct any valid inequality

__Resources:__ [wolsey] 8.1-8.3, 8.6

### Lecture 4 - Strong valid inequalities

Strong valid inequalities

* redundant inequalities
* minimal description of a polyhedron
* nonredundant inequalities define represent facets
* example: blossom inequalities for matching

0-1 Knapsack

* cover inequalities
* extended conver inequalities
* lifting cover inequalities to obtain facet-definining inequalities

Branch-and-cut

* embed strong cutting planes into branch and bound
* example: graph coloring (clique and odd-hole constraints)

__Resources:__ [wolsey] 9.1-3, 9.5-6

### Lecture 5 - Lagrangian relaxation

Lagrangian relaxation

* easy vs. complicating constraints
* idea: approximate by easier problem, price for violation (Lagrange multiplier)
* definition
* weak duality

Example: Resource-constrained shortest path

* obtaining dual bound,
* finding feasible solution

__Resources:__ [wolsey] 10.1, [lagrange] 12.1


### Lecture 6 - Lagrangian duality

Lagrangian dual

* Lagrangian bounding principle (it is a dual bound)
* weak duality property
* optimality test (primal-feasible + complementary slackness)
* duality gap as a certificate of near-optimality

Example: Traveling Salesperson Problem
* either dualize degree constraints, optimize 1-trees, or
* dualize subtour elimination constraints (express them as a flow), optimize cycle factor problem (corresponds to perfect matching)

Subgradient method

* idea: gradient descent but for nonsmooth, convex functions
* subgradient, subdifferential (set of all subgradients)
* subgradient algorithm: step in any subgradient direction
* step size: constant, diminishing, adaptive (problem-specific)

__Resources:__ [wolsey] 10.2-3, [lagrange] 12.2-3


### Lecture 7 - Column generation

Motivation:
* good/ideal formulations with exponentially many constraints
* more complex variables
* lazy constraint generation
* idea: branch and price

Example: Cutting Stock
* naive formulation: bad, weak LP relaxation, lots of symmetries (symmetry breaking)
* generate configurations on demand
* how to choose configurations? princing problem (knapsack)


Column generation:
* master problem, restricted master problem
* explicit pricing vs. implicit pricing
* generating initial set of configurations

Example: Vertex Coloring
* naive model
* master model: color classes (independent sets)

Branch and price:
* branch and bound, generate new columns at every node to improve relaxation
* run column generation
* if integral, terminate
* else, branch

__Resources:__ [wolsey] 11.1, 11.3


### Lecture 8 - Dantzig-Wolfe decomposition

Motivation:
* how to find useful master problem formulations?
* "forget" about rolls/colors, aggregate

Dantzig-Wolfe reformulation
* outer and inner representation of a polyhedron (Minkowski-Weyl)
* idea: apply Minkowski-Weyl on "easy" constraints
* Dantzig-Wolfe Master problem, RMP
* reduced cost computation

Block-Angular matrices
* subproblems (rolls in cutting stock, colors in Vertex coloring, vehicles in Vehicle routing)
* only linked by "total" constraints
* blocks can be identical, then we can aggregate

Example: Resource Constrained Shortest Path
* Dantzig-Wolfe reformulation, complex variables: all (s,t)-paths
* pricing problem: shortest path

__Resources:__ [wolsey] 11.2, 11.5

### Lecture 9 - Branch-price-and-cut

Motivation
* strengthen relaxation for branch-and-bound?
* column generation: adding columns
* cutting planes: adding rows
* combine both

Branch-price-and-cut
* Dantzig-Wolfe reformulation provides stronger relaxation
* strengthen it further by cutting planes
* cutting planes on the original variables
* cutting planes on master variables
* branch only on original variables

Examples: 
* Edge coloring problem (odd circuit cuts)
* Resource Constrained Shortest Path

__Resources:__ [wolsey] 11.4, 11.6-7

### Lecture 10 - Selected applications

Vehicle routing problem with time windows
* column generation
* branching strategies

__Resources:__ Chapter 3 of [Desaulniers et al: Column Generation, Springer, 2005](https://link.springer.com/book/10.1007/b135457)

<!--
TBA (Branch-price-and-cut for Multi-Agent Pathfinding?)

__Resources:__ [Branch-and-cut-and-price for multi-agent path finding](https://www.sciencedirect.com/science/article/pii/S0305054822000946)
-->

## Exam requirements

The exam is oral with written preparation. Requirements for the exam correspond to the syllabus of the course in the extent that has been covered in the lecture. Obtaining the credit from the tutorial is a necessary requirement for taking the exam.

## Frequently asked questions (FAQ)

* _I am interested in this course!_ --- That's not a question. But email me!
* _Where and when is the first class?_ --- The course will start in the second week of the semester. We will agree on the where and when by email during the first week.
* _What should I do if I have a question?_ --- Check the FAQ. If you don't see the answer here email me putting "nopt059" in the subject.
* _What if I want a consultation?_ --- Talk to me after class, come to the scheduled office hours, or email me to arrange an appointment.
