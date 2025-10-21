---
title: NAIL062 Homework: SAT Solver Application
---

# NAIL062 Homework: SAT Solver Application

Your task is to create a system for solving a given computational problem using a SAT solver. We will solve a *decision problem* (yes/no answer); if it is an optimization problem, solve its decision variant: "Does the given instance have a solution whose objective function is at least/at most a given value?" 

## Deadlines

Unless your instructor specifies otherwise:

* expressing preferences or proposing your own problems to solve: **by Oct 25**
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

You must work completely independently. You are not allowed to consult your solution with anyone except the instructor, nor to use generative AI tools. You may search for supplementary information about the problem (e.g., interesting instances or clarification of the problem statement), but this must not concern its CNF encoding or use of the SAT solver to solve it. You may also not read any code solving this (or related) problem. In case of uncertainty about how to proceed, contact the instructor, who will provide help or guidance.

## Example Solution

For inspiration, see the [example solution](https://gitlab.mff.cuni.cz/svancaj/logika_SAT_example) ([.zip](https://github.com/jbulin-mff-uk/nail062/raw/main/tutorial/sat-project/logika_SAT_example-master.zip)) for the [15 Puzzle](https://en.wikipedia.org/wiki/15_puzzle), kindly prepared by Dr. Jirka Švancara (big thanks to him).

## Assignment

Each student within one group will solve a different problem. You can choose from the list below, or you may propose your own problem that interests you: in that case, describe (by email) what the problem is and why it interests you (subject to approval by the instructor; it must be reasonably challenging — therefore, also state your preferences from the list as a backup).

Unless your instructor specifies otherwise:

Enter your preferences in SIS in the Study Group Roster as problem numbers separated by commas, e.g. "17,3,21,38". You may list any number of problems, in order of preference. If more than one student is interested in your top-preference problem, it will be assigned randomly to one of them, and the process will continue down your list of preferences. Then, any students without problems will be randomly assigned a problem from the remaining unassigned problems.

## Submission

Unless your instructor specifies otherwise:

Submit the finished project in the SIS module Study Group Roster as a link to a GitHub or GitLab repository. The repository must either be public, or you must grant your instructor access.

## List of Problems

1. [Bipartite Dimension](https://en.wikipedia.org/wiki/Bipartite_dimension)
2. [Clique Cover](https://en.wikipedia.org/wiki/Clique_cover)
3. [Cubic Subgraph](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 26)
4. [Degree-constrained Spanning Tree](https://en.wikipedia.org/wiki/Degree-constrained_spanning_tree)
5. [Domatic Number](https://en.wikipedia.org/wiki/Domatic_number)
6. [Exact Cover](https://en.wikipedia.org/wiki/Exact_cover)
7. [Garden of Eden](https://conwaylife.com/wiki/Garden_of_Eden)
8. [Graph Isomorphism](https://en.wikipedia.org/wiki/Graph_isomorphism_problem)
9. [Graph Partitioning](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 25)
10. [Hamiltonian Path](https://en.wikipedia.org/wiki/Hamiltonian_path_problem)
11. [Hitori](https://en.wikipedia.org/wiki/Hitori)
12. [Induced Subgraph Isomorphism](https://en.wikipedia.org/wiki/Induced_subgraph_isomorphism_problem)
13. [Intersection Number](https://en.wikipedia.org/wiki/Intersection_number_(graph_theory))
14. [Kernel](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 18)
15. [Killer Sudoku](https://www.csplib.org/Problems/prob057/), zobecnění pro mřížku $n\times n$ (where $n$ is a square)
16. [Longest Circuit](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 17)
17. [Maximum Clique](https://www.csplib.org/Problems/prob074/)
18. [Maximum Density Still Life](https://www.csplib.org/Problems/prob032/)
19. [Minesweeper](https://en.wikipedia.org/wiki/Minesweeper_(video_game))
20. [Minimum Test Set](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 44)
21. [Monochromatic Triangle](https://en.wikipedia.org/wiki/Monochromatic_triangle)
22. [Nonogram](https://www.csplib.org/Problems/prob012/)
23. [Numberlink](https://en.wikipedia.org/wiki/Numberlink)
24. [Nurikabe](https://en.wikipedia.org/wiki/Nurikabe_(puzzle)), you can limit the numbers to 1 or 2
25. [Peaceably Co-existing Armies of Queens](https://www.csplib.org/Problems/prob110/), generalized for an $n\times n$ chessboard
26. [Rural Postman](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 34)
27. [Set Cover](https://en.wikipedia.org/wiki/Set_cover_problem)
28. [Set Packing](https://en.wikipedia.org/wiki/Set_packing)
29. [Set Splitting](https://en.wikipedia.org/wiki/Set_splitting_problem)
30. [Shortest Common Superstring](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 16)
31. [Slitherink](https://en.wikipedia.org/wiki/Slitherlink)
32. [Social Golfers Problem](https://www.csplib.org/Problems/prob010/)
33. [Sports Tournament Scheduling](https://www.csplib.org/Problems/prob026/)
34. [Square-Tiling](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (Problem no. 54)
35. [Steiner Triple Systems](https://www.csplib.org/Problems/prob044/)
36. [Subgraph Isomorphism](https://en.wikipedia.org/wiki/Subgraph_isomorphism_problem)
37. [Three-dimensional Matching](https://en.wikipedia.org/wiki/3-dimensional_matching)
38. [Word Design for DNA Computing on Surfaces](https://www.csplib.org/Problems/prob033/)
