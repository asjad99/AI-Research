
## Background 

With the growing importance of data in society and the increasing volume of information, it is crucial for data-intensive computing systems to advance. 

This repo inspired from work being done at stanford's  [Future Data Systems group](http://www.futuredata.io.s3-website-us-west-2.amazonaws.com/) where their mission is to design and build post-database systems that enable next-generation data-intensive applications. This group is part of [stanford Dawn]() whose work inolves democratize AI by making it dramatically easier to build AI-powered applications. 

AI advancement is driven by three factors: algorithmic innovation, data (supervised or interactive environments), and available compute power for training. Compute power is the most quantifiable of these factors, enabling us to measure AI progress. The amount of compute used to train a single model correlates with the power of our best models. The trend shows an increase by roughly a factor of 10 each year, partly driven by custom hardware like GPUs and TPUs, and mainly propelled by researchers finding ways to use more chips in parallel.

Four distinct eras are visible in AI development: before 2012, when using GPUs for ML was uncommon; 2012-2014, when infrastructure to train on multiple GPUs was rare; 2014-2016, when large-scale results used 10-100 GPUs; and 2016-2017, when greater algorithmic parallelism and specialized hardware significantly increased limits for some applications.

The trend may continue as hardware startups develop AI-specific chips that promise increased FLOPS/Watt in the next 1-2 years. Additionally, algorithmic innovations could be combined multiplicatively for further gains. However, cost and physics will eventually limit parallelism and chip efficiency. Although it is uncertain how long the trend will persist, its potential for rapid capability increases highlights the importance of addressing safety and malicious AI use now. OpenAI aims to ensure AI progress benefits humanity, offering various research and engineering roles.

![ai-and-compute-all-2](https://user-images.githubusercontent.com/3470924/118594494-e9f14480-b7ec-11eb-8c31-90e0af92e532.png)

reference: https://openai.com/research/ai-and-compute 

As the significance of data continues to grow in society, it is essential for data-intensive computing systems to adapt accordingly. In Summary:

- Data generation will continue to increase
- Data-driven organizations will become standard practice
- Organizations will understand which data to collect from the outset
- Experiment-driven optimization of operations and design will be incorporated into educational curriculums
- Machine learning will become so user-friendly that average programmers will easily utilize it to build data products
- Domain-specific startups will automate some basic data analysis tasks, addressing particular data challenges
- Data analysis will consider the context in which the data was generated
- Overcoming data challenges and extracting value from data will remain difficult
- Creative business strategies will still rely on human input

<img width="586" alt="Screenshot 2023-05-16 at 8 10 28 pm" src="https://github.com/asjad99/Engineering-Data-Products/assets/3470924/c6a9f137-bb9e-447a-bd32-904c552a0147">



### LifeCycle 
Developing an AI project development life cycle involves five distinct tasks:

-  Data engineering: People responsible for data engineering prepare data
and transform data into formats that other team members can use.
-  Modeling: People assigned to modeling look for patterns in data that can
help a company predict outcomes of various decisions, identify business risks
and opportunities, or determine cause-and-effect relationships.
-  Deployment: People in charge of deployment take a stream of data, combine it
with a model, and test the integration before putting the model into production.
-  Business analysis: Team members responsible for business analysis evaluate a deployed
model’s performance and business value and adjust accordingly to maximize benefit or abandon unproductive models.
-  AI infrastructure: People who work in AI infrastructure build and maintain reliable, fast, secure, and scalable software
systems to help people working in data engineering, modeling, deployment and business analysis.


## Data Engineering: 

With 2,3 trillion gigabytes of data created each day, companies have access to a broad range of information on their users, market and much more.
This Data allows them to constantly improve their product/service. 

- At early stage start-ups: the primary analytic focus is to implement logging, to build ETL processes, to model data and design schemas so data can be tracked and stored. The goal here is focused on building the analytics foundation rather than analysis itself
- At mid-stage growing start-ups: Since the company is growing, the data is probably growing too. The data platform needs to adapt, but with the foundation laid out already, there will be a natural shift to insight generation. Unless the company leverages Data Science for its strategic differentiation to start with, many analytics work are around defining KPI, attributing growth, and finding the next opportunities to grow
- Companies who achieved scale: When the company scales up, data also scales up. It needs to leverage data to create or maintain competitive edge. e.g. Search results need to be better, recommendations need to be more relevant, logistics or operations need to be more efficient — this is the time where specialist like ML engineers, Optimization experts, Experimentation designers can play a huge role in stepping up the game.

Before we can do data science we need to setup the infrastructure

![alt text](images/ml_hierarchy_of_needs.png "Logo Title Text 1")


### Fundamentals 


**Guides on Python Programming**

- How to think like a CS in python
- SCIP in python
- Hitch Hiker's Guide to python
- python env https://jacobian.org/2018/feb/21/python-environment-2018/
- Cheatsheet
- MIT Hacker tools
- [Python is Cool] https://github.com/chiphuyen/python-is-cool
- [Data Algorithms](https://github.com/asjad99/modern_algorithms_toolkit)  


### Data Wrangling Libraries   

Data wrangling is about taking a messy or unrefined source of data and turning it into something useful. 
You begin by seeking out raw data sources and determining their value: How good are they as data sets? 
How relevant are they to your goal? Is there a better source? Once you’ve parsed and cleaned the data so that the data sets are usable, 
you can utilize tools and methods (like Python scripts) to help you analyze them and present your findings in a report. 
This allows you to take data no one would bother looking at and make it both clear and actionable.

Clean and wrangle data into a usable state

> Data engineers make sure the data the organization is using is clean, reliable, and prepped for whatever use cases may present themselves. 
Data engineers wrangle data into a state that can then have queries run against it by data scientists.

> Data Formats should be easy for computers to parse, people to read and widely used by systems in production. 
The computations we perform must be reproducible and tweakable. Data Pipelines need to be documented. 

#### Learning the tools 

| Notebook                 | Description | Code |
|--------------------------|-----------|------|
| Command-line             | Learn various unix command line utlities and how they can be used to clean and compute basic statistics          | [blog_post](https://asjadkhan.ghost.io/ghost/#/site) |     
| Web Data Collection      | Learn to collect data available on web (APIs or web scrapping)          | [Notebook](https://github.com/asjad99/datascience-GYM/tree/master/data_engineering)          |  
| numpy_Basics     | Learn the basics of the library that underpins scientific computing          |[Notebook](/work/datascience-GYM/Data_Munging/[Numpy]basics.ipynb)        | 
| numpy_linear_algebra     |           |Notebook        |     
| Pandas Basics            | Learn the basics of pandas        |[Notebook](https://github.com/asjad99/datascience-GYM/blob/master/Data_Munging/Pandas.ipynb)        |      |


Learn More: 
  - [just-pandas-things](https://github.com/chiphuyen/just-pandas-things)
  - Python for Data Analysis Books 


### Delta Lake: 

- https://github.com/databricks/tech-talks/tree/master/sessions/2020-04-16%20%7C%20Diving%20into%20Delta%20Lake%20-%20DML%20Internals
- https://github.com/databricks/tech-talks/tree/master/sessions/2020-03-26%20%7C%20Diving%20into%20Delta%20Lake%20-%20Unpacking%20the%20Transaction%20Log 
- https://github.com/databricks/tech-talks/tree/master/sessions/2020-04-02%20%7C%20Diving%20into%20Delta%20Lake%20-%20Schema%20Enforcement%20and%20Evolution 

### Big Data Processing: 

Case Study: [Scalable-Topic-Modeling](https://github.com/asjad99/Scalable-Topic-Modeling) - Singular Value Decomposition for Latent Semantic Indexing using PySpark


## Building Training Datasets for ML: 



#### Few old Projects: 


### Data Product - Case Studies: 

1. Fast Forwards Labs
2. Advanced Analytics in Spark 
3. Beautiful Data

