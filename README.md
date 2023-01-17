# Comp790-166 Computational Biology (Spring 2023)

## Details

Instructor: Natalie Stanley

Email: natalies@cs.unc.edu

Time and Place: Monday/Wednesday 11:00am-11:15am in Fred Brooks 007 (FB007). 

Info and Attributes: This is a 3-credit full-semester course and fulfills the 'Applications' category for CS students. It is a lecture-style class (I will teach the lectures) and includes two homework assignments and a course project. **Please make sure you selected the 3-credit option when you enrolled.** 

Office Hours: Tuesday 2:15pm-3:15pm. 

## Description
Modern, high-throughput assays allow us to efficiently profile a variety of biological processes to gain a systems-level understanding of health and disease. Recent technologies and experimental assays generate an abundance of detailed information that needs to be extracted, summarized, and interpreted. In this course we will discuss the methodology used to extract signal from (e.g. process, engineer features from, combine, etc.) data generated by some of the most cutting-edge technologies, such as single-cell assays and imaging. We will go into detail about the methods and theory underlying bioinformatics algorithms, originating from numerical linear algebra, graph-signal processing, and machine learning. While computational biology is a very broad field, we will focus here on applications in single-cell biology (CyTOF, single-cell RNA sequencing), multiomics/multi-modal analysis, systems immunology, and benchmarking. For each class of algorithms introduced for some task on biological data, we will also go over necessary theory and mathematical intuition. The course covers the foundations for biomedical data science and does not assume any biological knowledge.

## Syllabus and Course Structure
Please see the following link for a syllabus and information about key dates, homework, and the course project. [[Syllabus 2023](https://github.com/natalies-teaching/CompBio2023/blob/main/Syllabus.pdf)]. Note that this is a lecture course with two homework assignments and a course project. 

# Topics and Tentative Schedule. 

This is the preliminary set of topics. 


| Date | Topic | Reading | Notes | Code |
|------|-------|---------|-------|------|
|Monday, Jan 9 | Intro, Bioinformatics vs Computational Biology| [[Systems Immunology, Just Getting Started](https://www.nature.com/articles/ni.3768)], [[Grand Challenges in Single-Cell Data Science](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-1926-6)] | [[Lecture 1](https://github.com/natalies-teaching/CompBio2023/blob/main/Lectures/Lecture1.pdf)]  | 
|Wednesday, Jan 11| Linear Algebra Review, Matrix Rank, Building Graphs from Data, Graph Laplacian, Graph Diffusion | [[SLMP. pages 10-22](https://arxiv.org/abs/2004.07984)], [[Data Matrices + Low Rank](https://arxiv.org/abs/1705.07474)] | [[Lecture 2](https://github.com/natalies-teaching/CompBio2023/blob/main/Lectures/Lecture2.pdf)]  | [[graph tools for python](https://github.com/KrishnaswamyLab/graphtools)] |
|Monday, Jan 16| No Class - MLK Day | | | 
|Wednesday, Jan 18| Finish defining Graph Laplacian and Properties ; Building graphs from data; graph visualization and dimension reduction; graph partitioning intro ; modularity-based graph partitioning | [[LargeVis](https://arxiv.org/abs/1602.00370)], [[Random Projection Trees](https://cseweb.ucsd.edu/~dasgupta/papers/rptree-stoc.pdf)], [[Fast Unfolding of Communities in Large Networks](https://arxiv.org/abs/0803.0476)], [[Module Detection Benchmarking in Biological Data](https://www.nature.com/articles/s41592-019-0509-5)] | [[Lecture 3](https://github.com/natalies-teaching/CompBio2023/blob/main/Lectures/Lecture3.pdf)] | [[SNAP](https://snap.stanford.edu/)], [[Louvain](https://github.com/vtraag/louvain-igraph)], [[Leiden](https://github.com/vtraag/leidenalg)] 
|Week 3-1| Probabilistic graph partitioning (SBM, Affiliation Model)); Graph Embeddings with node2vec (such as node2vec)  | [[BigClam](https://dl.acm.org/doi/abs/10.1145/2433396.2433471)], [[SBM for Single-Cell](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04489-7)], [[Node2Vec](https://dl.acm.org/doi/pdf/10.1145/2939672.2939754?casa_token=vQTboPUL6qIAAAAA:XQsAUtXd4MyWfj1ClUBw8FKhuPbpqO-aE2d7EDs5iX9-jJZP9BuxDbKUjg3CM69YKHALjCAKJtJx)], [[Representation Learning on Graphs](https://arxiv.org/abs/1709.05584)], [[Review: Graph Embedding in Comp Bio](https://www.frontiersin.org/articles/10.3389/fgene.2019.00381/full)]]  |  |  [[graph-tool (SBM)](https://graph-tool.skewed.de/)], [[node2vec](https://github.com/aditya-grover/node2vec)] | 
|Week 3-2| Single Cell Day 1: Intro to Single-Cell {Data Structure, Technologies, Pre-Processing}, Automating Gating and Cell-Population Discovery in Single Cell Data| [[Spade](https://www.nature.com/articles/nbt.1991)], [[Single-Cells, Many Features](https://www.sciencedirect.com/science/article/pii/S009286741630410X)] |   | [[FCS file tutorial](https://github.com/stanleyn/fcs_tutorial)], [[Spade](https://github.com/nolanlab/spade)]   |
|Week 4-1| Graph-based automated gating, imputation in single-cell data|  [[phenograph](https://www.sciencedirect.com/science/article/pii/S0092867415006376)] |  | [[phenograph](https://github.com/JinmiaoChenLab/Rphenograph)],  [[FastPG](https://github.com/sararselitsky/FastPG)] |
|Week 4-2| Imputation for single-cell data, Branch Preserving Visualization for Single-Cell Data| [[MAGIC](https://www.biorxiv.org/content/10.1101/111591v1)],[[PHATE](https://www.nature.com/articles/s41587-019-0336-3)],  |  |   [[MAGIC](https://github.com/KrishnaswamyLab/MAGIC)],[[Phate](https://github.com/KrishnaswamyLab/PHATE)]  | 
|Week 5-1| Branch Preserving Visualizating for Cellular Differentiation, Data Augmentation for Single Cell Identifying prototypical cells of a particular experimental condition with graph signal processing| [[SUGAR](https://papers.nips.cc/paper/2018/hash/c8ed21db4f678f3b13b9d5ee16489088-Abstract.html)] |  | [[sugar](https://github.com/stanleyjs/sugar)] | 
|Week 5-2| Finish data augmentation for sparse single-cell landscapes, start graph signal processing background|[[Graph Signal Processing Review Article](https://web.media.mit.edu/~xdong/paper/spm20.pdf)],[[MELD](https://www.biorxiv.org/content/10.1101/532846v4)] |  | [[MELD](https://github.com/KrishnaswamyLab/MELD)] [[pyGSP](https://pygsp.readthedocs.io/en/stable/)] |
| Week 6-1 | Finish introducing graph signal processing, low-pass filtering, MELD for selecting condition-specific prototypical cells | See references from Monday. Also, [[The Emerging Field of Graph Signal Processing](https://arxiv.org/abs/1211.0053)] |  | |
|Week 6-2| Finish up GSP background, Identifying condition or experimentally-specific prototypical cells with Meld, Start Differential Abundance Analysis with Cydar | [[Cydar](https://www.nature.com/articles/nmeth.4295)] |  | [[cydar](https://www.bioconductor.org/packages/release/bioc/html/cydar.html)] |
|Week 7-1| Differential Abundance Day 2. Cydar,  Milo| [[Milo](https://www.nature.com/articles/s41587-021-01033-z)] |  |  [[Milo](https://github.com/emdann/milopy)] | 
|Week 7-2| Finish differential abundance analysis (Milo and Cydar), Contrastive PCA for dealing with background data | [[Contrastive PCA](https://www.nature.com/articles/s41467-018-04608-8)] |  | [[Contrastive PCA](https://github.com/abidlabs/contrastive)] |
|Week 8-1| Trajectory inference | [[PAGA](https://link.springer.com/article/10.1186/s13059-019-1663-x)], [[A Comparison of Single-Cell Trajectory Inference Methods](https://www.nature.com/articles/s41587-019-0071-9)], [[Slingshot](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-018-4772-0)]. |  | [[PAGA](https://scanpy.readthedocs.io/en/stable/generated/scanpy.tl.paga.html)] | 
|Week 9-1| Batch 1 of project presentations | |
|Week 9-2| Batch 2 of project presentations |  |
|Week 10-1| Spring Break -- No class! |
|Week 10-2| Spring Break -- No class! | 
|Week 11-1| Finish differential abundance analysis (Milo), Contrastive PCA, Merging Multiple Single-Cell Datasets (Conos) | [[Conos](https://www.nature.com/articles/s41592-019-0466-z)] |  | [[Conos](https://github.com/kharchenkolab/conos)] |
|Week 11-2| Pseudotime, Diffusion, and Cellular Differentiation | [[Diffusion Maps for Differentiation](https://academic.oup.com/bioinformatics/article/31/18/2989/241305)], [[SLICER-developed at UNC](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0975-3)], [[Original Diffusion Maps (Coifman)](https://papers.nips.cc/paper/2005/file/2a0f97f81755e2878b264adf39cba68e-Paper.pdf)] |  | [[Diffusion Maps -Scanpy](https://scanpy.readthedocs.io/en/latest/api/scanpy.tl.diffmap.html)], [[SLICER](https://github.com/jw156605/SLICER)]  | 
|Week 12-1| Last single-cell lecture. Branching trajectories with SLICER. Begin combining biological data from multiple modalities using Grassmann Embeddding| [[Subspace Merging on Grassmann Manifold](https://academic.oup.com/bioinformatics/article/35/10/1653/5134062?login=true)], [[Rayleigh Ritz Business (Spectral Clustering...](https://arxiv.org/abs/0711.0189)] |  | [[Grassmann Cluster](https://github.com/michaelsharpnack/GrassmannCluster)] | 
|Week 12-2| Finish multimodal data integration with Grassmann + Rayleigh Ritz, Start MOFA integration | [[MOFA](https://www.embopress.org/doi/full/10.15252/msb.20178124)], [[MOFA+](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-02015-1)] |  | [[MOFA](https://github.com/bioFAM/MOFA)] |
|Week 13-1| Integrating multiple heterogeneous graphs (e.g. multiple relational definitions) | [[Mashup](https://www.cell.com/cell-systems/fulltext/S2405-4712(16)30360-X?)] |  | [[Mashup](http://cb.csail.mit.edu/cb/mashup/)] | 
|Week 13-2| Graph Alignment and Summarization| [[REGAL (graph alignment)](https://gemslab.github.io/papers/heimann-2018-regal.pdf)], [[Refining Network Alignment](https://gemslab.github.io/papers/heimann-2021-RefiNA.pdf)] |   | [[REGAL](https://github.com/GemsLab/REGAL)], [[RefiNA](https://github.com/GemsLab/RefiNA)] |
|Week 14-1| Graph Alignment Refinment, Summarization, and Compression | See papers from last time | |
|Week 14-2| Label Propagation and Graph Neural Networks   | [[Correct and Smooth](https://arxiv.org/abs/2010.13993)] |  |
|Weel 15-1 | Imaging Omics and Spatial Modalities |[[LEAPH](https://www.cell.com/cell-reports-methods/pdfExtended/S2667-2375(21)00124-7)] |  | 
|Wednesday, April 20| Technical Writing in Comp Bio and Wrap-Up, Summary of the Semester wrt to graphs in biomedicine | [[Watch : How to be a Machine Learning Biologist](https://www.youtube.com/watch?v=xueh6WnpRDQ&t=1651s)], [[Graph Representation Learning in Biomedicine](https://arxiv.org/abs/2104.04883)] |  |
|Week 15-2| Project Presentations Day 1 |
|Week 16-1| Project Presentations Day 2|
|Final Project| Final Project Writeups Due

# Reading Questions

**Please choose 2 papers over the course of the semester to do this for, and turn them in before our class meeting 11am to natalies+comp790@cs.unc.edu**. 

1) Please explain in 2 sentences or less what the problem being solved is.

2) What were the main contributions of the authors in this work? (You can answer in a few bullet points). 

3) Please describe 1-2 computational experiments that the authors implemented to test their method.

4) Were the authors the first to attempt this particular problem? If not, did they compare their results to other baselines? Do you think that their evaluation was objective?

5) Do you think that the authors provided enough evidence for why their developed method is an important contribution? If yes, please describe their reasoning here. If you do not think they adequately justified why they worked on this particular problem, please describe your thoughts on that here. 

6) What is one follow-up idea or extension from this work? 
