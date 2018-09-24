---
layout: about
title: Research
description: >
  Md Mofijul Islam's Research.
hide_description: true
menu: true
order: 3
---
Table of Contents
  * [Artificial Inteligence and Machine learning](#artificial-intelligence-and-machine-learning)
    - [Multi-modal and Multi-task Learning **\[Grant\]**](#multi-modal-and-multi-task-learning)
      - [Transfer Lerning in Visual Question Answering](#transfer-learning-in-visual-question-answering)
    - [Design Optimization and Evolutionary Approches](#design-optimization-and-evolutionary-approaches)
      - [Resource Allocation in Mobile Cloud Computing](#resource-allocation-in-mobile-cloud-computing)
      - [Reduce Overfiting Problem in Deep Learning Models](#reduce-overfitting-problem-in-deep-learning-models)
      - [Optimized Distributed Clustering Model in DSN](#optimized-distributed-clustering-model-in-dsn)
    - [Developer Question Answering and Repository Mining](#developer-question-answering-and-repository-mining)
    - [Interpretable Machine Learning](#interpretable-machine-learning)
  - [Natural Language Processing](#natural-language-processing)
    - [Transfer Learning Approach to Extract Fact and Validate Statement](#transfer-learning-approach-to-extract-fact-and-validate-statement)
    - [Bangla Article Classfication](#bangla-article-classification)
    - [Bangla Speech and Speakers Identification](#bangla-speech-and-speakers-identification)
  * [Computational Biology](#computational-biology)
    - [iProtGly-SS: Identifying Protein Lysine Glycation Sites](#iprotgly-ss-identifying-protein-lysine-glycation-sites)
    - [Identification of Recombination Hotspot in Genome](#identification-of-recombination-hotspot-in-genome)
  * [Big Graph Query and Mining](#big-graph-query-and-mining)

## Artificial Intelligence and Machine Learning
I am mainly working in the intersection of theoretical artificial intelligence and practical machine learning approaches. Currently, I am working to develop some learning models to solve problems in the various domain. As mainly I am involved in the design and developing learning model, I collaborate with several domain experts in different fields. Furthermore, I am interested to design and modify the internal structure of various learning models.

  * ## Multi-modal and Multi-task Learning
    Representation learning is applied in different areas, such as Computer Vision, Natural Language Processing(NLP), Social Network analysis, etc. Most of the representational learning are applied in solving inference problems by leveraging the unimodal data. However, in recent years, with the increasing computation power, multi-modal learning is applied in developing different inference system. As multi-modal learning brings new information from different modalities, which in turn enable an inference system to embed this new information to learn a particular modality data representation with better confidence. For example, we can jointly learn the visual and textual data representation for Visual Question Answering System.

      **Outcome:** **I received Nvidia Academic GPU Grant to conduct this work**

    -  ### Transfer Learning in Visual Question Answering
      Primarily, in this project, we want to apply the multi-modal and transfer learning approaches to improve the Visual Question Answering(VQA) system. We developed a multi-modal learning model by utilizing [VizWiz Dataset](http://vizwiz.org/data/#dataset) and achieved considerable performance. We have a plan to extend this work to test our approach in other datasets by incorporating transfer learning approach.

        **Outcome:** [Manuscript in Preparation]

  * ## Design Optimization and Evolutionary Approaches
    The aim of this project is to design optimization and evolutionary approaches to solve NP-Complete problems in various domains, such as resource allocation in cloud computing environment and reduce overfitting issue as well as improve the reasoning process in learning models.
      - ### Resource Allocation in Mobile Cloud Computing
      In this project, we utilized two evolutionary approaches, Genetic Algorithm and Particle Swarm Optimization(specifically Ant Colony Optimization) to design two resource allocation schemes in heterogeneous Mobile Cloud Computing(MCC) environment. This meta-heuristics resource allocation approaches helps to minimize the task execution and subsequently increase resource utilization in MCC, which is very crucial for Big data-based resource constrained cloud application, such as mobile and e-health application.

        **Outcome:** [IEEE Access 2017](http://ieeexplore.ieee.org/document/7933943/),[NSysS 2016](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=7400696)

      - ### Reduce Overfitting Problem in Deep Learning Models
      We are currently working with some evolutionary and meta-heuristic local search approaches to reduce the overfitting problem in deep learning problem, as till now most of the effective solution of overfitting problem is not guided approach. Primarily, we are working in designing meta-heuristic dropout approach to reducing the overfitting problem.

        **Outcome:** [Work in Progress]

      - ### Optimized Distributed Clustering Model in DSN
      We developed a dynamic distributed clustering model to minimizes energy consumption and data collection time in the directional sensor network(DSN) by minimizing the active directional sensor nodes. Our clustering approach is showed effective performance to increase the network lifetime in DSN.

        **Outcome:** [EURASIP JWCN 2015](http://link.springer.com/article/10.1186/s13638-015-0394-2),[IEEE APWiMob 2014](http://ieeexplore.ieee.org/document/6920259/)

  * ## Developer Question Answering and Repository Mining
    The aim of this work is to mine the question answering(QA) system data, especially StackOverflow QA data, and other software project repository data in order to design some learning and thus ease the software development process. As a part of this project, we developed an accepted answer recommendation model, which helps to rank the answer in a StackOverflow question by utilizing various textual and meta-features of the question, answer and the comments [RAiTA](https://link.springer.com/chapter/10.1007/978-981-13-1498-8_11).

    **Outcome:** [Springer IEMIS 2018](https://link.springer.com/chapter/10.1007/978-981-13-1498-8_11)

  * ## Interpretable Machine Learning
    The goal of this project is to develop applications, which enable people to understand the learning process of learning models. In recent years several complex learning models have been proposed and these models outperform in solving several complex tasks. However, these mostly fails to explain the internal reasoning process, i.e. how their internal structure learns and most importantly which features learns in a particular layer. In this project, we address this problem and develop applications which help people to understand the black-box learning process. Moreover, we are also developing application which may help to debug learning models.

      **Outcome:** [Under Review],[Manuscript in Preparation]s

## Natural Language Processing
Currently, we are working in designing transfer learning approaches in order to improve various computational linguistic problems. Furthermore, we are involved in developing the computationally linguistic model and comprehensive datasets of Bangla language. Because, in the literature, a few works address Bangla language, mainly due to the complexity of this language and the scarcity of the datasets.

  * ### Transfer Learning Approach to Extract Fact and Validate Statement
  In recent years, with the proliferation of social media, the validating statement appears as a crucial problem and attract the attention of NLP research communities. However, due to the lack of any comprehensive dataset, NLP communities could not address this problem effectively. That's why in this work, we are utilizing the transfer learning approach to develop a fact extraction and checking models with the few available datasets.

    **Outcome:**[Manuscript in Preparation]

  * ### Bangla Article Classification
  We curated a comprehensive dataset of Bangla news articles, which contains around 400,000 news articles collected from different Bangla News portals. We also develop Bangla articles classification model with semantic textual features, which outperforms state-of-art-works. Moreover, we have also plan to extend this dataset, so that we can address other Bangla NLP research problems.

    **Outcome:** ICBSLP 2018[[Dataset and Source Code](https://github.com/tanvirfahim15/BARD-Bangla-Article-Classifier), [Web Application](http://bard2018.pythonanywhere.com/)]
  * ### Bangla Speech and Speakers Identification
  Presently, in this work, we are developing a Bangla speech dataset so that researchers can develop various computational learning models, such as Bangla voice recognition, speakers identification etc. Till now, there is no public Bangla speech dataset available for research purpose.

    **Outcome:** [Data Collection Application](http://banglawordlearner.firebaseapp.com)

## Computational Biology
In this research project, we are working with domain experts to develop a learning model to solve various Bio-Informatics related problems.

  * ###  iProtGly-SS: Identifying Protein Lysine Glycation Sites
  Glycation is a chemical reaction by which sugar molecule bonds with a protein without the help of enzymes. This is often caused to many diseases and therefore the knowledge about glycation is very important. In this work, we designed a supervised learning model, iProtGly-SS, to identify protein lysine glycation site based on features extracted from sequence and secondary structural information.

    **Outcome:** [Proteins Journal 2018](https://www.ncbi.nlm.nih.gov/pubmed/29675975) [[Source Code, Data, Web Application](http://brl.uiu.ac.bd/iprotgly-ss/)]

  * ### Identification of Recombination Hotspot in Genome
  In this work, we are trying to develop a deep learning in order to extract the sequence-based features and thus identify the recombination hotspot in a genome.
    **Outcome:** [Work in Progress]


## Big Graph Query and Mining
We are working to develop algorithms which help to query and mining subgraph in a big graph dataset. Currently, we developed heuristic pruning based subgraph graph query approach to speed up the search and mining approach in the big scholarly dataset. As we are writing the paper, that's why we can not able to disclose our complete problem description and solution. However, if you need any more information, you can contact me.

  **Outcome:** [Manuscript in Preparation]
