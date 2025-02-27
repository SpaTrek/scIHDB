# scIHDB

**S**ingle-**C**ell **I**ntegrated **D**ata**b**ase of **I**schemic **H**eart Disease (**scIHDB**, https://xomics.com.cn/ihdb) is a comprehensive resource for ischemic heart disease that allows spatial and temporal interpretations. ScIHDB is composed of a single-cell atlas of IHD (**IHDAtlas**) encompassing over 1.4 million cells that can be categorized into 40 common cell types, and a IHD knowledge graph (**IHDKG**) with manually curated 6,035 CHD-related genes, 3,157 drugs, 80 comorbidities, and gene-disease associations and molecular interactions between them. To make scIHDB a reliable reference for IHD research, we performed collective meta-program (MP) analysis and generated 16 MPs associated with different murine disease models. Each MP is a representitive of a group of gene programs under disease states. Besides, a pipeline was constructed from a series of state-of-the-art computational tools to analyze each dataset individually. All analysis results, including differential gene expression, cell-cell interaction, pathway activeness, were visulized and publicly available on our website. Our IHDKG was so far the largest manually curated knowledge graph for ischemic heart disease. It provides the most genes, drugs, and gene-disease associations with supporting literature comparing to other dedicated databases. Besides, IHDKG is a "dynamic" knowledge graph with each gene been annotated with its significance in cell types under different disease conditions. Our website provides a network creation and manipulation tool for users to build subgraphs for download and further analysis with tools such as networkx and SNAP.

![资源 4cover letter2](https://github.com/user-attachments/assets/2cce839c-d261-46a8-b43e-eee208200dcf)


To run the single-cell RNA-seq pipeline, we suggest to install Anaconda on a Windows PC and create a new environment using the sc.yml configuration to install all related packages.
```
conda env create -f sc.yml -n sc
conda activate sc
```
Besides, an R environment should be configured to include all related packages. The required R packages include:
NMF==0.27
scry==1.16.0
scran==1.32.0
Biobase==2.62.0
iocParallel==1.36.0
