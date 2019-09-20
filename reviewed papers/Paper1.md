
# Demand Response for Home Energy Management using Reinforcement learning and Artificial Neural Network 

## Author: Renzhi Lu 
## Publisher: IEEE Transactions on Smart Grid 
******
**Summary** 

Renzhi Lu et al (2019) has proposed an hour-ahead reinforcement learning based demand response algorithm for Home Energy Management System to minimize the user energy bill and the degree of discomfort. In the proposed method, ANN based model is used to forecast the price and on top of that a multi-agent RL algorithm is chosen to make optimal decisions for different appliances. The electricity costs of two different cases without and with RL based demand response are compared in this paper, the latter case is found to be significantly cost-effective. 

**Demand Response Management** 

The AI technique can enhance the management of demand response. Model free learning such as Q learing is used to tackle such situation. Because in model free learing, the agent does not need to rely on past data, it learns through trial & errors. 


**Problems Formulation**

They considered the home equipped with various loads which is remarkable. As different kinds of loads can have different effect depending on how its managed. Therefore, it is important to take note of the various loads and classify it to manage them in different orders. They typically classifieds the loads in three kinds. 

1. Non-shiftable Load

Basically the non-shiftable loads are the refrigerators, fire alarm, lights etc. Since once the non-shiftable loads start operation, it needs to be operated continously. Therefore, in this case, the energy cosumed by non-shiftable loads are equal to the energy demand. 

2. Shiftable Load

Shiftable loads such as washing machine, dryer etc. are that can be shifted to operate during the off-peak hour to reduce the cost. 

3. Controllable load 

The example of controlable loads can be air conditioner. It can be controlled to reduce the power consumtion during the peak hour, however it could create a problem such as uncomfortness of the users. 

*The scope for reducing energy bill for the controllable load are highly limited due to the fact that user's satisfaction should be ensured when managing its demand. Therefore, it may need more in depth analysis to create a optimal situation as compared to this paper. Although they mentioned about an objective function that minimize the dissatisfaction cost.*

**Methodology**

1. Use of ANN for price forecasting 

In here they used hour-ahead price data to predict the prices of electricity.

2. On top of that, they used multi-agent RL 

They considered each loads as an individiual agent and each agent maintauns its each own q value. After the Q value is stored and updated from each policy, Q value eventually converges to the maximum value. 

**Novelty**

They used multi-agent reinforement learning for the decision making whereas several others works are done by only using single agent.  

*How about using deep multi-level RL?*

**Improvement**

1. Time of use (ToU) prices could be taken into consideration to make it more sophisticated model which can effect the performance of the agent. 

1. Smart grid can be taken into consideration for more futuristic model. PV and solar energy can be considered. 

2. deep multi-agent Rl can be used for more complicated scenarios 

