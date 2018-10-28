# McKinsey Analytics Online Hackathon 

**Problem Statement**

The client is an insurance company and need a model to: 
- predict clients propensity to pay renewal premium 
- build an incentive plan for its agents to maximise the net revenue 

The client has provided about informations about:
- past transactions from the policy holders along with their demographics 
- aggregated historical transactional data like number of premiums delayed by 3/ 6/ 12 months across all the products 
- number of premiums paid customer 
- sourcing channel 
- customer demographics like age, monthly income and area type

In addition to the information above, the client has provided the following relationships:
- Expected effort in hours put in by an agent for incentives provided 
<a href="http://www.codecogs.com/eqnedit.php?latex=Y&space;=&space;10*(1-exp(-X/400))" target="_blank"><img src="http://latex.codecogs.com/gif.latex?Y&space;=&space;10*(1-exp(-X/400))" title="Y = 10*(1-exp(-X/400))" /></a>
- Expected increase in chances of renewal, given the effort from the agent.

Given the information, the client wants you to predict the propensity of renewal collection and create an incentive plan for agents (at policy level) to maximise the net revenues from these policies.
