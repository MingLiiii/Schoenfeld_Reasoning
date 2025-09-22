# Understanding the Thinking Process of Reasoning Models: A Perspective from Schoenfeld's Episode Theory (EMNLP'25)


[Understanding the Thinking Process of Reasoning Models: A Perspective from Schoenfeld's Episode Theory](https://arxiv.org/abs/2509.14662)<br>(EMNLP'25)

This is the repo for the Schoenfeld_Reasoning project, which utilizes Schoenfeld's Episode Theory to analyze the reasoning traces for DeepSeek-R1. 

The repo contains: 

- The full SAT data we crawled, which contains not only SAT problems, but also metadata like skills, domains, and difficulties, which can be used for further analysis. 
- The full DeepSeek-R1 responses, and their corresponding paragraph-level and sentence-level episode annotations for our selected responses. 

(Feel free to email [Email](minglii@umd.edu) for any questions or feedback.)

## Contents
- [Overview](#overview)
- [Highlights](#highlights)
- [Data](#data)
- [Citation](#citation)

## Overview

While Large Reasoning Models (LRMs) generate extensive chain-of-thought reasoning, we lack a principled framework for understanding how these thoughts are structured. In this paper, we introduce a novel approach by applying Schoenfeld's Episode Theory, a classic cognitive framework for human mathematical problem-solving, to analyze the reasoning traces of LRMs. We annotated thousands of sentences and paragraphs from model-generated solutions to math problems using seven cognitive labels (e.g., Plan, Implement, Verify). The result is the first publicly available benchmark for the fine-grained analysis of machine reasoning, including a large annotated corpus and detailed annotation guidebooks. Our preliminary analysis reveals distinct patterns in LRM reasoning, such as the transition dynamics between cognitive states. This framework provides a theoretically grounded methodology for interpreting LRM cognition and enables future work on more controllable and transparent reasoning systems.

## Highlights

* We propose the earliest exploration on applying Schoenfeld’s Episode Theory to reasoning traces of LRMs, providing a unified view between how humans and LRMs solve math problems.
* We provide a theoretically grounded analytical framework for understanding and analyzing LRM thinking process from a cognitive view.
* We release the open annotation protocol and annotated corpus with thousands of annotations for the above-mentioned task, making it a well-defined task for controllable analysis.

## Data

`SAT.json`: All the SAT data. <br>
`responses_original/SAT_deepseekR1_results.json`: The DeepSeek-R1 responses for the selected SAT problems. <br>
`responses_labeled`: The directory that contains all the segmented responses and corresponding paragraph-level and sentence-level episode annotations. 

## Citation

Please consider citing our paper if you think our paper, data are useful. Thank you!
```
@article{li2025understanding,
  title={Understanding the Thinking Process of Reasoning Models: A Perspective from Schoenfeld's Episode Theory},
  author={Li, Ming and Zhang, Nan and Fan, Chenrui and Jiao, Hong and Fu, Yanbin and Peters, Sydney and Xu, Qingshu and Lissitz, Robert and Zhou, Tianyi},
  journal={arXiv preprint arXiv:2509.14662},
  year={2025}
}
```
