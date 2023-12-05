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

Ruixiang Cui, Daniel Hershcovich, and Anders Søgaard. 2022. [Generalized Quantifiers as a Source of Error in Multilingual NLU Benchmarks](https://aclanthology.org/2022.naacl-main.359). In *Proceedings of the 2022 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies*, pages 4875–4893, Seattle, United States. Association for Computational Linguistics.

# Acknowledgements

This work was supported by the Defence Innovation Agency (AID) of the Directorate General of Armament (DGA) of the French Ministry of Armed Forces, and by the ICO, _Institut Cybersécurité Occitanie_, funded by Région Occitanie, France.
