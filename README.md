Since a paper is currently in work for this research project, the full ReadMe will not be published until after the publication of the final paper.

# Dynamic Sectorization in Multi-Panel Massive MIMO Systems
- Dynamic user grouping in multi-panel massive MIMO scenario for 5G networks. 

## Scenario 

- Investigation of a multi-panel base transceiver station (BTS) architecture for the realization of a massive MIMO system for 5G / Beyond 5G
- Opposite to conventional massive MIMO with a single BTS, where many antennas are co-located in one single large panel, it is assumed distributing the antennas into multiple panels to be more cost-efficient for future communication standards
- A big challenge is to find good associations, in the sense of best possible spectral efficiency, of users and panels by the realization of a dynamic sectorization with user-centric virtual cells for the multi-panel BTS
- The different BTSs are assumed to be connected to central processing and therefore to be jointly processable 
- Throughout the work joint precoding of all panels as done in a conventional massive MIMO system will serve as a comparable scheme
- It is aimed to dynamically choose the partition which leads to the best Downlink spectral efficiency
- The precoders are assumed to be Matched Filter precoders, as it is the handiest of the standard precoders and the focus of the work is on the sectorization aspect. Other precoders certainly have the potential to further boost performance

![Farmers Market Finder Demo](ImagesDynamicSec/scenario.gif)


## Simulation Results

- Developed algorithm boosts the sum-rate in a practical downlink scenario by over 70%
