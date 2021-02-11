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



## Simulation Results

- Developed algorithm boosts the sum-rate in a practical downlink scenario by over 70%




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


