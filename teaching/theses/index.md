---
title: Theses and student projects
---

# Theses and student projects

I am currently looking for at least two new bachelor students and at least one master student. Get in touch to discuss more!

## Bachelor theses

Suitable in particular for specializations General computer science and Artificial Intelligence. I prefer topics in or adjacent to the following areas:

* constraint satisfaction
* computational logic
* descriptive complexity
* discrete optimization

You are however most welcome to bring your own topic, I am open to new areas as long as I feel I will be able to provide meaningful supervision.

## Software projects

Some of the topics are suitable for a software project as well. Typically, but not necessarily, the software you would be implementing would be of experimental and/or theoretical flavor.

## Master theses

Also preferably related to some of the above areas, or my reserach. We can tailor the topic to fit both our interests.

Informal inquiries are most welcome!


## Some particular open topics I have in mind:

### **Efficient testing of polymorphism conditions for digraphs**

* suitable for a software project and bachelor thesis (could possibly be expanded to a master thesis)
* keywords: constraint satisfaction; graph homomorphism; polymorphism; arc consistency

The goal of this thesis is to propose and implement an efficient heuristic algorithm for testing whether a given digraph H satisfies a given polymorphism condition.

A polymorphism of a directed graph H is an edge-preserving multivariate function on the vertex set. The existence of polymorphisms with certain properties, typically expressed by a set of identities, is tightly connected to the complexity of the graph homomorphism problem CSP(H). For instance, if H admits a ternary polymorphism satisfying f(x,x,y)=f(x,y,x)=f(y,x,x)=x, as is the case for e.g. K_2 or C_3, then CSP(H) is in NL. The existence of such a polymorphism can be checked by constructing the categorical power H^3, identifying the triples that ought to be equal, and testing for a homomorphism from the resulting graph into H. Homomorphism testing can be done fairly efficiently using constraint programming methods, e.g. arc consistency and various implicit constraints based on local structure of G and H. However, explicit a priori construction of H^n can be prohibitively expensive for larger arities n.

The student will
* implement a baseline approach via explicit construction of H^n,
* design a method that avoids explicit construction of H^n by generating tuples lazily and integrating propagation and pruning techniques from graph homomorphism solvers during the search, and
* experimentally compare the approaches.

[1] Kraiczy, S., & McCreesh, C. (2021). Solving Graph Homomorphism and Subgraph Isomorphism Problems Faster Through Clique Neighbourhood Constraints. International Joint Conference on Artificial Intelligence.
[2] Chen, H., & Larose, B. (2017). Asking the Metaquestions in Constraint Tractability. ACM Trans. Comput. Theory, 9(3), 11:1-11:27. https://doi.org/10.1145/3134757
[3] Bodirsky, M., Bulín, J., Starke, F., & Wernthaler, M. (2023). The smallest hard trees. Constraints, 28(2), 105–137. https://doi.org/10.1007/s10601-023-09341-8
[4] Barto, L., Krokhin, A., & Willard, R. (2017). Polymorphisms, and how to use them. https://doi.org/10.4230/dfu.vol7.15301.1
