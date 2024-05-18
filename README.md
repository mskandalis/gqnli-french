# French version of the English GQNLI dataset (GQNLI-FR)

This repository contains a manually translated French version of the [GQNLI](https://github.com/ruixiangcui/GQNLI) challenge dataset, originally written in English. 

GQNLI is an evaluation corpus that is aimed for testing language model's generalized quantifier reasoning ability. The dataset can be used for the task of Natural Language Inference (NLI), also known as Recognizing Textual Entailment (RTE), which is a sentence-pair classification task.

It is also available directly on [huggingface.co](https://huggingface.co/datasets/maximoss/gqnli-fr).

# How to use in python

```
import pandas as pd

test = pd.read_csv("./gqnli.test.fr.tsv", sep='\t')
print(test)
```

# Citation Information

**BibTeX:**

````BibTeX
@inproceedings{skandalis-etal-2024-new-datasets,
    title = "New Datasets for Automatic Detection of Textual Entailment and of Contradictions between Sentences in {F}rench",
    author = "Skandalis, Maximos  and
      Moot, Richard  and
      Retor{\'e}, Christian  and
      Robillard, Simon",
    editor = "Calzolari, Nicoletta  and
      Kan, Min-Yen  and
      Hoste, Veronique  and
      Lenci, Alessandro  and
      Sakti, Sakriani  and
      Xue, Nianwen",
    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
    month = may,
    year = "2024",
    address = "Torino, Italy",
    publisher = "ELRA and ICCL",
    url = "https://aclanthology.org/2024.lrec-main.1065",
    pages = "12173--12186",
    abstract = "This paper introduces DACCORD, an original dataset in French for automatic detection of contradictions between sentences. It also presents new, manually translated versions of two datasets, namely the well known dataset RTE3 and the recent dataset GQNLI, from English to French, for the task of natural language inference / recognising textual entailment, which is a sentence-pair classification task. These datasets help increase the admittedly limited number of datasets in French available for these tasks. DACCORD consists of 1034 pairs of sentences and is the first dataset exclusively dedicated to this task and covering among others the topic of the Russian invasion in Ukraine. RTE3-FR contains 800 examples for each of its validation and test subsets, while GQNLI-FR is composed of 300 pairs of sentences and focuses specifically on the use of generalised quantifiers. Our experiments on these datasets show that they are more challenging than the two already existing datasets for the mainstream NLI task in French (XNLI, FraCaS). For languages other than English, most deep learning models for NLI tasks currently have only XNLI available as a training set. Additional datasets, such as ours for French, could permit different training and evaluation strategies, producing more robust results and reducing the inevitable biases present in any single dataset.",
}

@inproceedings{cui-etal-2022-generalized-quantifiers,
    title = "Generalized Quantifiers as a Source of Error in Multilingual {NLU} Benchmarks",
    author = "Cui, Ruixiang  and
      Hershcovich, Daniel  and
      S{\o}gaard, Anders",
    booktitle = "Proceedings of the 2022 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies",
    month = jul,
    year = "2022",
    address = "Seattle, United States",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.naacl-main.359",
    doi = "10.18653/v1/2022.naacl-main.359",
    pages = "4875--4893",
    abstract = "Logical approaches to representing language have developed and evaluated computational models of quantifier words since the 19th century, but today{'}s NLU models still struggle to capture their semantics. We rely on Generalized Quantifier Theory for language-independent representations of the semantics of quantifier words, to quantify their contribution to the errors of NLU models. We find that quantifiers are pervasive in NLU benchmarks, and their occurrence at test time is associated with performance drops. Multilingual models also exhibit unsatisfying quantifier reasoning abilities, but not necessarily worse for non-English languages. To facilitate directly-targeted probing, we present an adversarial generalized quantifier NLI task (GQNLI) and show that pre-trained language models have a clear lack of robustness in generalized quantifier reasoning.",
}
````

**ACL:**

Maximos Skandalis, Richard Moot, Christian Retoré, and Simon Robillard. 2024. [New Datasets for Automatic Detection of Textual Entailment and of Contradictions between Sentences in French](https://aclanthology.org/2024.lrec-main.1065). In *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)*, pages 12173–12186, Torino, Italy. ELRA and ICCL.

And

Ruixiang Cui, Daniel Hershcovich, and Anders Søgaard. 2022. [Generalized Quantifiers as a Source of Error in Multilingual NLU Benchmarks](https://aclanthology.org/2022.naacl-main.359). In *Proceedings of the 2022 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies*, pages 4875–4893, Seattle, United States. Association for Computational Linguistics.

# Acknowledgements

This work was supported by the Defence Innovation Agency (AID) of the Directorate General of Armament (DGA) of the French Ministry of Armed Forces, and by the ICO, _Institut Cybersécurité Occitanie_, funded by Région Occitanie, France.
