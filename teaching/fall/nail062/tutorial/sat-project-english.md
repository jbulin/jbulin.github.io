---
title: NAIL062 Homework: SAT Solver Application
---

# NAIL062 Homework: SAT Solver Application

Your task is to create a system for solving a given computational problem using a SAT solver. We will solve a *decision problem* (yes/no answer); if it is an optimization problem, solve its decision variant: "Does the given instance have a solution whose objective function is at least/at most a given value?" 

## Deadlines

Unless your instructor specifies otherwise:

* expressing preferences or proposing your own problems to solve: **by October 20**
* submission of the finished project: **by the end of November**

## Assignment Guidelines

Use the Python 3 programming language and the SAT solver [Glucose 4.2](https://github.com/audemard/glucose/). Do not use any libraries that convert formulas to CNF or similar.

Program a script that:

* accepts a problem instance as input (either parameters, or a path to a file describing the instance, or a combination of both),
* encodes this instance into SAT in [DIMACS CNF](https://jix.github.io/varisat/manual/0.2.0/formats/dimacs.html) format,
* calls the Glucose SAT solver on the CNF formula,
* decodes the resulting variable assignment (if any) back to a solution of the problem,
* prints this solution in a reasonable, human-readable format.
* the script will moreover be able to optionally print the constructed CNF formula in DIMACS CNF format, and statistics about the SAT solver's execution.

Include several instances for testing, at least:

* a small, human-analyzable satisfiable instance,
* a small, human-analyzable unsatisfiable instance (if one exists),
* a satisfiable instance that runs for a non-trivial amount of time (at least 10s); if you cannot find one, describe your attempt.

The submission must also include a `README.md` file with brief documentation containing:

* an exact description of the problem you are solving (parameters, decision variables, constraints, etc.)
* a description of your chosen CNF encoding, and possibly alternatives
* user documentation for your script (including input format, and also output format if not obvious)
* description of included instances
* description of experiments you performed (e.g., what size instances can your script solve in reasonable time?)

## Ethical Rules

You must work completely independently. It is not allowed to consult any intelligence except the instructor. You may search for supplementary information about the problem (e.g., interesting instances or clarification of the problem statement), but this must not concern its CNF encoding or use of the SAT solver to solve it. You may also not read any code solving this (or related) problem. In case of uncertainty about how to proceed, contact the instructor, who will provide help or guidance.

## Example Solution

For inspiration, see the [example solution](https://gitlab.mff.cuni.cz/svancaj/logika_SAT_example) ([.zip](https://github.com/jbulin-mff-uk/nail062/raw/main/tutorial/sat-project/logika_SAT_example-master.zip)) for the [15 Puzzle](https://en.wikipedia.org/wiki/15_puzzle), kindly prepared by Dr. Jirka Švancara (big thanks to him).

## Assignment

Each student within a single tutorial group will solve a different problem. You can choose from the list below, or propose your own problem of interest: In that case, describe what the problem is and why it interests you (subject to instructor approval; it must be reasonably challenging; so it is better to also indicate your preferences from the list).

Unless your instructor specifies otherwise:

Send your preferences to the instructor by email. You may list any number of problems, one problem per line in order of preference. If more students request the same most-preferred problem, it will be assigned randomly to one, and the next preference will be considered. Unassigned problems will be randomly assigned to remaining students.

## Submission

Unless your instructor specifies otherwise:

Submit the finished project either as a link to a public GitHub or GitLab repository, or as a `.zip` file; send one of these by email to the instructor.

## List of Problems

* [Bipartite Dimension](https://en.wikipedia.org/wiki/Bipartite_dimension)
* [Clique Cover](https://en.wikipedia.org/wiki/Clique_cover)
* [Cubic Subgraph](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 26)
* [Degree-constrained Spanning Tree](https://en.wikipedia.org/wiki/Degree-constrained_spanning_tree)
* [Domatic Number](https://en.wikipedia.org/wiki/Domatic_number)
* [Exact Cover](https://en.wikipedia.org/wiki/Exact_cover)
* [Graph Isomorphism](https://en.wikipedia.org/wiki/Graph_isomorphism_problem)
* [Graph Partitioning](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 25)
* [Hamiltonian Path](https://en.wikipedia.org/wiki/Hamiltonian_path_problem)
* [Induced Subgraph Isomorphism](https://en.wikipedia.org/wiki/Induced_subgraph_isomorphism_problem)
* [Intersection Number](https://en.wikipedia.org/wiki/Intersection_number_(graph_theory))
* [Kernel](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 18)
* [Killer Sudoku](https://www.csplib.org/Problems/prob057/), zobecnění pro mřížku $n\times n$ (where $n$ is a square)
* [Longest Circuit](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 17)
* [Maximum Clique](https://www.csplib.org/Problems/prob074/)
* [Maximum Density Still Life](https://www.csplib.org/Problems/prob032/)
* [Minesweeper](https://en.wikipedia.org/wiki/Minesweeper_(video_game))
* [Minimum Test Set](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 44)
* [Monochromatic Triangle](https://en.wikipedia.org/wiki/Monochromatic_triangle)
* [Nonogram](https://www.csplib.org/Problems/prob012/)
* [Numberlink](https://en.wikipedia.org/wiki/Numberlink)
* [Nurikabe](https://en.wikipedia.org/wiki/Nurikabe_(puzzle)), you can limit the numbers to 1 or 2
* [Peaceably Co-existing Armies of Queens](https://www.csplib.org/Problems/prob110/), generalized for an $n\times n$ chessboard
* [Rural Postman](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 34)
* [Set Cover](https://en.wikipedia.org/wiki/Set_cover_problem)
* [Set Packing](https://en.wikipedia.org/wiki/Set_packing)
* [Set Splitting](https://en.wikipedia.org/wiki/Set_splitting_problem)
* [Shortest Common Superstring](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 16)
* [Slitherink](https://en.wikipedia.org/wiki/Slitherlink)
* [Social Golfers Problem](https://www.csplib.org/Problems/prob010/)
* [Sports Tournament Scheduling](https://www.csplib.org/Problems/prob026/)
* [Square-Tiling](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 54)
* [Steiner Triple Systems](https://www.csplib.org/Problems/prob044/)
* [Subgraph Isomorphism](https://en.wikipedia.org/wiki/Subgraph_isomorphism_problem)
* [Three-dimensional Matching](https://en.wikipedia.org/wiki/3-dimensional_matching)
* [Word Design for DNA Computing on Surfaces](https://www.csplib.org/Problems/prob033/)
