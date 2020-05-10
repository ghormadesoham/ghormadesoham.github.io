---
layout: post
title: 'Machine Learning'
---

January – April 2020

- I learnt about the concepts and applications of machine learning in the projects for this <a href="https://www.omscs.gatech.edu/cs-7641-machine-learning" target="_blank"> class</a>.

- Specifically, I learnt how to :
    <ul>
    <li> tune parameters for  supervised learning algorithms,</li>

    <li> apply clustering and dimensionality reduction techniques to improve performance for a  chosen metric,</li>

    <li>apply randomized optimization techniques to find solve NP hard problems, and,</li>
    <li> apply fundamental Reinforcement Learning algorithms to solve Markov Decision Process(MDP) problems.</li>

    </ul>

- **Tools used**: Python, sklearn, <a href="https://gym.openai.com/" target="_blank"> OpenAIGym</a>, <a href="https://pymdptoolbox.readthedocs.io/en/latest/api/mdptoolbox.html" target="_blank"> MDPToolbox</a>, <a href="https://mlrose.readthedocs.io/en/stable/" target="_blank"> MLROSE</a>
- **Algorithms used**
    <ul>
        <li>Supervised Learning
            <ul>Decision Trees, Support Vector Machines, Artificial Neural Networks</ul>
        </li>
        <li>Unsupervised Learning
            <ul>K-Means, Expectation Maximization, Principal Component Analysis(PCA), Independent Component Analysis(ICA), hill climbing, simulated annealing, genetic algorithms </ul>  
        </li>          
        <li>Reinforcement Learning
            <ul>Policy and Value Iteration, Q-Learning </ul>
        </li>
    </ul>

**Selected Results**    
{% include image_plain.html image="projects/proj-5/diabetes average_precision.png" %}

**Figure 1**: Comparision of Area under Precision recall curve of supervised learning algorithms. Area under Precision recall curve works well for the <a href="http://archive.ics.uci.edu/ml/datasets/Wine/dataset" target="_blank"> wines</a> dataset  which is imbalanced. SVM and Neural Networks perform well in this case. However, Neural Networks take longer to train compared to SVM. Consequently, SVM is the best choice amongst the algorithms available.

{% include image_plain.html image="projects/proj-5/MaxKColor 50 iteration_fitness.png" %}

**Figure 2**: Comparison of randomized optimization algorithms for the Max K Color problem.
Genetic Algorithm converges to a high value of fitness while other algorithms take
longer. MIMIC, notably, converges quickly but to a much lower value of fitness. 

{% include image_plain.html image="projects/proj-5/dim_red.png" %}

**Figure 3**:Learning curve to compare dimensionality reduction algorithms for the  <a href="https://www.kaggle.com/uciml/pima-indians-diabetes-database" target="_blank"> diabetes</a> dataset. PCA has the highest accuracy(74%) compared to other algorithms. The likely explanation is because PCA lowers the number of dimensions to be manageable instead of removing selected features for example. Consequently, the accuracy improves.

{% include image_plain.html image="projects/proj-5/Tune epsilon Reward4x4.png" %}

**Figure 4**:For 16 states, an ε = 0.5 i.e equal amount of exploration and exploitation results in higher
reward(80,000). Notably, only exploration (ε = 1) is not preferred because it results in
relatively smaller value for reward(40,000)