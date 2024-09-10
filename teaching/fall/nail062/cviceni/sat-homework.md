---
title: NAIL062 Domácí úkol: aplikace SAT solveru"
---

# NAIL062 Domácí úkol: aplikace SAT solveru

Vaším úkolem bude vytvořit systém pro řešení zadaného výpočetního problém za použití SAT solveru. Jde-li o optimalizační problém, řešte jeho rozhodovací variantu: "Má daná instance řešení, jehož objektivní funkce má alespoň/nejvýše danou hodnotu?" 

## Zásady pro vypracování

K řešení použijte programovací jazyk Python a SAT solver [Glucose 4.2](https://github.com/audemard/glucose/).

Naprogramujte skript, který:

* na vstupu přijme instanci problému (buď parametry, nebo cestu k souboru popisujícímu instanci, případně obojí),
* zakóduje tuto instanci do SAT ve formátu [DIMACS CNF](https://jix.github.io/varisat/manual/0.2.0/formats/dimacs.html),
* zavolá na CNF formuli SAT solver Glucose,
* dekóduje nalezené ohodnocení proměnných (existuje-li) zpět na řešení daného problému,
* toto řešení vypíše v nějakém rozumném, člověkem čitelném formátu.
* Skript navíc volitelně vypíše zkonstruovanou CNF formuli v DIMACS CNF formátu, a statistiky o průběhu řešení SAT solveru.

K řešení přiložte několik instancí, a to alespoň:

* malou, člověkem analyzovatelnou splnitelnou instanci,
* malou, člověkem analyzovatelnou nesplnitelnou instanci (existuje-li),
* splnitelnou instanci, která poběží netriviálně dlouho (alespoň 10s), pokud se Vám ji nepodaří nalézt, popište proč.

Dále musí být součástí řešení soubor README.md se stručná dokumentací obsahující:

* přesný popis problému, který řešíte (parametry, rozhodovací proměnné, constrainty, aj.)
* popis Vámi zvoleného zakódování do CNF, případně jeho alternativ
* uživatelská dokumentace vašeho skriptu (vč. popisu formátu vstupu a výstupu)
* popis přiložených instancí
* popis experimentů, které jste prováděli (např. jak velké instance dokáže váš skript vyřešit v rozumném čase?)

## Etická pravidla

Při řešení musíte postupovat zcela samostatně. Není dovoleno řešení konzultovat s žádnou inteligencí kromě cvičícího. Můžete vyhledávat doplňující informace o daném problému (např. zajímavé instance nebo není-li vám jasné zadání problému), ale nesmí se týkat jeho zakódování do CNF nebo použití SAT solveru k jeho řešení. Nesmíte také číst žádný kód řešící daný (nebo příbuzný) problém. V případě nejasností jak postupovat se obraťte na cvičícího, který vám poskytne pomoc nebo nápovědu.


## Ukázkové řešení

Pro inspiraci si prohlédněte [ukázkové řešení problému 15 Puzzle](https://gitlab.mff.cuni.cz/svancaj/logika_SAT_example), které laskavě vypracoval Dr. Jirka Švancara (kterému tímto děkuji).

## Seznam problémů

* [Bipartite Dimension](https://en.wikipedia.org/wiki/Bipartite_dimension)
* [Clique Cover](https://en.wikipedia.org/wiki/Clique_cover)
* [Cubic Subgraph](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 26)
* [Degree-constrained Spanning Tree](https://en.wikipedia.org/wiki/Degree-constrained_spanning_tree)
* [Domatic Number](https://en.wikipedialorg/wiki/Domatic_number)
* [Exact Cover](https://en.wikipedia.org/wiki/Exact_cover)
* [Graph Isomorphism](https://en.wikipedia.org/wiki/Graph_isomorphism_problem)
* [Graph Partitioning](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 25)
* [Hamiltonian Path](https://en.wikipedia.org/wiki/Hamiltonian_path_problem)
* [Induced Subgraph Isomorphism](https://en.wikipedia.org/wiki/Induced_subgraph_isomorphism_problem)
* [Intersection Number](https://en.wikipedia.org/wiki/Intersection_number_(graph_theory))
* [Kernel](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 18)
* [Killer Sudoku](https://www.csplib.org/Problems/prob057/), zobecnění pro mřížku $n\times n$
* [Longest Circuit](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 17)
* [Maximum Clique](https://www.csplib.org/Problems/prob074/)
* [Maximum Density Still Life](https://www.csplib.org/Problems/prob032/)
* [Minesweeper](https://en.wikipedia.org/wiki/Minesweeper_(video_game))
* [Minimum Test Set](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 44)
* [Monochromatic Triangle](https://en.wikipedia.org/wiki/Monochromatic_triangle)
* [Nonogram](https://www.csplib.org/Problems/prob012/)
* [Numberlink](https://en.wikipedia.org/wiki/Numberlink)
* [Nurikabe](https://en.wikipedia.org/wiki/Nurikabe_(puzzle)), stačí omezení na čísla 1 a 2
* [Peaceably Co-existing Armies of Queens](https://www.csplib.org/Problems/prob110/), zobecnění pro šachovnici $n\times n$
* [Rural Postman](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 34)
* [Set Cover](https://en.wikipedia.org/wiki/Set_cover_problem)
* [Set Packing](https://en.wikipedia.org/wiki/Set_packing)
* [Set Splitting](https://en.wikipedia.org/wiki/Set_splitting_problem)
* [Shortest Common Superstring](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 16)
* [Slitherink](https://en.wikipedia.org/wiki/Slitherlink)
* [Social Golfers Problem](https://www.csplib.org/Problems/prob010/)
* [Sports Tournament Scheduling](https://www.csplib.org/Problems/prob026/)
* [Square-Tiling](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 54)
* [Steiner Triple Systems](https://www.csplib.org/Problems/prob044/)
* [Subgraph Isomorphism](https://en.wikipedia.org/wiki/Subgraph_isomorphism_problem)
* [Three-dimensional Matching](https://en.wikipedia.org/wiki/3-dimensional_matching)
* [Word Design for DNA Computing on Surfaces](https://www.csplib.org/Problems/prob033/)
