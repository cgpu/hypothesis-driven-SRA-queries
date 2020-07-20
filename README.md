# Jupyter notebook-based tools for building structured datasets from the Sequence Read Archive

This repository implements a pair of Jupyter notebook-based tools that utilize the [MetaSRA](http://metasra.biostat.wisc.edu) for building structured datasets from the [SRA](https://www.ncbi.nlm.nih.gov/sra) in order to facilitate secondary analyses of the SRA’s human RNA-seq data: 
* *[Case-Control Finder:](https://github.com/mbernste/hypothesis-driven-SRA-queries/blob/master/case_control_finder.ipynb)* Finds suitable case and control samples for a given disease or condition where the cases and controls are matched by tissue or cell type.  
* *[Series Finder:](https://github.com/mbernste/hypothesis-driven-SRA-queries/blob/master/series_finder.ipynb)* Finds ordered sets of samples for the purpose of addressing biological questions pertaining to changes over a numerical property such as time. 

For a more in depth description of these tools, please see our publication: 

[Bernstein, M.N. et al. (2020). Jupyter notebook-based tools for building structured datasets from the Sequence Read Archive. F1000Research, 9:376](https://f1000research.com/articles/9-376/v1#article-reports)


A few things to note:
* These notebooks currently utilize the MetaSRA version 1.6. 
* This repository was copied and modified from the following repository: [https://github.com/NCBI-Hackathons/RNA-Seq-in-the-Cloud/tree/master/Metadata](https://github.com/NCBI-Hackathons/RNA-Seq-in-the-Cloud/tree/master/Metadata). These tools were developed at an NCBI computational biology codeathon in March 2019 held in Chapel Hill, North Carolina.

###  Setup

The dependencies for these notebooks are described in ``requirements.txt``.  To install these dependencies, please run

``pip install -r requirements.txt``

Furthermore, before running the notebook, you must unpack the static metadata files from ``data.tar.gz``. To do so, run the following command:

``tar -zcf data.tar.gz``

### Running the notebooks

To run the Case-Control Finder, run:

``jupyter notebook case_control_finder.ipynb``

To run the Series Finder, run:

``jupyter notebook series_finder.ipynb``


### Contributors
* Matthew Bernstein 
* Emily Clough
* Ariella Gladstein
* Khun Zaw Latt
* Ben Busby
* Allissa Dillman
