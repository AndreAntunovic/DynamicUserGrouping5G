# Dynamic Sectorization in Multi-Panel Massive MIMO Systems
Dynamic user grouping in multi-panel massive MIMO scenario for 5G networks. 
Since a paper is currently in work for this research project, the full ReadMe will not be published until after the publication of the paper.

## Dynamic User-Grouping in MU-MIMO  - Scenario 

- Investigation of a multi-panel base transceiver station (BTS) architecture for the realization of a massive MIMO system
- Opposite to conventional massive MIMO with a single BTS, where many antennas are co-located in one single large panel, it is assumed distributing the antennas into multiple panels to be more cost-efficient for future communication standards
- A big challenge is to find good associations, in the sense of best possible spectral efficiency, of users and panels by the realization of a dynamic sectorization with user-centric virtual cells for the multi-panel BTS
- The different BTSs are assumed to be connected to central processing and therefore to be jointly processable 
- Throughout the work joint precoding of all panels as done in a conventional massive MIMO system will serve as a comparable scheme
- It is aimed to dynamically choose the partition which leads to the best Downlink spectral efficiency
- The precoders are assumed to be Matched Filter precoders, as it is the handiest of the standard precoders and the focus of the work is on the sectorization aspect. Other precoders certainly have the potential to further boost performance

![Farmers Market Finder Demo](ImagesDynamicSec/Scenario.gif)


## Approaching the problem via discrete mathematical optimisation by use of the Stirling Numbers

### Relation to Bipartite Graphs
- A graph H is bipartite if its nodes can be partitioned into two sets 𝑉<sub>1</sub>, 𝑉<sub>2</sub> so that every edge joins a node in V<sub>1</sub> to a node in V<sub>2</sub>
- Bipartite graphs only contain cycles of even length
- Adapting the given problem to graph theory, the channel matrix  translates to the graph and the panels and users can be described as the sets of nodes V<sub>1</sub> and V<sub>2</sub>  
- Partitioning a bipartite graph is an equivalent problem to sectorizing the panels and users in a Multi-Panel MIMO system



![Farmers Market Finder Demo](ImagesDynamicSec/IP.gif)

<!---

### Exploiting the Stirling Numbers of the second kind to simplify the IP structure

- On one side of the bipartite graph only eight nodes are representing the panels
- Sticking to the IP problem which is to be solved, the number of partitions needs to be fixed
- Reconsidering the placement of the panels (around the edges of a building), four partitions seem to be reasonable out of a geometric point of view, which leads to a total of only 1701 possibilities of partitioning the eight panels
- Since there shouldn‘t be one division that is much bigger than the others some sorts of divisions were excluded which leads to a further reduction of the number of possibilities after the exclusion


![Farmers Market Finder Demo](ImagesDynamicSec/IP2Stirling.gif)


## Local Movebased Heuristic helps to further improve the results

- Nodes are partitioned according to the best IP solution
- Throughout the iterations the users are selected in an arbitrary order and put into all possible partitions. For each possibility, the spectral efficiency is calculated and the user is locked to the partition for which the spectral efficiency is maximal. 
- If the spectral efficiency is maximal for more than one possible partition or even equal for all possibilities, the user is placed arbitrarily in one partition
- After all nodes are locked, the change in the result value is checked. If the completed iteration increases the value of the spectral efficiency, a new iteration starts by configuring the initial state with the best found in the previous iteration. Otherwise, iterations end and the best solution is returned 
- Throughout the whole process the division into partitions on the panel side remains unchanged


![Farmers Market Finder Demo](ImagesDynamicSec/MoveBased.gif) 

--->


## Simulation Results

- Combination of IP based and greedy algorithm boosts the rate by over 70%




<!---  
- IP solution itself increases the spectral efficiency by over 30 % 
- Combination of IP solution and movebased heuristic boosts the performance by over 70%
![Dynamic](ImagesDynamicSec/SimulationResults.png) 
---> 

## References

[1] R. SCHOBER: Script of the Lecture MIMO Communication Systems. Friedrich-Alexander-University Erlangen-Nürnberg,Institute for Digital Communications

[2] F. LIERS: Script of the Lecture Mathematical Optimization for Communications and Signal Processing. Friedrich-Alexander University Erlangen-Nürnberg, Department for applied Mathematics

[3] HUANG, Yi, et al. “Multi-panel MIMO in 5G.“ IEEE Communciations Magazine 56.3 (2018): 56-61

[4] OMEROGLU, Nurettin B., et al. “K-partitioning of signed or weighted bipartite graphs.“ 2013 International Conference on Social Computing. IEEE, 2013

[5] ZHA, Hongyuan, et al. “Bipartite graph partitioning and data clustering.“ Proceedings of the tenth international conference on information and knowledge management. ACM, 2001

[6] D.E. Knuth, „The Art of Computer Programming“, Vol. 1., Second edition, Addison-Wesley, Reading, Mass., 1973. 

[7] D.E. Knuth, „The Art of Computer Programming“, Vol. 2., Secondcdilion, Addison-Wesley, Reading, Mass., 1981. 


