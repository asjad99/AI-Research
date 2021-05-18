Build general purpose Intelligent Agents capable of sensing, learning, reasoning and acting in complex enviornments.

Definition of intelligent Agent: 

   - Agents/Systems that can reach their goals in a variety of different (complex/stochastic)environments 


Interesting Papers: 

   - An Approximation of the Universal Intelligence Measure
   - 70 definitions of intelligence 





Ideas Behind the Success of Above systems:


Reinforcement Learning
    - The framework that researchers working on general AI think is reinforcement learning
    - its action reward loop where the agent is constantly interacting with the environment 


Deep Learning 

Attention: 

Need attention model to select or ignore certain inputs Human exercises great attention capability – the ability to filter out unimportant noises ­ Foveating & saccadic eye movement In life, events are not linear but interleaving. Pooling (as in CNN) is also a kind of attention Routing (as in CapsNet) is another example.


https://distill.pub/2016/augmented-rnns/



(Episodic and Working) Memory: 

Attention based memory can be used to augment neural networks to support few-shot learning, rapid adaptability and more generally to support non-parametric extensions.

Short-term/working (temporary storage) 
Episodic (events happened at specific time) 
Long-term/semantic (facts, objects, relations) 
Procedural (sequence of actions)

LSTMs and MANNs


Interesting Papers: 

    1. Using Fast Weights to Attend to the Recent Past (Ba & Hinton, 2016), Hebbian learning with fast synapse plasticity. Related to Hypernetworks.
    2. Hybrid computing using a neural network with dynamic external memory (DeepMind, 2016), role of external memory. Early version: Neural Turing machine (2014).
    3. Ask me anything: dynamic memory networks (ICML, 2016), a cool way to do question answering using memory
    4. End-to-end memory networks (NIPS, 2015), role of memory


Self-Play

https://blog.openai.com/competitive-self-play/


Challenges that still remain: 


![source: agi.mit.edu - Lecture 1](https://d2mxuefqeaa7sj.cloudfront.net/s_F651687F06B7CF24A31D9979C63B8B6B371986087EA14C0BE1407DC4CF82DF43_1529481709517_Screen+Shot+2018-06-20+at+6.00.57+pm.png)





Promising Ideas:
Continual Learning 

https://deepmind.com/blog/enabling-continual-learning-in-neural-networks/ 

Interesting Papers:

1. Progressive neural networks (2016),
2.  curriculumn learning (ICML, 2009), 
3. learning to start "small" (1992)


Reasoning: 

https://deepmind.com/blog/neural-approach-relational-reasoning/
https://deepmind.com/blog/imagine-creating-new-visual-concepts-recombining-familiar-ones/

MANN: examples Memory networks of Facebook: (Weston et al, Facebook, 2015); (Sukhbaatar et al, 2015) – associative memory Dynamic memory networks of MetaMind: (Kumar et al, 2015) – episodic memory Neural Turing machine and Differential Neural Computer of DeepMind (Graves et al. 2014, 2016) -- tape

Imagination: https://deepmind.com/blog/agents-imagine-and-plan/


Meta-learning: Meta-Learning with Memory-Augmented Neural Networks (ICML, 2016)

GAN/VAE/Implicit models

1. Wasserstein GAN (ICML, 2017), a key development of GAN. It's improved version (ICML, 2017).
2. Generative Adversarial Nets (NIPS, 2014), a totally new way of generating high quality data
3. Variational Auto-Encoders (NIPS, 2014), a new powerful way to learn a generative model
4. A list compiled by Dustin Tran (2017)
Experiments: 

Until Recently It was quite tricky to reproduce the results they achieved but OpenAI has known-good implementations (and best practices for creating them). 
https://blog.openai.com/openai-baselines-dqn/

OpenAI realised the need for  for better benchmarks and that RL research was being slowed downed Lack of standardization of environments used in publications. Hence they launched openAI GYM:  https://gym.openai.com/


 https://arxiv.org/abs/1704.04651 
DisTraL: Robust multitask reinforcement learning
https://arxiv.org/abs/1707.04175 


---------------

#### Talks: 

  - [Can the brain do backprop](https://youtu.be/VIRCybGgHts) 
  - [2015 Lecture of DeepMind and its mission](https://youtu.be/0X-NdPtFKq0)
