**Reinforcement Learning**

Reinforcement learning is an autonomous, self-teaching system that essentially learns by trial and error. It performs actions with the aim of maximizing rewards, or in other words, it is learning by doing in order to achieve the best outcomes. This is like how we learn things like riding a bike where in the beginning we fall off a lot and make too heavy and often erratic moves, but over time we use the feedback of what worked and what didn&#39;t to fine-tune our actions and learn how to ride a bike. The same is true when computers use reinforcement learning, they try different actions, learn from the feedback whether that action delivered a better result, and then reinforce the actions that worked, i.e. reworking and modifying its algorithms autonomously over many iterations until it makes decisions that deliver the best result.

A good example of using reinforcement learning is a robot learning how to walk. The robot first tries a large step forward and falls. The outcome of a fall with that big step is a data point the reinforcement learning system responds to. Since the feedback was negative, a fall, the system adjusts the action to try a smaller step. The robot can move forward. This is an example of reinforcement learning in action.

One of the most fascinating examples of reinforcement learning in action I have seen was when Google&#39;s Deep Mind applied the tool to classic Atari computer games such as Break Out. The goal (or reward) was to maximize the score and the actions were to move the bar at the bottom of the screen to bounce the playing ball back up to break the bricks at the top of the screen. You can watch the video here which shows how, in the beginning, the algorithm is making lots of mistakes but quickly improves to a stage where it would beat even the best human players

**In Theory:**

Reinforcement Learning, known as a semi-supervised learning model in machine learning, is a technique to allow an agent to take actions and interact with an environment to maximize the total rewards. RL is usually modelled as a Markov Decision Process (MDP).

 ![](https://github.com/NitinRajS/ai-in-action/blob/master/Reinforcement%20Learning/images/RL_Basic.png)

**Practical Applications of Reinforcement Learning**

**Manufacturing**

In Fanuc, robot uses deep reinforcement learning to pick a device from one box and putting it in a container. Whether it succeeds or fails, it memorizes the object and gains knowledge and train&#39;s itself to do this job with great speed and precision

 ![](https://github.com/NitinRajS/ai-in-action/blob/master/Reinforcement%20Learning/images/Manufacturing.png)

**Finance Sector**

[Pit.AI](http://pit.ai/) is at the forefront leveraging reinforcement learning for evaluating trading strategies. It is turning out to be a robust tool for training systems to optimize financial objectives.

**Traffic Light Control**

In the paper &quot; **Reinforcement learning-based multi-agent system for network traffic signal control**&quot;, researchers tried to design a traffic light controller to solve the congestion problem. Tested only on simulated environment though, their methods showed superior results than traditional methods and shed a light on the potential uses of multi-agent RL in designing traffic system.

 ![](https://github.com/NitinRajS/ai-in-action/blob/master/Reinforcement%20Learning/images/Traffic_Light_Control.png)

Five agents were put in the five-intersection traffic network, with a RL agent at the central intersection to control traffic signalling. The state was defined as eight-dimensional vector with each element representing the relative traffic flow of each lane. Eight choices were available to the agent, each representing a phase combination, and the reward function was defined as reduction in delay compared with previous time step. The authors used DQN to learn the Q value of the {state, action} pairs.

**Games**

Reinforcement Learning is so well-known these days because it is the mainstream algorithm used to solve different games and sometimes achieve super-human performance.

The most famous one must be AlphaGo and AlphaGo Zero. AlphaGo, trained with countless human games, already achieved super-human performance by using value network and Monte Carlo tree search (MCTS) in its policy network. Yet, the researchers later thought back and tried a purer RL approach — train it from scratch. The researchers let the new agent, AlphaGo Zero, played with itself and finally beat AlphaGo 100–0.

**Text, speech, and dialog systems**

Companies collect a lot of text, and good tools that can help unlock unstructured text will find users. Earlier this year, AI researchers at SalesForce used deep RL for abstractive text summarization (a technique for automatically generating summaries from text based on content &quot;abstracted&quot; from some original text document). This could be an area where RL-based tools gain new users, as many companies need better text mining solutions.

RL is also being used to allow dialog systems (i.e., chatbots) to learn from user interactions and thus help them improve over time (many enterprise chatbots currently rely on decision trees). This is an active area of research and VC investments: see Semantic Machines and VocalIQ—acquired by Apple.

**Media and advertising**

Microsoft recently described an internal system called Decision Service that has since been made available on Azure. This paper describes applications of Decision Service to content recommendation and advertising. Decision Service more generally targets machine learning products that suffer from failure modes including &quot;_feedback loops and bias, distributed data collection, changes in the environment, and weak monitoring and debugging_&quot;.

Other applications of RL include cross-channel marketing optimization and real time bidding systems for online display advertising.

**Training Driverless Car using Reinforcement Learning**

_By 2040, 95% of new vehicles sold will be fully autonomous_

A UK company, Wayve, has designed a first-ever autonomous car that works with the help of reinforcement learning. This approach helped them teach the car how to drive in just 15-20 minutes. The system is powered by a deep neural network that has 4 convolutional layers and 3 fully connected layers. When the car veers off track, a safety driver guides it back. The car is then &quot;rewarded&quot; for learning from that mistake.

 ![](https://github.com/NitinRajS/ai-in-action/blob/master/Reinforcement%20Learning/images/Driverless_Car.png)
The researchers used a popular reinforcement learning algorithm called Deep Deterministic Policy Gradients (DDPG). This helped them solve the task of following the lane in front of the car. The architecture of the algorithm was a deep neural network with 4 convolutional layers and 3 fully connected layers with just under 10,000 parameters. In contrast, other state-of-the-art image classification networks have millions of parameters. Only a single camera was used with the autonomous car to capture the surroundings and to follow the road. All the processing requirements were done in the car on just a single GPU.Of course the trial and error process to train the car&#39;s system did not start on the road (too much of a safety hazard in public), but in Wayve&#39;s workspace. A lot of testing was done in simulated environments to understand the task and fine tune the hyperparameters of the reinforcement learning algorithm.
