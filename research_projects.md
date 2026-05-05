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
  * [Artificial Intelligence and Machine Learning](#artificial-intelligence-and-machine-learning)
    - [Multi-modal and Multi-task Learning **\[Grant\]**](#multi-modal-and-multi-task-learning)
    - [Design Optimization and Evolutionary Approaches](#design-optimization-and-evolutionary-approaches)
      - [Resource Allocation in Mobile Cloud Computing](#resource-allocation-in-mobile-cloud-computing)
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

## Generative AI and Large Language Models
At AWS GenAI, I lead research on the next generation of multimodal LLMs and agentic systems. My focus spans multi-agent reasoning, post-training and finetuning of multimodal LLMs, synthetic data generation, and agentic document intelligence.

  * ## Multi-Agent Reasoning
    Lead: Md Mofijul Islam, AWS GenAI

    We develop multi-agent reasoning frameworks that plan, search, and coordinate across specialized agents to tackle complex tasks such as scientific discovery, retrosynthesis, document understanding, and compliance validation. Our work combines structured memory, search-based planning, and tool use to move beyond single-pass LLM reasoning toward collaborative agentic inference.

    **Outcome:** [COLM-2026 (RETROAGENT)], [ACL-2026 Demo — IDP Accelerator: Agentic Document Intelligence from Extraction to Compliance Validation], [AWS Blog: Strands AI Agents for GenAI IDP](https://aws.amazon.com/blogs/machine-learning/enhance-document-analytics-with-strands-ai-agents-for-the-genai-idp-accelerator/), [AWS Blog: Agent Tooling for LLM-Powered Data Exploration (DXC)](https://aws.amazon.com/blogs/machine-learning/dxc-transforms-data-exploration-for-their-oil-and-gas-customers-with-llm-powered-tools/)

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

    **Outcome:** [AWS Blog: SailPoint TypeScript Code Generation](https://aws.amazon.com/blogs/machine-learning/how-sailpoint-uses-anthropics-claude-on-amazon-bedrock-to-automatically-generate-typescript-code-for-saas-connectors/), [AWS Blog: Agentic Code Generation (Totogi)](https://aws.amazon.com/blogs/machine-learning/how-totogi-automated-change-request-processing-with-totogi-bss-magic-and-amazon-bedrock/)

## Artificial Intelligence and Machine Learning
I work at the intersection of theoretical artificial intelligence and practical machine learning. I develop learning models that solve problems across a variety of domains, collaborating with domain experts while also designing and modifying the internal structure of various learning models.

  * ## Multi-modal and Multi-task Learning
    Primary Investigator: Md Mofijul Islam, University of Dhaka

    Representation learning has been widely applied in areas such as computer vision, natural language processing (NLP), and social network analysis. Most representation learning approaches solve inference problems using unimodal data. In recent years, with growing compute, multimodal learning has become central to many inference systems: by bringing in complementary information across modalities, it allows a system to learn stronger representations for each modality. For example, we can jointly learn visual and textual representations for Visual Question Answering systems.

      **Outcome:** Received the NVIDIA Academic GPU Grant to support this work.

  * ## Design Optimization and Evolutionary Approaches
    This project designs optimization and evolutionary approaches to solve NP-complete problems across domains — including resource allocation in cloud computing, mitigating overfitting, and improving the reasoning process in learning models.
      - ### Resource Allocation in Mobile Cloud Computing
      Supervisor: Dr. Md Abdur Razzaque, University of Dhaka

      We used two evolutionary approaches — Genetic Algorithms and Particle Swarm Optimization (specifically Ant Colony Optimization) — to design resource allocation schemes for heterogeneous Mobile Cloud Computing (MCC) environments. These meta-heuristic approaches minimize task execution time and improve resource utilization, which is critical for big-data-driven, resource-constrained cloud applications such as mobile and e-health systems.

      **Outcome:** [IEEE Access 2017](http://ieeexplore.ieee.org/document/7933943/), [NSysS 2016](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=7400696)

      - ### Optimized Distributed Clustering Model in DSN
      Supervisor: Dr. Md Abdur Razzaque, University of Dhaka

      We developed a dynamic distributed clustering model that minimizes energy consumption and data collection time in directional sensor networks (DSNs) by reducing the number of active directional sensor nodes. The approach effectively increased network lifetime in DSNs.

      **Outcome:** [EURASIP JWCN 2015](http://link.springer.com/article/10.1186/s13638-015-0394-2), [IEEE APWiMob 2014](http://ieeexplore.ieee.org/document/6920259/)

  * ## Developer Question Answering and Repository Mining
    Supervisor: Md Mofijul Islam, United International University

    This project mines question-answering (QA) data — especially from Stack Overflow — along with data from software project repositories, with the goal of designing learning models that streamline the software development process. As part of this work, we developed an accepted-answer recommendation model, [RAiTA](https://link.springer.com/chapter/10.1007/978-981-13-1498-8_11), which ranks answers to Stack Overflow questions using textual and meta-features of the question, answer, and comments.

    **Outcome:** [Springer IEMIS 2018](https://link.springer.com/chapter/10.1007/978-981-13-1498-8_11)

  * ## Interpretable Machine Learning
    Primary Investigator: Md Mofijul Islam, University of Dhaka

    This project builds tools that help people understand how learning models learn. In recent years, several complex models have achieved strong performance on difficult tasks, yet often fail to explain their internal reasoning — how their layers learn and which features each layer captures. We develop applications that help users understand these black-box learning processes, and we are also building tools to aid in debugging learning models.

      - ### d-DeVIS: A Gray-Box Interpretable Visual Debugging Approach for Deep Sequence Learning Models

      Deep learning algorithms are frequently treated as black boxes and are difficult to interpret. Their widespread use demands a deeper, more transparent understanding of their internal representations and decision-making. Models trained on sequential data — such as audio and video — have especially intricate internal reasoning due to complex feature distributions. A visual simulator can help trace internal decision-making in response to adversarial inputs, aiding both debugging and model design. We developed d-DeVIS, an interactive web application that visualizes the internal reasoning of a model trained on audio data, letting users interpret model behavior and debug it by interactively generating adversarial audio inputs.

      **Outcome:** [ArXiv](https://arxiv.org/abs/1811.08374), [Video Demo](https://www.youtube.com/watch?v=O2bNV-U0ylg), [Web Application](http://ddevis.herokuapp.com/), [Source Code](https://github.com/anon-conf/d-DeVIS)


## Natural Language Processing
We design transfer learning approaches to improve a range of computational linguistic tasks, and we also build computational linguistic models and comprehensive datasets for the Bangla language. Relatively few works address Bangla, largely due to the complexity of the language and the scarcity of publicly available datasets.

  * ### Transfer Learning Approach to Fact Extraction and Statement Validation
  Primary Investigator: Md Mofijul Islam, University of Dhaka

  With the proliferation of social media, statement validation has become a crucial problem for the NLP research community. However, progress has been limited by the lack of comprehensive datasets. In this project, we use transfer learning to build fact extraction and checking models from the limited data available.

  **Outcome:** Accepted at IJCCI 2018.

  * ### Bangla Article Classification
  Supervisor: Md Mofijul Islam, University of Dhaka

  We curated a comprehensive dataset of approximately 400,000 Bangla news articles collected from various Bangla news portals, and developed a Bangla article classification model using semantic textual features that outperforms state-of-the-art methods. We plan to extend this dataset to support additional Bangla NLP research problems.

  **Outcome:** ICBSLP 2018 [[Dataset & Code]](https://github.com/tanvirfahim15/BARD-Bangla-Article-Classifier) [[Web App]](http://bard2018.pythonanywhere.com/)

  * ### Bangla Speech and Speaker Identification
  Primary Investigator: Md Mofijul Islam, University of Dhaka

  In this project, we are developing a Bangla speech dataset to enable research on computational learning models for tasks such as Bangla voice recognition and speaker identification. To date, no public Bangla speech dataset has been available for research purposes.

  **Outcome:** [Data Collection App](http://banglawordlearner.firebaseapp.com)

## Computational Biology
Supervisor: Dr. Swakkhar Shatabda, United International University

In this project, we collaborate with domain experts to develop learning models for a range of bioinformatics problems.

  * ### iProtGly-SS: Identifying Protein Lysine Glycation Sites Using Sequence Features
  Glycation is a chemical reaction in which a sugar molecule bonds with a protein without the aid of enzymes, and it is implicated in many diseases — so accurate identification of glycation sites is important. In this work, we designed a supervised learning model, iProtGly-SS, to identify protein lysine glycation sites from features extracted from sequence and secondary-structure information.

    **Outcome:** [Proteins Journal 2018](https://www.ncbi.nlm.nih.gov/pubmed/29675975) [[Code, Data & Web App]](http://brl.uiu.ac.bd/iprotgly-ss/)
