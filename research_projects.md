---
layout: about
title: Research
description: >
  Md Mofijul Islam's Portfolio.
hide_description: true
menu: true
order: 3
---
Table of Contents
  * [Artificial Inteligence and Machine learning](#artificial-inteligence-and-machine-learning)
    - [Multi-modal and Multi-task Learning \[Grant\]](#multi-modal-and-multi-task-learning)
      - [Transfer Lerning in Visual Question Answering](#transfer-lerning-in-visual-question-answering)
    - [Design Optimization and Evolutionary Approches](#design-optimization-and-evolutionary-approches)
      - [Resource Allocation in Mobile Cloud Computing](#resource-allocation-in-mobile-cloud-computing)
      - [Reduce Overfiting Problem in Deep Learning Models](#reduce-overfiting-problem-in-deep-learning-models)
      - [Interpretable Machine Learning](#interpretable-machine-learning)
  - [Natural Language Processing](#natural-language-processing)
    - [Transfer Learning Approach to Extract Fact and Validate Statement](#transfer-learning-approach-to-extract-fact-and-validate-statement)
    - [Bangla Article Classfication](#bangla-article-classfication)
    - [Bangla Speech and Speakers Identification](#bangla-speech-and-speakers-identification)
  * [Computational Biology](#computational-biology)
    - [iProtGly-SS: Identifying Protein Lysine Glycation Sites](#iprotgly-ss-identifying-protein-lysine-glycation-sites)
    - [Identification of Recombination Hotspot in Genome](#identification-of-recombination-hotspot-in-genome)
  * [Big Graph Mining](#big-graph-mining)

[//]:  * [Data Visualization](#data-visualization)

## Artificial Inteligence and Machine Learning
I am mainly working in intersection of theoretical artificial inteligence and practicle machine learning approaches. Currently, I am working to develop some learning models to solve problems in various domain. As, mainly I am involved in design and developing learing model, I collaborate with several domain experts of differnt fields. Furthermore, I am interested to design and modify the internal structure of various learning models.

  * ## Multi-modal and Multi-task Learning
    Representation learning is applied in different areas, such as Computer Vision, Natural Language Processing(NLP), Social Network analysis, etc. Most of the representational learning are applied in solving inference problems by leveraging the unimodal data. However, in recent years, with the increasing computation power, multi-modal learning is applied in developing different inference system. As multi-modal learning brings new information from different modalities, which in turn enable an inference system to embed this new information to learn a particular modality data representation with better confidence. For example, we can jointly learn the visual and textual data representation for Visual Question Answering System.

      **Outcome:** **I received Nvidia Academic GPU Grant to conduct this work**

    -  ### Transfer Lerning in Visual Question Answering
      Primarily, in this project, we want to apply the multi-modal and transfer learning approaches to improve the Visual Question Answering(VQA) system. We developed a multi-modal learning model by utilizing [VizWiz Dataset](http://vizwiz.org/data/#dataset) and acheived considerable performance. We have a plan to extend this work to test our approach in other datasets by incorporating transfer learning approach.

        **Outcome:** [Manuscript in Preparation]

  * ## Design Optimization and Evolutionary Approches
    The aim of this project is to design optimization and evolutionary approches to solve NP-Complete problems in various domains, such as resource allocation in cloud computing environment and reduce overfiting issue as well as improve the reasoning process in learning models.
      - ### Resource Allocation in Mobile Cloud Computing
      In this project, we utilized two evolutionary approches, Genetic Algorithm and Particle Swarm Optimization(specifically Ant Colony Optimization) to design two resource allocation schemes in heterogeneous Mobile Cloud Computing(MCC) environment. These meta-heuristics resource allocation approches helps to minimizes the task execution and subsequently increase resource utilization in MCC, which is very crucial for Big data based resource constrained cloud application, such as mobile and e-health application.

        **Outcome:** [IEEE Access 2017](http://ieeexplore.ieee.org/document/7933943/),[NSysS 2016](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=7400696)

      - ### Reduce Overfiting Problem in Deep Learning Models
      We are currently working with some evolutionary and meta-heuristic local search approches to reduce the overfiting problem in deep learing problem, as till now most of the effective solution of overfiting problem is not guided approach. Primarily, we are working in designing meta-heuristic dropout approach to reduce the overfiting problem.

        **Outcome:** [Work in Progress]

      - ### Optimized Distributed Clustering Model in DSN
      We developed dynamic distributed clustering model to minimizes energy consumption and data collection time in directional sensor network(DSN) by minizing the active directional sensor nodes. Our clustering approches is showed effective performance to increase the network lifetime in DSN.

        **Outcome:** [EURASIP JWCN 2015](http://link.springer.com/article/10.1186/s13638-015-0394-2),[IEEE APWiMob 2014](http://ieeexplore.ieee.org/document/6920259/)

  * ## Developer Question Answering and Repository Mining
    The aim of this work is to develop

  * ## Interpretable Machine Learning
    The goal of this project is to develop applications, which enable people to understand the learning process of a learning models. In recent years several complex learning models have been proposed and these models outperforms in solving several complex task. However, these mostly fails to explain the internal reasoning process, i.e. how their internal structure learns and most importantly which features learns in a particular layer. In this project, we address this problem and develop applications which helps people to understand the black-box learning process. Moreover, we are also developing application which may help debugging a learning models.

      **Outcome:** [Under Review],[Manuscript in Preparation]s

## Natural Language Processing
Currently, we are working in designing transfer learning approaches in order to improve various computational linguistic problems. Furthermore, we are involved in developing the computationally linguistic model and comprehensive datasets of Bangla language. Because, in the literature, a few works address Bangla language, mainly due to the complexity of this language and scarccity of the datasets.

  * ### Transfer Learning Approach to Extract Fact and Validate Statement
  In recent years, with the proliferation of social media, validating statement apprears as a crucial problem and attract the attention of NLP research communities. However, due to the lack of any comprehensive dataset, NLP communities could not address this problems effectively. That's why in this work, we are utilizing the transfer learning approach to develop a fact extraction and checking models with the few available dataset.

    **Outcome:**[Manuscript in Preparation]

  * ### Bangla Article Classfication
  We curated a comprehensive dataset of Bangla news articles, which contains around 400,000 news articles collected from different Bangla News portals. We also develop Bangla articles classification model with semantic textual features, which outperforms state-of-art-works. Moreover, we have also plan to extend this dataset, so that we can address other Bangla NLP reserach problems.

    **Outcome:** ICBSLP 2018[[Dataset and Source Code](https://github.com/tanvirfahim15/BARD-Bangla-Article-Classifier), [Web Application](http://bard2018.pythonanywhere.com/)]
  * ### Bangla Speech and Speakers Identification
  Presently, in this work, we are developing a Bangla speech dataset so that researchers can develop various computational learning models, such as Bangla voice recognition, speakers identification etc. Till now, there is no public Bangla speech dataset avaiable for research purpose.

    **Outcome:** [Data Collection Application](http://banglawordlearner.firebaseapp.com)

## Computational Biology
In this research project, we are working with domain experts to develop learning model to solve various Bio-Informatics related problems.

  * ###  iProtGly-SS: Identifying Protein Lysine Glycation Sites
  Glycation is chemical reaction by which sugar molecule bonds with a protein without the help of enzymes. This is often cause to many diseases and therefore the knowledge about glycation is very important. In this work, we designed a supervised learning model, iProtGly-SS, to identify protein lysine glycation site based on features extracted from sequence and secondary structural information.

    **Outcome:** [Proteins Journal 2018](https://www.ncbi.nlm.nih.gov/pubmed/29675975) [[Source Code, Data, Web Application](http://brl.uiu.ac.bd/iprotgly-ss/)]

  * ### Identification of Recombination Hotspot in Genome
  In this work, we are trying to develop a deep learning in order to extract the sequence based features and thus identify the recombination hotspot in a genome.
    **Outcome:** [Work in Progress]


## Big Graph Mining
We are working to develop algorithms which helps to query and mining subgraph in big graph dataset. Currently, we developed heuristic puring based subgraph graph query approach to speedup the search and mining approach in big scholary dataset. As we are writing the paper, that's why we can not able to disclose our complete problem description and solution. However, if you need any more information, you can contact me.

  **Outcome:** [Manuscript in Preparation]

[//]: ## Data Visualization
