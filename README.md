# McKinsey Analytics Online Hackathon 

This project was part of the McKinsey Analytics Online Hackathon organised in July 2018 on Analytic Vidhya platform.

Private Leaderboard: ranked 56th (score: 0.7926365431)

https://datahack.analyticsvidhya.com/contest/mckinsey-analytics-online-hackathon-4/pvt_lb


**Problem Statement**

The client is an insurance company and need a model to: 
1) predict clients propensity to renew their policy
2) create an incentive plan for agents (at policy level) to maximise the net revenues from these policies.


The client has provided about information about:
- past transactions from the policy holders along with their demographics 
- aggregated historical transactional data like number of premiums delayed by 3/ 6/ 12 months across all the products 
- number of premiums paid customer 
- sourcing channel 
- customer demographics like age, monthly income and area type


The following curve provides the relationship between extra effort in hours invested by the agent with Incentive to the agent and % improvement in renewal probability vs agent effort in hours.

- Relationship between extra efforts in hours invested by an agent and Incentive to agent. After a point more incentives does not convert to extra efforts.

  Equation for the effort-incentives curve:   <a href="http://www.codecogs.com/eqnedit.php?latex=Y&space;=&space;10*(1-exp(-X/400))" target="_blank"><img src="http://latex.codecogs.com/gif.latex?Y&space;=&space;10*(1-exp(-X/400))" title="Y = 10*(1-exp(-X/400))" /></a>

- Relationship between % improvement in renewal probability vs Agent effort in hours. The renewal probability cannot be improved beyond a certain level even with more efforts.

  Equation for the % improvement in renewal prob vs effort curve:   <a href="http://www.codecogs.com/eqnedit.php?latex=Y&space;=&space;20*(1-exp(-X/5))" target="_blank"><img src="http://latex.codecogs.com/gif.latex?Y&space;=&space;20*(1-exp(-X/5))" title="Y = 20*(1-exp(-X/5))" /></a>


