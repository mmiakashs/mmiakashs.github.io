---
layout: about
title: Research Projects
description: >
  Md Mofijul Islam's Research.
hide_description: true
menu: false
order: 3
---

Table of Contents
  * [Generative AI and Large Language Models](#generative-ai-and-large-language-models)
    - [Multi-Agent Reasoning](#multi-agent-reasoning)
    - [Post-Training and Finetuning of Multimodal LLMs](#post-training-and-finetuning-of-multimodal-llms)
    - [Synthetic Data Generation](#synthetic-data-generation)
    - [Agentic Document Intelligence](#agentic-document-intelligence)
    - [Code Generation](#code-generation)
  * [Artificial Inteligence and Machine learning](#artificial-intelligence-and-machine-learning)
    - [Multi-modal and Multi-task Learning **\[Grant\]**](#multi-modal-and-multi-task-learning)
      - [Transfer Lerning in Visual Question Answering](#transfer-learning-in-visual-question-answering)
    - [Design Optimization and Evolutionary Approches](#design-optimization-and-evolutionary-approaches)
      - [Resource Allocation in Mobile Cloud Computing](#resource-allocation-in-mobile-cloud-computing)
      - [Reduce Overfiting Problem in Deep Learning Models](#reduce-overfitting-problem-in-deep-learning-models)
      - [Optimized Distributed Clustering Model in DSN](#optimized-distributed-clustering-model-in-dsn)
    - [Developer Question Answering and Repository Mining](#developer-question-answering-and-repository-mining)
    - [Interpretable Machine Learning](#interpretable-machine-learning)
      - [d-DeVIS](#d-devis-a-gray-box-interpretable-visual-debugging-approach-for-deep-sequence-learning-model)
  - [Natural Language Processing](#natural-language-processing)
    - [Transfer Learning Approach to Extract Fact and Validate Statement](#transfer-learning-approach-to-extract-fact-and-validate-statement)
    - [Bangla Article Classfication](#bangla-article-classification)
    - [Bangla Speech and Speakers Identification](#bangla-speech-and-speakers-identification)
  * [Computational Biology](#computational-biology)
    - [iProtGly-SS: Identifying Protein Lysine Glycation Sites Using Sequence Features](#iprotgly-ss-identifying-protein-lysine-glycation-sites-using-sequence-features)
    - [Identification of Recombination Hotspot in Genome](#identification-of-recombination-hotspot-in-genome)
  * [Big Graph Query and Mining](#big-graph-query-and-mining)
  * [Mining Spatiotemporal Behavior of Contributors in OpenStreetMap](#mining-spatiotemporal-behavior-of-contributors-in-openstreetmap)

## Generative AI and Large Language Models
At AWS GenAI, I lead research on the next generation of multimodal LLMs and agentic systems. My focus spans multi-agent reasoning, post-training and finetuning of multimodal LLMs, synthetic data generation, and agentic document intelligence.

  * ## Multi-Agent Reasoning
    Lead: Md Mofijul Islam, AWS GenAI

    We develop multi-agent reasoning frameworks that plan, search, and coordinate across specialized agents to tackle complex tasks such as scientific discovery, retrosynthesis, document understanding, and compliance validation. Our work combines structured memory, search-based planning, and tool use to move beyond single-pass LLM reasoning toward collaborative agentic inference.

    **Outcome:** [COLM-2026 (RETROAGENT)], [ACL-2026 Demo — IDP Accelerator: Agentic Document Intelligence from Extraction to Compliance Validation], [AWS Blog: Strands AI Agents for GenAI IDP](https://aws.amazon.com/blogs/machine-learning/enhance-document-analytics-with-strands-ai-agents-for-the-genai-idp-accelerator/)

  * ## Post-Training and Finetuning of Multimodal LLMs
    Lead: Md Mofijul Islam, AWS GenAI

    We develop post-training and finetuning techniques — including supervised finetuning, preference optimization, distillation, and residual multimodal alignment — to adapt multimodal LLMs to high-value downstream tasks across text, vision, and speech. This work underpins several recent publications on scalable learners, multilingual reasoning, speech tokenization, and embodied referring expression comprehension.

    **Outcome:** [ICLR-2026 Oral (Energy-Based Transformers)](https://arxiv.org/abs/2406.08862), [ACL-2026 (Multilingual LLMs)](https://arxiv.org/abs/2510.07877), [EACL-2026 (MATHMIST)](https://arxiv.org/abs/2510.14305), [HRI-2026 (Embodied REC)](https://arxiv.org/abs/2512.06558), [EMNLP-2025 (DM-Codec)](https://arxiv.org/abs/2410.15017), [InterSpeech-2026 (FuseCodec)](https://arxiv.org/abs/2509.11425)

  * ## Synthetic Data Generation
    Lead: Md Mofijul Islam, AWS GenAI

    Data scarcity and distribution mismatch are core bottlenecks for post-training multimodal and multilingual LLMs. We build synthetic data generation pipelines — including benchmark construction and targeted data curation — that cover low-resource languages, complex document forms, and mathematical reasoning.

    **Outcome:** [ACL-2026 Industry Track (DocSplit)](https://huggingface.co/datasets/amazon/doc_split), [EACL-2026 (MATHMIST)](https://arxiv.org/abs/2510.14305), [ECCV-2026 (BaFCo: Complex Bangla Form Comprehension)]

  * ## Agentic Document Intelligence
    Lead: Md Mofijul Islam, AWS GenAI

    We build end-to-end agentic systems for intelligent document processing — spanning document packet splitting, multimodal extraction, analytics, and compliance validation — and released an org-wide open-source [GenAI IDP Accelerator](https://github.com/aws-samples/sample-genai-idp) that has contributed millions in ARR.

    **Outcome:** [Open-Source: GenAI IDP Accelerator](https://github.com/aws-samples/sample-genai-idp), [ACL-2026 Industry Track (DocSplit)](https://huggingface.co/datasets/amazon/doc_split), [ACL-2026 Demo (IDP Accelerator)], [AWS Blog: Multimodal Document Processing](https://aws.amazon.com/blogs/machine-learning/accelerate-intelligent-document-processing-with-generative-ai-on-aws/), [AWS Blog: Healthcare Document Comprehension](https://aws.amazon.com/blogs/machine-learning/how-myriad-genetics-achieved-fast-accurate-and-cost-efficient-document-processing-using-the-aws-open-source-generative-ai-intelligent-document-processing-accelerator/)

  * ## Code Generation
    Lead: Md Mofijul Islam, AWS GenAI

    We develop LLM-powered code generation systems for real-world software engineering workflows — including automated SaaS connector generation and agentic change-request processing for enterprise customers.

    **Outcome:** [AWS Blog: SailPoint TypeScript Code Generation](https://aws.amazon.com/blogs/machine-learning/how-sailpoint-uses-anthropics-claude-on-amazon-bedrock-to-automatically-generate-typescript-code-for-saas-connectors/), [AWS Blog: Agentic Code Generation (Totogi)](https://aws.amazon.com/blogs/machine-learning/how-totogi-automated-change-request-processing-with-totogi-bss-magic-and-amazon-bedrock/), [AWS Blog: LLM-Tools (DXC)](https://aws.amazon.com/blogs/machine-learning/dxc-transforms-data-exploration-for-their-oil-and-gas-customers-with-llm-powered-tools/)

## Artificial Intelligence and Machine Learning
I am mainly working in the intersection of theoretical artificial intelligence and practical machine learning approaches. Currently, I am working to develop some learning models to solve problems in the various domain. As mainly I am involved in the design and developing learning model, I collaborate with several domain experts in different fields. Furthermore, I am interested to design and modify the internal structure of various learning models.

  * ## Multi-modal and Multi-task Learning
    Primary Investigator: Md Mofijul Islam, University of Dhaka

    Representation learning is applied in different areas, such as Computer Vision, Natural Language Processing(NLP), Social Network analysis, etc. Most of the representational learning are applied in solving inference problems by leveraging the unimodal data. However, in recent years, with the increasing computation power, multi-modal learning is applied in developing different inference system. As multi-modal learning brings new information from different modalities, which in turn enable an inference system to embed this new information to learn a particular modality data representation with better confidence. For example, we can jointly learn the visual and textual data representation for Visual Question Answering System.

      **Outcome:** **Received Nvidia Academic GPU Grant to conduct this work**

    -  ### Transfer Learning in Visual Question Answering
      Primary Investigator: Md Mofijul Islam, University of Dhaka

      Primarily, in this project, we want to apply the multi-modal and transfer learning approaches to improve the Visual Question Answering(VQA) system. We developed a multi-modal learning model by utilizing [VizWiz Dataset](http://vizwiz.org/data/#dataset) and achieved considerable performance. We have a plan to extend this work to test our approach in other datasets by incorporating transfer learning approach.

      **Outcome:** [Manuscript in Preparation]

  * ## Design Optimization and Evolutionary Approaches
    The aim of this project is to design optimization and evolutionary approaches to solve NP-Complete problems in various domains, such as resource allocation in cloud computing environment and reduce overfitting issue as well as improve the reasoning process in learning models.
      - ### Resource Allocation in Mobile Cloud Computing
      Supervisor: Dr. Md Abdur Razzaque, University of Dhaka

      In this project, we utilized two evolutionary approaches, Genetic Algorithm and Particle Swarm Optimization(specifically Ant Colony Optimization) to design two resource allocation schemes in heterogeneous Mobile Cloud Computing(MCC) environment. This meta-heuristics resource allocation approaches helps to minimize the task execution and subsequently increase resource utilization in MCC, which is very crucial for Big data-based resource constrained cloud application, such as mobile and e-health application.

      **Outcome:** [IEEE Access 2017](http://ieeexplore.ieee.org/document/7933943/),[NSysS 2016](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=7400696)

      - ### Reduce Overfitting Problem in Deep Learning Models
      Supervisor: Dr. Swakkhar Shatabda, United International University

      We are currently working with some evolutionary and meta-heuristic local search approaches to reduce the overfitting problem in deep learning problem, as till now most of the effective solution of overfitting problem is not guided approach. Primarily, we are working in designing meta-heuristic dropout approach to reducing the overfitting problem.

      **Outcome:** [Work in Progress]

      - ### Optimized Distributed Clustering Model in DSN
      Supervisor: Dr. Md Abdur Razzaque, University of Dhaka

      We developed a dynamic distributed clustering model to minimize energy consumption and data collection time in the directional sensor network(DSN) by minimizing the active directional sensor nodes. Our clustering approach is showed effective performance to increase the network lifetime in DSN.

      **Outcome:** [EURASIP JWCN 2015](http://link.springer.com/article/10.1186/s13638-015-0394-2),[IEEE APWiMob 2014](http://ieeexplore.ieee.org/document/6920259/)

  * ## Developer Question Answering and Repository Mining
    Supervisor: Md Mofijul Islam, United International University

    The aim of this work is to mine the question answering(QA) system data, especially StackOverflow QA data, and other software project repositories data in order to design some learning and thus ease the software development process. As a part of this project, we developed an accepted answer recommendation model, which helps to rank the answer in a StackOverflow question by utilizing various textual and meta-features of the question, answer and the comments [RAiTA](https://link.springer.com/chapter/10.1007/978-981-13-1498-8_11).

    **Outcome:** [Springer IEMIS 2018](https://link.springer.com/chapter/10.1007/978-981-13-1498-8_11)

  * ## Interpretable Machine Learning
    Primary Investigator: Md Mofijul Islam, University of Dhaka

    The goal of this project is to develop applications, which enable people to understand the learning process of learning models. In recent years several complex learning models have been proposed and these models outperform in solving several complex tasks. However, these mostly fails to explain the internal reasoning process, i.e. how their internal structure learns and most importantly which features learns in a particular layer. In this project, we address this problem and develop applications which help people to understand the black-box learning process. Moreover, we are also developing application which may help to debug learning models.

      - ### d-DeVIS: A Gray Box Interpretable Visual Debugging Approach for Deep Sequence Learning Model

      Deep Learning algorithms are often used as black box type learning and they are too complex to understand. The widespread usability of Deep Learning algorithms to solve various machine learning problems demands deep and transparent understanding of the internal representation as well as decision making. Moreover, the learning models, trained on sequential data, such as audio and video data, have intricate internal reasoning process due to their complex distribution of features. Thus, a visual simulator might be helpful to trace the internal decision making mechanisms in response to adversarial input data, and it would help to debug and design appropriate deep learning models. However, interpreting the internal reasoning of deep learning model is not well studied in the literature. In this work, we have developed a visual interactive web application, namely d-DeVIS, which helps to visualize the internal reasoning of the learning model which is trained on the audio data. The proposed system allows to perceive the behavior as well as to debug the model by interactively generating adversarial audio data point.

      **Outcome:** [ArXiv](https://arxiv.org/abs/1811.08374), [Video Demo](https://www.youtube.com/watch?v=O2bNV-U0ylg), [Web Application](http://ddevis.herokuapp.com/), [Source Code](https://github.com/anon-conf/d-DeVIS)


## Natural Language Processing
Currently, we are working in designing transfer learning approaches in order to improve various computational linguistic problems. Furthermore, we are involved in developing the computationally linguistic model and comprehensive datasets of Bangla language. Because, in the literature, a few works address Bangla language, mainly due to the complexity of this language and the scarcity of the datasets.

  * ### Transfer Learning Approach to Extract Fact and Validate Statement
  Primary Investigator: Md Mofijul Islam, University of Dhaka

  In recent years, with the proliferation of social media, the validating statement appears as a crucial problem and attract the attention of NLP research communities. However, due to the lack of any comprehensive dataset, NLP communities could not address this problem effectively. That's why in this work, we are utilizing the transfer learning approach to develop a fact extraction and checking models with the few available datasets.

  **Outcome:** [Accepted in IJCCI 2018]

  * ### Bangla Article Classification
  Supervisor: Md Mofijul Islam, University of Dhaka

  We curated a comprehensive dataset of Bangla news articles, which contains around 400,000 news articles collected from different Bangla News portals. We also develop Bangla articles classification model with semantic textual features, which outperforms state-of-art-works. Moreover, we have also plan to extend this dataset, so that we can address other Bangla NLP research problems.

  **Outcome:** ICBSLP 2018[[Dataset and Source Code](https://github.com/tanvirfahim15/BARD-Bangla-Article-Classifier), [Web Application](http://bard2018.pythonanywhere.com/)]

  * ### Bangla Speech and Speakers Identification
  Primary Investigator: Md Mofijul Islam, University of Dhaka

  Presently, in this work, we are developing a Bangla speech dataset so that researchers can develop various computational learning models, such as Bangla voice recognition, speakers identification etc. Till now, there is no public Bangla speech dataset available for research purpose.

  **Outcome:** [Data Collection Application](http://banglawordlearner.firebaseapp.com)

## Computational Biology
Supervisor: Dr. Swakkhar Shatabda, United International University

In this research project, we are working with domain experts to develop a learning model to solve various Bio-Informatics related problems.

  * ###  iProtGly-SS: Identifying Protein Lysine Glycation Sites Using Sequence Features
  Glycation is a chemical reaction by which sugar molecule bonds with a protein without the help of enzymes. This is often caused to many diseases and therefore the knowledge about glycation is very important. In this work, we designed a supervised learning model, iProtGly-SS, to identify protein lysine glycation site based on features extracted from sequence and secondary structural information.

    **Outcome:** [Proteins Journal 2018](https://www.ncbi.nlm.nih.gov/pubmed/29675975) [[Source Code, Data, Web Application](http://brl.uiu.ac.bd/iprotgly-ss/)]

  * ### Identification of Recombination Hotspot in Genome
  In this work, we are trying to develop a deep learning in order to extract the sequence-based features and thus identify the recombination hotspot in a genome.
    **Outcome:** [Work in Progress]


## Big Graph Query and Mining
Primary Investigator: Md Mofijul Islam, University of Dhaka

We are working to develop algorithms which help to query and mining subgraph in a big graph dataset. Currently, we developed heuristic pruning based subgraph graph query approach to speed up the search and mining approach in the big scholarly dataset. As we are writing the paper, that's why we can not able to disclose our complete problem description and solution. However, if you need any more information, you can contact me.

  **Outcome:** [Manuscript in Preparation]

## Mining Spatiotemporal Behavior of Contributors in OpenStreetMap
Supervisor: Dr. Syed Ishtiaque Ahmed, University of Toronto

The aim of this project is to mine the Spatiotemporal behavior and contribution bias in peer of production system, specifically OpenStreetMap.
