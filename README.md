# SmuDGE: semantic Disease-Gene embeddings



Python scripts to generate semantic features vectors of the disease and gene by utilizing model 
phenotypes and PPI network


## scripts


* smudge_P.groovy - script to generate corpus using phenomNet ontology

* smudge_E.py - script to generate the corpus and features vectors of genes and diseases by sampling 
from the node's surrounding environment, and extracting phenomNet ontology associated and superclasses 

* smudge_ann.py - script to run ANN in 5-fold from Keras package on the gnerated embeddings to evaluate gene-disease association

* smudge_logit.py - script to run Logistic regression on the gnerated embeddings to evaluate gene-disease association



## data

The files contain the features vector represenations of diseases and genes reprenseted in our hetergenous Knowledge graph (KG). The first column is the gene entrez ID or OMIM disease and the reset is the features values 

* E_vec_embeddings_human.txt - The Environment-based vector represenations (embeddings) based on human phenotypes for gene and diseases and genes nodes. 
* E_vec_embeddings_mouse.txt - The Environment-based vector represenations (embeddings) based on mouse phenotypes for genes and diseases nodes.
* P_vec_embeddings_human.txt - The Phenotype-based vector representations (embeddings) using mouse phenotypes for genes and diseases nodes.
* P_vec_embeddings_mouse.txt - The phenotype-based vector represnetations (embeddings) using mouse phenotype for genes and diseases nodes.

