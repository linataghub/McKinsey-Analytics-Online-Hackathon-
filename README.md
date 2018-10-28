# McKinsey Analytics Online Hackathon 

This project was part of the McKinsey Analytics Online Hackathon organised in July 2018 on Analytics Vidhya platform.

Private Leaderboard: Ranked 56th (score: 0.7926365431)

https://datahack.analyticsvidhya.com/contest/mckinsey-analytics-online-hackathon-4/


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


The net revenue across all policies is be calculated in the following manner:

<a href="http://www.codecogs.com/eqnedit.php?latex=Total&space;Net&space;Revenue&space;=&space;\sum&space;((Pbenchmark&space;&plus;&space;\Delta&space;p)*premium&space;-&space;incentive)" target="_blank"><img src="http://latex.codecogs.com/gif.latex?Total&space;Net&space;Revenue&space;=&space;\sum&space;((Pbenchmark&space;&plus;&space;\Delta&space;p)*premium&space;-&space;incentive)" title="Total Net Revenue = \sum ((Pbenchmark + \Delta p)*premium - incentive)" /></a>

<a href="http://www.codecogs.com/eqnedit.php?latex=Pbenchmark" target="_blank"><img src="http://latex.codecogs.com/gif.latex?Pbenchmark" title="Pbenchmark" /></a> is the renewal probability predicted using a benchmark model by the insurance company.
<a href="http://www.codecogs.com/eqnedit.php?latex=\Delta&space;p" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\Delta&space;p" title="\Delta p" /></a> is the improvement in renewal probability calculated from the agent efforts in hours.
<a href="http://www.codecogs.com/eqnedit.php?latex=premium" target="_blank"><img src="http://latex.codecogs.com/gif.latex?premium" title="premium" /></a> is the premium paid by the policy holder for the policy in consideration
<a href="http://www.codecogs.com/eqnedit.php?latex=incentive" target="_blank"><img src="http://latex.codecogs.com/gif.latex?incentive" title="incentive" /></a> is the incentive given to the agent for increasing the chance of renewal (estimated by the participant) for each policy

The following equations provide the relationship between extra effort in hours invested by the agent with Incentive to the agent and % improvement in renewal probability vs agent effort in hours.

- Relationship between extra efforts in hours invested by an agent and Incentive to agent. After a point more incentives does not convert to extra efforts.

  Equation for the effort-incentives curve:   <a href="http://www.codecogs.com/eqnedit.php?latex=Y&space;=&space;10*(1-exp(-X/400))" target="_blank"><img src="http://latex.codecogs.com/gif.latex?Y&space;=&space;10*(1-exp(-X/400))" title="Y = 10*(1-exp(-X/400))" /></a>

- Relationship between % improvement in renewal probability vs Agent effort in hours. The renewal probability cannot be improved beyond a certain level even with more efforts.

  Equation for the % improvement in renewal prob vs effort curve:   <a href="http://www.codecogs.com/eqnedit.php?latex=Y&space;=&space;20*(1-exp(-X/5))" target="_blank"><img src="http://latex.codecogs.com/gif.latex?Y&space;=&space;20*(1-exp(-X/5))" title="Y = 20*(1-exp(-X/5))" /></a>


