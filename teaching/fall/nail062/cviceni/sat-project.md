---
title: NAIL062 Domácí úkol: aplikace SAT solveru"
---

# NAIL062 Domácí úkol: aplikace SAT solveru

Vaším úkolem bude vytvořit systém pro řešení zadaného výpočetního problému za použití SAT solveru. Budeme řešit *rozhodovací problém* (odpověď ano/ne), jde-li o optimalizační problém, řešte jeho rozhodovací variantu: "Má daná instance řešení, jehož objektivní funkce má alespoň/nejvýše danou hodnotu?" 

## Termíny

Neurčí-li váš cvičící jinak:

* vyjádření preferencí případně návrh vlastních problémů k řešení: **do 25. října**
* odevzdání hotového projektu: **do konce listopadu**

## Zásady pro vypracování

K řešení použijte programovací jazyk Python 3 a SAT solver [Glucose 4.2](https://github.com/audemard/glucose/). Nepoužívejte žádné knihovny, které umí převádět formule do CNF apod.

Naprogramujte skript, který:

* na vstupu přijme instanci problému (buď parametry, nebo cestu k souboru popisujícímu instanci, případně kombinaci obojího),
* zakóduje tuto instanci do SAT ve formátu [DIMACS CNF](https://jix.github.io/varisat/manual/0.2.0/formats/dimacs.html),
* zavolá na CNF formuli SAT solver Glucose,
* dekóduje nalezené ohodnocení proměnných (existuje-li) zpět na řešení daného problému,
* toto řešení vypíše v nějakém rozumném, člověkem čitelném formátu.
* Skript navíc volitelně vypíše zkonstruovanou CNF formuli v DIMACS CNF formátu, a statistiky o průběhu řešení SAT solveru.

K řešení přiložte několik instancí, a to alespoň:

* malou, člověkem analyzovatelnou splnitelnou instanci,
* malou, člověkem analyzovatelnou nesplnitelnou instanci (existuje-li),
* splnitelnou instanci, která poběží netriviálně dlouho (alespoň 10s), pokud se Vám ji nepodaří nalézt, popište vaše snažení.

Dále musí být součástí řešení soubor README.md se stručnou dokumentací obsahující:

* přesný popis problému, který řešíte (parametry, rozhodovací proměnné, constrainty, aj.)
* popis Vámi zvoleného zakódování do CNF, případně jeho alternativ
* uživatelská dokumentace vašeho skriptu (vč. popisu formátu vstupu, a také výstupu není-li zřejmý)
* popis přiložených instancí
* popis experimentů, které jste prováděli (např. jak velké instance dokáže váš skript vyřešit v rozumném čase?)

## Etická pravidla

Při řešení musíte postupovat zcela samostatně. Není dovoleno řešení konzultovat s nikým kromě cvičícího an používat nástroje generativní AI. Můžete vyhledávat doplňující informace o daném problému (např. zajímavé instance nebo není-li vám jasné zadání problému), ale nesmí se týkat jeho zakódování do CNF nebo použití SAT solveru k jeho řešení. Nesmíte také číst žádný kód řešící daný (nebo příbuzný) problém. V případě nejasností jak postupovat se obraťte na cvičícího, který vám poskytne pomoc nebo nápovědu.

## Ukázkové řešení

Pro inspiraci si prohlédněte [ukázkové řešení](https://gitlab.mff.cuni.cz/svancaj/logika_SAT_example) ([.zip](https://github.com/jbulin-mff-uk/nail062/raw/main/tutorial/sat-project/logika_SAT_example-master.zip)) problému [15 Puzzle](https://en.wikipedia.org/wiki/15_puzzle), které laskavě vypracoval Dr. Jirka Švancara (kterému tímto děkuji).

## Zadání

Každý student v rámci jedné skupiny cvičení bude řešit jiný problém. Můžete si vybírat ze seznamu níže, nebo i navrhnout vlastní problém, který vás zajímá: V tom případě popište (emailem) o jaký problém jde a proč vás zajímá (podléhá schválení cvičícím, musí být rozumně obtížný — proto raději uveďte i preference problémů ze seznamu).

Neurčí-li váš cvičící jinak:

Vaše preference zadejte v Grupíku jako čísla problémů oddělená čárkami, např. "17,3,21,38". Můžete napsat libovolné množství problémů, dle pořadí preference. V případě, že o váš nejvíce preferovaný problém bude mít zájem více studentů, bude přidělen jednomu náhodně zvolenému, a dále se bude postupovat níže ve vašem seznamu preferencí. Bezproblémovým studentům budou nakonec přiřazeny nepřiřazené problémy náhodně.

## Odevzdání

Neurčí-li váš cvičící jinak:

Hotový projekt odevzdejte v Grupíku jako link na GitHub nebo GitLab repozitář. Repozitář může být buď veřejný, nebo povolte svému cvičícímu přístup.

## Seznam problémů

1. [Bipartite Dimension](https://en.wikipedia.org/wiki/Bipartite_dimension)
2. [Clique Cover](https://en.wikipedia.org/wiki/Clique_cover)
3. [Cubic Subgraph](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 26)
4. [Degree-constrained Spanning Tree](https://en.wikipedia.org/wiki/Degree-constrained_spanning_tree)
5. [Domatic Number](https://en.wikipedia.org/wiki/Domatic_number)
6. [Exact Cover](https://en.wikipedia.org/wiki/Exact_cover)
7. [Garden of Eden](https://conwaylife.com/wiki/Garden_of_Eden)
8. [Graph Isomorphism](https://en.wikipedia.org/wiki/Graph_isomorphism_problem)
9. [Graph Partitioning](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 25)
10. [Hamiltonian Path](https://en.wikipedia.org/wiki/Hamiltonian_path_problem)
11. [Hitori](https://en.wikipedia.org/wiki/Hitori)
12. [Induced Subgraph Isomorphism](https://en.wikipedia.org/wiki/Induced_subgraph_isomorphism_problem)
13. [Intersection Number](https://en.wikipedia.org/wiki/Intersection_number_(graph_theory))
14. [Kernel](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 18)
15. [Killer Sudoku](https://www.csplib.org/Problems/prob057/), zobecnění pro mřížku $n\times n$ (kde $n$ je čtverec)
16. [Longest Circuit](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 17)
17. [Maximum Clique](https://www.csplib.org/Problems/prob074/)
18. [Maximum Density Still Life](https://www.csplib.org/Problems/prob032/)
19. [Minesweeper](https://en.wikipedia.org/wiki/Minesweeper_(video_game))
20. [Minimum Test Set](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 44)
21. [Monochromatic Triangle](https://en.wikipedia.org/wiki/Monochromatic_triangle)
22. [Nonogram](https://www.csplib.org/Problems/prob012/)
23. [Numberlink](https://en.wikipedia.org/wiki/Numberlink)
24. [Nurikabe](https://en.wikipedia.org/wiki/Nurikabe_(puzzle)), stačí omezení na čísla 1 a 2
25. [Peaceably Co-existing Armies of Queens](https://www.csplib.org/Problems/prob110/), zobecnění pro šachovnici $n\times n$
26. [Rural Postman](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 34)
27. [Set Cover](https://en.wikipedia.org/wiki/Set_cover_problem)
28. [Set Packing](https://en.wikipedia.org/wiki/Set_packing)
29. [Set Splitting](https://en.wikipedia.org/wiki/Set_splitting_problem)
30. [Shortest Common Superstring](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 16)
31. [Slitherink](https://en.wikipedia.org/wiki/Slitherlink)
32. [Social Golfers Problem](https://www.csplib.org/Problems/prob010/)
33. [Sports Tournament Scheduling](https://www.csplib.org/Problems/prob026/)
34. [Square-Tiling](https://cgi.csc.liv.ac.uk/~ped/teachadmin/COMP202/annotated_np.html) (problém č. 54)
35. [Steiner Triple Systems](https://www.csplib.org/Problems/prob044/)
36. [Subgraph Isomorphism](https://en.wikipedia.org/wiki/Subgraph_isomorphism_problem)
37. [Three-dimensional Matching](https://en.wikipedia.org/wiki/3-dimensional_matching)
38. [Word Design for DNA Computing on Surfaces](https://www.csplib.org/Problems/prob033/)
