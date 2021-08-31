# Reinforcement-Learning (RL) with OpenAI
The key players of RL are the agent and the environment. The agent lives in the environment and interacts with it.


<p align="center">
  <img width="460" height="300" src="https://user-images.githubusercontent.com/75802671/131371250-4bbf68b6-3f76-4453-b67f-51de153afc49.png">
</p>

### Terminology

- **State (s):** A state is the complete description of the state of the world/environment. No information of the world/environment is hidden from the state

- **Observation (o):** A partial description of a state, which may omit information. A Observation is the answer to the question, what the actions of the agent are doing to the                                environment.

- **Action space:** Set of all valid actions in a given environment.
  - Discrete action space: only a finite number of moves are available to the agent
  - Continuous action space: actions are real-valued vectors 
  - This distinction has some quite-profound consequences for methods in deep RL. Some families of algorithms can only be directly applied in one case and would have to be        substantially reworked for the other.

- **Polices:** A rule used by an agent to decide what actions to take. One can say it is the agent’s brain and tries to maximize the reward.

- **Trajectories/episode (τ):** A sequence of states and actions in the world, τ=(s_0,a_0,s_1,a_1 ).
                                The first state s_0 of the world is randomly sampled. State transitions (what happens to the world between the state at time t, s_t and the state at t+1,                                 s_(t+1)) are governed by the natural laws of the environment and depend on only the most recent action. 
                                A trajectorie/episode is done if the agent for example loses the game he is currrently playing. 

- **Reward (R):** Signal from the environment, a number that tells it how good or bad the current world state is. The goal of the agent is to maximize its cumulative reward, called                       return.


### Sources: 
- https://spinningup.openai.com/en/latest/spinningup/rl_intro.html
- https://gym.openai.com/docs/

