# ThoughtSource⚡
__A framework for the science of machine thinking__

ThoughtSource⚡ is a central, open resource and community around data and tools related to _chain-of-thought reasoning_ in large language models ([Wei 2022](https://arxiv.org/abs/2201.11903)). Our long-term goal is to enable trustworthy and robust reasoning in advanced AI systems for driving scientific research and development.

![ThoughtSource overview 3](/resources/images/thoughtsource-overview-3-small.png)

<br/><br/>

### __AI chain of thought creation:__

![ThoughtSource overview 1](/resources/images/thoughtsource-overview-1-small.png)

<br/><br/>

### __Human annotation:__
![ThoughtSource overview 2](/resources/images/thoughtsource-overview-2-small.png)


## Roadmap

1. Create a repository of chain-of-thought (CoT) datasets converted to a unified format. ✅
2. Create a conceptual model of different CoT reasoning styles and errors.
3. Create tools for diagnosing, annotating and evaluating CoT reasoning.
4. Provide models fine-tuned on high-quality CoT data.
4. Apply CoT reasoning to high-impact use-cases such as biomedical research or clinical decision making.

## Current datasets
__Datasets can be [browsed online through the Dataset Viewer 🔎](http://thought.samwald.info/)__. 
 
 We created [dataloaders](./libs/dataloader/) that allow you to access the following datasets in a standardized chain-of-thought format. The dataloaders create objects in the [Hugginface 🤗 Datasets format](https://huggingface.co/docs/datasets/index).


### General question answering
* __[commonsense_qa](https://www.tau-nlp.sites.tau.ac.il/commonsenseqa):__ Multiple-choice commonsense knowledge question answering dataset ([Talmor 2018](https://arxiv.org/abs/1811.00937)) enriched with explanations [ECQA](https://github.com/dair-iitd/ECQA-Dataset) ([Aggarwal 2021](https://aclanthology.org/2021.acl-long.238/)). _License:_ Unknown for CommonsenseQA, Community Data License Agreements Sharing license 1.0 for ECQA.
* __[strategy_qa](https://allenai.org/data/strategyqa):__ General-domain question-answering data from the StrategyQA dataset ([Geva 2021](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00370/100680/Did-Aristotle-Use-a-Laptop-A-Question-Answering)). _License:_ MIT.
* __[qed](https://github.com/google-research-datasets/QED):__ General-domain question-answering data from the QED dataset ([Lamm 2020](https://arxiv.org/abs/2009.06354)). _License:_ CC BY-SA 3.0.

### Scientific question answering
* __[worldtree](http://cognitiveai.org/explanationbank/):__ Scientific question-answering data from the WorldTree v2 dataset ([Xie 2020](https://aclanthology.org/2020.lrec-1.671/)) _License:_ Unknown.
* __[entailment_bank](https://allenai.org/data/entailmentbank):__ Science exam questions with expert-authored explanations from the EntailmentBank dataset ([Dalvi 2022](https://arxiv.org/pdf/2104.08661.pdf)). _License:_ CC BY 4.0.
* __[open_book_qa](https://allenai.org/data/open-book-qa):__ Scientific question-answering modeled after open book exams for assessing human understanding from the OpenBookQA dataset ([Mihaylov 2018](https://aclanthology.org/D18-1260.pdf)). _License:_ Unknown.

### Math word problems
* __[aqua](https://github.com/deepmind/AQuA):__ Math word problems from the AQUA-RAT (Algebra Question Answering with Rationales) dataset ([Ling 2017](https://arxiv.org/pdf/1705.04146.pdf)). _License:_ Apache 2.0.
* __[asdiv](https://github.com/chaochun/nlu-asdiv-dataset):__ Math word problems from the Academia Sinica Diverse MWP dataset ([Miao 2020](https://aclanthology.org/2020.acl-main.92/)). _License:_ Unknown.
* __[gsm8k](https://github.com/openai/grade-school-math):__  Math word problems from the GSM8K dataset ([Cobbe 2021](https://arxiv.org/abs/2110.14168)). _License:_ MIT.
* __[mawps](https://github.com/sroy9/mawps):__ Math word problems from MAWPS, the Math Word Problem Repository dataset ([Koncel-Kedziorski 2016](https://aclanthology.org/N16-1136.pdf)). _License:_ Unknown.
* __[svamp](https://github.com/arkilpatel/SVAMP):__ Math word problems. Source: SVAMP ([Patel 2021](https://aclanthology.org/2021.naacl-main.168/)) _License:_ MIT.


We are working on collecting and generating additional datasets, and on further improving the quality of existing datasets (see [dataset issues](https://github.com/OpenBioLink/ThoughtSource/issues?q=is%3Aissue+label%3Adataset)). We welcome suggestions for the inclusion of other datasets!

## Code
### Libraries

* __[dataloader](./libs/dataloader/):__ Library for creating and processing of ThoughtSource datasets (based on the Hugging Face 🤗 Datasets library).

### Applications

* __[dataset-viewer](./apps/dataset-viewer/):__ Streamlit application for browsing ThoughtSource datasets




