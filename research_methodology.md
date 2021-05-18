## How to conduct research? 

![https://anatomyof.ai/](https://paper-attachments.dropbox.com/s_D1A960734D0D7CAB48E833F866248DD4620C386C6B0485DEE7BAA389AE9734ED_1550146865187_image.png)



   In my opinion, the most important aspect of computer science is algorithmic thinking. By “algorithmic thinking,” I mean the crisp definition of a problem, and the deliberate decomposition of a potential solution into a series of well-defined steps. Algorithmic thinking is useful for everyone, not just computer scientists, because everyone will encounter problems in their lives, and everyone will want to devise good solutions for those problems. Algorithmic thinking forces people to be explicit about their assumptions and their goals; clarity of thought results in better solutions! -James Mickens



### Philosophy of PhD

You are responsible for pushing the boundaries of a tiny sub-field of human knowledge
 

- You Hold a Tiny Area of Human Knowledge 
- You are the expert in that sub-field 
- You regularly push the boundaries/understanding of that area by 
- You communicate your findings via research papers
- Which entails You must know how to conduct Scientific Research,Formulate problems formally, Solve Problems, Do Experiments, Know statistics, present findings   
- In Practice, To progress in career folks find areas that few people care about or do variations - this gives them good careers and they can hence pay bills etc. 


Richard Hamming 10 RULES: https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.0030213 


### How to write a paper - lessons learned
 
 
 
"When you understand that nobody wants to read your shit, your mind becomes powerfully concentrated. 
You begin to understand that writing/reading is, above all, a transaction. 
The reader donates his time and attention, which are supremely valuable commodities. In return, you the writer must give him something worthy of his gift to you.” 
— Steven Pressfield



Abstract
 

1. Introduction (why they should read your paper)


    1. What is the problem you are trying to solve
    2. why is it important
    3. what has already been done(2-3 references)
    4. Shortcomings of existing techniques
    5. What do you propose
    6. Results (maybe)
    7. Structure of paper  


2. Background
    1. Give a short tutorial of stuff needed to understand the paper
3. Methodology
    1. Innovations
    2. some equations
4. Experiments
    1. Setup
    2. Comments on graphs 


talk: https://youtu.be/1AYxMbYZQ1Y


-----

### Research in RL 


Frame 1: Improving on an Existing Approach. This is the incrementalist angle, where you try to get performance gains in an established problem setting by tweaking an existing algorithm. Reimplementing prior work is super helpful here, because it exposes you to the ways that existing algorithms are brittle and could be improved. A novice will find this the most accessible frame, but it can also be worthwhile for researchers at any level of experience. While some researchers find incrementalism less exciting, some of the most impressive achievements in machine learning have come from work of this nature.
Because projects like these are tied to existing methods, they are by nature narrowly scoped and can wrap up quickly (a few months), which may be desirable (especially when starting out as a researcher). But this also sets up the risks: it’s possible that the tweaks you have in mind for an algorithm may fail to improve it, in which case, unless you come up with more tweaks, the project is just over and you have no clear signal on what to do next.

Frame 2: Focusing on Unsolved Benchmarks. Instead of thinking about how to improve an existing method, you aim to succeed on a task that no one has solved before. For example: achieving perfect generalization from training levels to test levels in the Sonic domain or Gym Retro. When you hammer away at an unsolved task, you might try a wide variety of methods, including prior approaches and new ones that you invent for the project. It is possible for a novice to approch this kind of problem, but there will be a steeper learning curve.
Projects in this frame have a broad scope and can go on for a while (several months to a year-plus). The main risk is that the benchmark is unsolvable without a substantial breakthrough, meaning that it would be easy to spend a lot of time without making any progress on it. But even if a project like this fails, it often leads the researcher to many new insights that become fertile soil for the next project.

Frame 3: Create a New Problem Setting. Instead of thinking about existing methods or current grand challenges, think of an entirely different conceptual problem that hasn’t been studied yet. Then, figure out how to make progress on it. For projects along these lines, a standard benchmark probably doesn’t exist yet, and you will have to design one. This can be a huge challenge, but it’s worth embracing—great benchmarks move the whole field forward.
Problems in this frame come up when they come up—it’s hard to go looking for them.
Avoid reinventing the wheel. When you come up with a good idea that you want to start testing, that’s great! But while you’re still in the early stages with it, do the most thorough check you can to make sure it hasn’t already been done. It can be pretty disheartening to get halfway through a project, and only then discover that there’s already a paper about your idea. It’s especially frustrating when the work is concurrent, which happens from time to time! But don’t let that deter you—and definitely don’t let it motivate you to plant flags with not-quite-finished research and over-claim the merits of the partial work. Do good research and finish out your projects with complete and thorough investigations, because that’s what counts, and by far what matters most in the long run.


----

### A CRASH COURSE IN HOW TO EMPIRICAL RESEARCH

1. Implement things. If you haven't implemented things, start from the bottom and work your way up. My path to my first "New" idea was [MLP on MNIST in MATLAB -> MNIST with MatConvNet (I know, I know) -> bigger VGG-nets with theano/lasagne (resnets weren't out yet otherwise they would be a better choice) -> VAEs in theano/lasagne -> DCGAN came out so I implemented that -> mildly novel VAE/GAN hybrid].
2. While implementing things, pay attention to the details. You will either notice things that are done suboptimally (Why are they using 5x5 filters instead of dilated convs? etc) or come up with ideas for how to do things better (What if I used a convolutional layer where all the weights were made with some sort of tensor product? What if I tweaked the loss function to be smoother here and sharper there?). Try out your ideas.
3. After you try out a lot of ideas, you'll begin to gain intuition and a deeper understanding of the thing you're studying. Think about what it is that you actually want to study--do you care about the underlying task, or what you can learn generally about neural net training by working on this task, or what you can learn about optimization by improving scores there? Is the task or dataset actually the best way to study what you truly want to study, or does the field need a different task or a better dataset to accomplish this?
4. Some of your ideas will work. The vast majority of them will not. Pay attention to both the failures and successes, and think critically about the phenomena underlying each. Why does idea A improve performance while idea B doesn't?
5. After a while you will have more ideas than you have time to implement, and more new knowledge than you have time to write down or space to fit in a paper. Ideally the direction of research you take will mean you have a story to tell--On Task X, method A is dominant. But what happens if we tweak method A / apply method B / modify task X / generally change things up. Or maybe you say, "Everyone is asking question Y. But what if we ask question Z? Or what if we try to get an answer to question Y in this way that hasn't been tried before?" (The Rethinking Generalization paper from ICLR a few years back is a great example of this). A paper is a medium by which you express this knowledge as succinctly and clearly as possible, with supporting empirical evidence.
6. Rinse and repeat. Think about the process, because you will always be able to do it more optimally. Think about research direction, and try and fine-tune your ability to drill into the questions you actually want to answer. For some people this means focusing less on trying to top the leaderboards; for some people, this means focusing more on the best way to top the leaderboards (both can be valid!).

TL;DR: Do stuff, all the time. Always be doing stuff and thinking about the stuff you're doing. Then make tweaks to the stuff, think about those tweaks, and then write them up.

Quick Research: 


- Read 5-6 best papers 
- understand their ideas
- pick something that hasn’t been done before yet is easy to do (some hybrid approach that combines the best of x and y paradigms)
- pick the simplest best execution of idea for this new approach
- write down the core steps 
- add 100 small details to make it look like you have given enough thought

### Asking Good questions

How to Ask Good Questions

1. A good question is energising. It’s an inviting challenge, it’s something that’s interesting and fun to pursue. It inspires a new way of seeing things, a new way of ordering information.
2. A good question is an act of pointing. First you survey the ideascape in front of you – maybe it’s shared territory between the two of you, or maybe it’s you looking over your conversation-partner’s shoulder – and then you try and identify the most compelling, interesting thing, and point to that.
3. “Funny” or “interesting” is a sort of compass or gyroscope that guides you away from stale questions.

### Example of Open Problem in RL 

Following our previous discussions on real world applicability of RL(summarised in this paper https://arxiv.org/pdf/1904.12901.pdf), I spent some time figuring out the most impactful areas of RL. 

I feel like studying the sample efficiency issue of reinforcement learning from multiple aspects is an interesting direction and can have a big impact on making RL mainstream like supervised ML in the long term. 

Here is an interesting talk by Stanford Professor Emma Brunkskill related to this topic: https://www.youtube.com/watch?v=U2wHy7xmx9k

I think this area is rich enough in terms of unsolved problems and can be explored with an opportunity to publish several papers in the long term. 

On a high level there exist various approaches to attack this problem(e.g model-based RL and immitation learning), but for now I'm looking into Efficient Exploration(i.e how can we accelerate the process of Exploration in a new environment?) which seems quite promising.  

After spending time learning the basics I found that few or no people have worked on the problem of applying Transfer Learning(a topic popular in ML community) to the process of exploration so that's one of the main ideas i’m exploring at the moment. Incorporating prior knowledge in exploration was something that was discussed at ICML panel discussion as well https://sites.google.com/view/erl-2018/homewhich gave me some validation that this is indeed the right direction to proceed. 

I don't have a concrete solution yet but ideas on how to approach this. I’ll share some of them once they have taken a bit of shape. 

Regarding the limited time remaining of the scholarship funding, I think basic research with my level of experience is a slow and a time consuming process and RL experiments beyond toy problems are quite tedious(e.g see http://amid.fish/reproducing-deep-rl). So im not sure how can I quickly wrap up things. One option is working on RL applications which is faster if one has the right domain expertise and datasets available. so far I have only looked a little bit into healthcare applications of RL (survey: https://arxiv.org/pdf/1908.08796.pdf). 


#### How to get good at research 

Replicate Papers

[ ] Understand Project goals clearly
[ ] Install the environment and code
[ ] Replicate the experiment to get a sense of time for training
[ ] Understand the core algorithm
[ ] Tinker with the algo. https://www.youtube.com/watch?v=8EcdaCk9KaQ


![image](https://user-images.githubusercontent.com/3470924/118581974-f322e700-b7d5-11eb-94f6-b843adfe7b79.png)

### Resources:
https://people.eecs.berkeley.edu/~pattrsn/talks/BadCareer.pdf
in research ask a research question then learn everything around tht topic
·  kickstart research in CS by Prof Anandhttps://www.youtube.com/watch?v=foflxVMuF6A&list=PLXDX4vxbgW0Cvnf4R9m4Y8Yt9mJqIt-bV
·  How to read a paper by Anaad

https://blog.usejournal.com/advice-on-building-a-machine-learning-career-and-reading-research-papers-by-prof-andrew-ng-f90ac99a0182
Notes on Postmodern Programming
Paul Graham Essays
A Survival Guide to a PhD by Andrej Karpathy
10 Tips for Research and a PhD by Sebastian Ruder
An Opinionated Guide to ML Research by John Schulman
So you want to be a research scientist by Vincent Vanhoucke, aka, how to do modern ML/AI research
Advice for early-stage Ph.D. students by Philip Guo
How to have a good CS career by Stefan Savage
How to do Research At the MIT AI Lab
How to do good (data mining) research, get it published by  Eamonn Keogh
How to Be a Good Graduate Student by Marie desJardins
Advice for researchers and students, compiled by Michael Ernst

·  how to write a paper by Simon Peyton Jones
·  Essay writing by jorden petersonhttps://bigthink.com/personal-growth/jordan-petersons-ten-step-process-for-stronger-writing?rebelltitem=1#rebelltitem1
·  Paul graham: http://www.paulgraham.com/useful.html
·  You and your research by richard hamming
·  Papers we love : https://github.com/papers-we-love/papers-we-love
·  by 2 minute papers ACM and other newsletters
·  https://www.cloudera.com/products/fast-forward-labs-research/fast-forward-labs-research-reports.html
·  https://brendenlake.github.io/CCM-site/
·  https://github.com/sindresorhus/awesome
·  ·  https://dspace.mit.edu/bitstream/handle/1721.1/41487/AI_WP_316.pdf?sequence=4&isAllowed=y
·  Great Readings for Researchers and Scholars
·  Lex fridman AI podcast
·  Escaping the local optimum https://www.youtube.com/watch?v=5qjA8HPJl_0
