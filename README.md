# Causal_Learn_Hackathon
This is a repository for the task [Causal Discovery for Cancer](https://uk-ai.org/e-hackathon-march-2023/materials/problem_1/causal_discovery_cancer.html) in the [Turing AI Fellow Hackathon event](https://uk-ai.org/e-hackathon-march-2023/) 

Task introduction & significance
Cancer is a genetic disease. It is caused by changes in genes that control the way cells grow and multiply. Somatic genomic alterations (SGAs) in DNA are largely responsible for initiating cancer. In particular, SGAs cause cancer through differential expression of genes (DEGs). Those SGAs that cause DEGs are good candidates as drivers of cancer.

Causal discovery for cancer is an important and challenging biomedical problem. Computational methods and machine learning are driving the development of new algorithms that meet the needs of biomedical researchers. The ability to discover and model causal relationships accurately is a key step in more fully realizing precision cancer diagnosis, prognosis, and therapy. The task is to identify SGAs that cause the DEGs in breast cancer.

The dataset provided for this Hackathon is the [Mini-TCGA Cancer Dataset](http://www.ccd.pitt.edu/wp-content/uploads/2019/06/cancer_data.txt) from the [Center for Causal Discovery](https://www.ccd.pitt.edu/biomedical-science/).

The Mini-TCGA Cancer Dataset contains data of Somatic Genomic Alteration (SGA) and Differentially Expressed Gene (DEG).

SGA indicates both nonsynonymous somatic mutations and copy number alterations; a gene sequence variable is coded as 1 if altered (SGA ) and 0 if not (not SGA). The selected 6 SGAs in the dataset are well known breast cancer drivers.

DEG indicates which genes are differentially expressed, relative to a baseline (e.g., normal tissue); DEG = 1 means a gene is differentially expressed, e.g. expression more than 2 SD from mean of normal-cells distribution. Otherwise DEG = 0. The selected 60 DEGs are most frequently regulated by the SGAs according to the TCI algorithm.

This [Jupyter notebook](https://colab.research.google.com/drive/1LL-gsrJ7fdx4BosBQT9OM1Z5RBBw0g3y?usp=sharing) shows how to load toy data and the Mini-TCGA Cancer data, as well as a few demos to call an off-the-shelf algorithm (e.g. fast greedy equivalence search (GES)) for causal discovery, i.e. predict a Directed Acyclic Graph (DAG) from the data.

Helpful tools & resources
Please feel free to explore these tools and resources. It is feasible to choose a method from these references to address the task. You may also consider further development upon the chosen method and apply it to the tasks. Alternatively, you may develop your own methods for the task.

* [Causal-learn documentation](https://causal-learn.readthedocs.io/en/latest/index.html)

* [Causal-learn and benchmarks](https://www.cmu.edu/dietrich/causality/causal-learn/)

* [Center for causal discovery](https://bd2kccd.github.io/docs/)

* [Center for causal discovery - Biomedical science](https://www.ccd.pitt.edu/biomedical-science/)

* [Causal discovery toolbox](https://github.com/FenTechSolutions/CausalDiscoveryToolbox)
