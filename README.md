# OCoClus - Overlapped Co-Clustering method

This is a project with the OCoClus implementation that finds non-overlapped and overlapped co-clusters.
Source code of the paper **A Frequent Pattern Based Approach for Mining Overlapped Co-clusters in Binary Data**, accepted for publication in ...

\[ [publication](https://#) ] \[ [preprint](./reference/preprint.pdf) ] \[ [bibtex](./reference/bibliography.bib) ]

Dummy text bellow ...

## Setup
A. dependencies version
  - Pandas: 0.25.1
  - Numpy: 1.16.4
  - Python: 3.7.1 | package by conda-forge [MSC v.1900 64 bit (AMD64)]
  - IPython: 7.8.0
  - IPython genutils: 0.2.0

```Shell
pip install -r ./dist/automatize/requirements.txt
```

Install R, and the dependent packages. To enter the R environment:

```Shell
sudo apt-get install r-base
R
```

Install `data.table` and `dplyr` packages, and exit.

```R
install.packages("data.table")
install.packages("dplyr")
q()
```

## What do you find in the project?
1. Directories
  - Data:
    * synthetic
    * real_application
    * ground_truth
    * toy_example

2. Jupyter notebooks
  * OCoClus-1 for synthetic data
  * OCoClus-2 for real data

## Usage

### 1. 

```Shell
-curpath "$BASIC_PATH" 
-respath "$RESULT_PATH" 
-descfile "$DESC_FILE"  
-version hiper
-nt 8
```


Where:
- `BASIC_PATH`: The path for the input CSV training and test files.
- `RESULT_PATH`: The destination folder for CSV results files.
- `DESC_FILE`: Path for the descriptor file. File that describes the dataset attributes and similarity measures.
- `-version`: Method to run (hiper, hiper-pvt, ...)
- `-nt`: Number of threads

    
### 2. For instance:

To run the XXX you can run the java code with the following default entries as example:


```Shell
java -Xmx80G -jar HIPERMovelets.jar 
-curpath "$BASIC_PATH" -respath "$RESULT_PATH" -descfile "$DESC_FILE" 
-version hiper -nt 8 -ed true -samples 1 -sampleSize 0.5 -medium "none" -output "discrete" -lowm "false" -ms 1 -Ms -3 | tee -a "output.txt"
```


This will run with 80G memory limit, 8 threads, and save the output to the file output.txt`. 

It is the same as (without the output file):


```Shell
java -Xmx80G -jar HIPERMovelets.jar 
-curpath "$BASIC_PATH" -respath "$RESULT_PATH" -descfile "$DESC_FILE" 
-version hiper -nt 8
```

# License


# Acknowledgments
This work was financed  by the Brazilian agencies Coordenação de Aperfeiçoamento de Pessoal de Nivel Superior - CAPES, Finance code 001, and Conselho Nacional de Desenvolvimento Científico e Tecnológico - CNPq.
