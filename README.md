# OCoClus - <i>O</i>verlapped <i>Co</i>-<i>Clus</i>tering method

This is a project with the OCoClus implementation that finds non-overlapped and overlapped co-clusters.
Source code of the paper **A Co-occurrence Based Approach for Mining Overlapped Co-clusters in Binary Data**, accepted for publication in BRACIS-21.

[Access the paper here!](https://link.springer.com/chapter/10.1007%2F978-3-030-91702-9_25) <!--\[ [preprint](./reference/preprint.pdf) ] \[ [bibtex](./reference/bibliography.bib) ]-->

## Setup
A. Packages and dependencies version
  - Pandas: 0.25.1
  - Numpy: 1.16.4
  - sklearn: 0.21.2
  - Python: 3.7.1 | package by conda-forge [MSC v.1900 64 bit (AMD64)]
  - IPython: 7.8.0
  - IPython genutils: 0.2.0

Please, install the minor dependencies that your jupyter notebook may require.

## What do you find in the project?
1. Directories
  - Data: It contains the datasets
    * synthetic: It has the synthetic datasets used in the experimental analysis.
    * real_application: It has the real datasets used to exemplify the efficacy of our method.
    * toy_example: It has two simple files that the reader can use to play with our method.
  - OutputAnalysis: It has the clustering output files per simulation for each synthetic dataset.
  - xmeasures: It has the ground-truth and clustering output files used for evaluation.
  - Supplementary material: It has the clustering outputs of each method used to compute the evaluation scores from the xmeasures project. These scores are reported in the paper. Moreover, we provide the xlsx files with the evaluation scores obtained in each run.

2. Jupyter notebooks
  * overlapped_coclustering_synthetic.ipynb: It is the OCoClus method. The reader can run it for synthetic and real data experiment.
  * experimental_baselines.ipynb: In this notebook, we provide the methods reported in the paper used in comparison with our method.

## Usage

Please, install all dependencies, run the support functions in the block cells, then run the main method.


# License

- MIT


# Acknowledgments

This work was financed  by the Brazilian agencies Coordenação de Aperfeiçoamento de Pessoal de Nivel Superior - CAPES, Finance code 001, and Conselho Nacional de Desenvolvimento Científico e Tecnológico - CNPq.
