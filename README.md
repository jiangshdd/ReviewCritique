# ReviewCritique

This repository contains the **ReviewCritique** dataset from our EMNLP'24 paper: [LLMs Assist NLP Researchers: Critique Paper (Meta-)Reviewing](https://arxiv.org/abs/2406.16253).

## Claim

This work is not advocating the use of LLMs for paper (meta-)reviewing. Instead, we present a comparative analysis to identify and distinguish LLM activities from human activities. Two research goals: i) Enable better recognition of instances when someone implicitly uses LLMs for reviewing activities; ii) Increase community awareness that LLMs, and AI in general, are currently inadequate for performing tasks that require a high level of expertise and nuanced judgment.

## Abstract

This work is motivated by two key trends. On one hand, large language models (LLMs) have shown remarkable versatility in various generative tasks such as writing, drawing, and question answering, significantly reducing the time required for many routine tasks. On the other hand, researchers, whose work is not only time-consuming but also highly expertise-demanding, face increasing challenges as they have to spend more time reading, writing, and reviewing papers. This raises the question: how can LLMs potentially assist researchers in alleviating their heavy workload?

This study focuses on the topic of LLMs as NLP Researchers, particularly examining the effectiveness of LLMs in assisting paper (meta-)reviewing and its recognizability. To address this, we constructed the ReviewCritique dataset, which includes two types of information: (i) NLP papers (initial submissions rather than camera-ready) with both human-written and LLM-generated reviews, and (ii) each review comes with "deficiency" labels and corresponding explanations for individual segments, annotated by experts. Using ReviewCritique, this study explores two threads of research questions: (i) "LLMs as Reviewers", how do reviews generated by LLMs compare with those written by humans in terms of quality and distinguishability? (ii) "LLMs as Metareviewers", how effectively can LLMs identify potential issues, such as Deficient or unprofessional review segments, within individual paper reviews? To our knowledge, this is the first work to provide such a comprehensive analysis.

## Files

Datasets are located in the `/data/` folder:

- **ReviewCritique.jsonl**: Contains 100 papers with their corresponding human-written reviews, along with expert annotations for each review segment.

- **ReviewCritique_LLM.jsonl**: Contains 20 papers with LLM-generated reviews, including expert annotations for each review segment.

## License and Usage Restrictions

This dataset is provided for **research only**. It should **not** be used for training any models in order to preserve the dataset's integrity for future benchmarking of LLMs.

By using this dataset, you agree to the following terms:

1. The dataset may be used for evaluation, analysis, and benchmarking tasks.
2. You **must not** use the dataset for training machine learning models.
3. Any derivative works based on this dataset should clearly state the origin and follow these usage guidelines.

For more information, please refer to the detailed [LICENSE](./LICENSE).

## Citation
Please consider using the follow citation when using our dataset:
```
@article{du2024llms,
  title={Llms assist nlp researchers: Critique paper (meta-) reviewing},
  author={Du, Jiangshu and Wang, Yibo and Zhao, Wenting and Deng, Zhongfen and Liu, Shuaiqi and Lou, Renze and Zou, Henry Peng and Venkit, Pranav Narayanan and Zhang, Nan and Srinath, Mukund and others},
  journal={arXiv preprint arXiv:2406.16253},
  year={2024}
}
```