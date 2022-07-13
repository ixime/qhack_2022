# qhack_2022
## Open Hackaton project

This repo contains my project in the qhack_2022. 

### Goal

Explore quantum approaches for dynamic bayesian network structure learning (DBNSL) with generated data and real data [2].  

### Intro

DBNSL's main goal is to obtain P(G|D), that means obtaining a direct acyclic graph (DAG) given a dataset consisiting of at least two events or moments in time. This solution can be applied to solve problems in different fields, like finance, biology and ecology to name a few. This kind of problem is super-exponential (O(n! 2^(n!/(2!(n-2)!)))) [1] due to a search over all DAGs possible. I reviewed different approaches, and I decided to implement three different approaches:

   - Hybrid network = (classic) encoder + (quantum) circuit.
   - Variational circuit
   - Quantum circuit structure learning

The first step is to implement these approaches with a tiny dummy dataset of 4 variables (8 nodes) and if I get the AWS credits, implement them with a real dataset of microarray studies on cell cycle regulated genes.

### References:

[1] Prashant S. Emani1, et al, Quantum Computing at the Frontiers of Biological Sciences

[2] [Spellman PT, Sherlock G, et al, Comprehensive identification of cell cycle-regulated genes of the yeast Saccharomyces cerevisiae by microarray hybridization](https://www.ebi.ac.uk/biostudies/studies/S-EPMC25624)
