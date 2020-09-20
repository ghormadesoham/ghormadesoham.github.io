---
layout: post
title: 'Reinforcement Learning'
---

May – July 2020

- I learnt about the concepts and applications of reinforcement learning in the projects for this <a href="https://omscs.gatech.edu/cs-7642-reinforcement-learning" target="_blank"> class</a>.

- Specifically, I learnt how to :
    <ul>
    <li> apply tabular methods to discrete space problems,</li>
    <li> apply continuous methods to continuous space problems, </li>
    <li> study and understand game theory concepts,</li>
    <li> learn about solutions to solving Partially Observable Markov Decision Processes (POMDPs) and </li>
    <li> replicate results from research papers when details are left out.</li>
    </ul>

- **Tools used**: Python, <a href="https://gym.openai.com/" target="_blank"> OpenAIGym</a>

- **Methods used**
    <ul>
        <li>Temporal Difference methods
            <ul>TD(λ), Q-Learning, SARSA </ul>
        </li>
        <li>Approximate Methods
            <ul>Deep Q-Learning using Neural Networks i.e. <a href="https://deepmind.com/research/publications/human-level-control-through-deep-reinforcement-learning" target="_blank"> DQN </a> </ul>  
        </li>          
        <li> Game theory concepts 
            <ul>Nash equilibrium, Folk Theorem, Subgame Perfect, Friend-Foe Q,COCO, Correlated Equilibrium. </ul>
        </li>
    </ul>

**Selected Results**    
{% include image_plain.html image="projects/proj-6/Figure_4.png" %}

**Figure 1**: TD:The intermediate values of λ < 1 do better than TD(1). In
particular, TD(1) continues to perform poorly as seen in the
previous experiment. Amongst TD methods, lower values of
λ like 0 and 0.3 do better than higher values like 0.8.

{% include image_plain.html image="projects/proj-6/LunarLander-v2500_24_tune_epsilon_decay.png" %}
**Figure 2**: DQN:HP tuning for Lunar Lander:A smaller value of ε-decay = 0.05 allows the agent to balance exploration and exploitation better than other
values in the range of available values.

{% include image_plain.html image="projects/proj-6/Foe-Q.png" %}

**Figure 3**:Linear Programming: For the game of Soccer(two player, zero-sum, repeated game with imperfect information.) Foe-Q <a href="http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.589.8571&rep=rep1&type=pdf" target="_blank"> algorithm</a>  converges within 5 x 10<sup>5</sup> episodes.

