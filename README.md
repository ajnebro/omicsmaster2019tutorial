# Tutorial: "Multi-objective optimization with metaheuristics. Applications to Bioinformatics"

This site contains stuff to be used in the tutorial I will give in the Omics Data Analysis Master of the University of Vic on 31th January 2019.

In this tutorial we will learn:
* What are metaheuristic techniques and why they are useful.
* Issues related to optimizing problems having more tan one objective function (multi-objective optimization problems).
* How to use the [jMetalPy optimization framework](https://github.com/jMetal/jmetalpy) to solve both single and multi-objective optimization problems.
* To assess the quality of aligned sequences with the [pyMSA software](https://github.com/benhid/pyMSA). 
* To apply metaheuristics to deal with multi-objective formulations of the multiple sequence alignment problem using [Sequoya](https://github.com/benhid/Sequoya).

## Recommended readings

* Metaheuristics in combinatorial optimization: Overview and conceptual comparison. C. Blum, A. Roli. ACM Computing Surveys Volume 35 Issue 3, September 2003. [DOI](https://doi.org/10.1145/937503.937505).

* An Introduction to Evolutionary Algorithms. Shahim Rostami. [Video](https://www.youtube.com/watch?v=L--IxUH4fac). 

*  Multiobjective optimization in bioinformatics and computational biology. J. Handl, DB Kell, J Knowles. 
IEEE/ACM Transactions on Computational Biology and Bioinformatics (2), 279-292. 2007. [DOI](https://doi.org/10.1109/TCBB.2007.070203)

* Optimizing multiple sequence alignments using a genetic algorithm based on three objectives: structural information, non-gaps percentage and totally conserved columns. F.M. Ortuño et al. Bioinformatics, Volume 29, Issue 17, 1 September 2013, Pages 2112–2121. [DOI](https://doi.org/10.1093/bioinformatics/btt360).

* M2Align: parallel multiple sequence alignment with a multi-objective metaheuristic. C. Zambrano-Vega, A.J. Nebro, J. García-Nieto, J.F. Aldana-Montes. Bioinformatics, Volume 33, Issue 19, 1 October 2017, Pages 3011–3017. [DOI](https://doi.org/10.1093/bioinformatics/btx338).

## Software requirements
* Python (Anaconda Python 3.6+): https://www.anaconda.com/download/ 
* PyCharm Community Edition:  https://www.jetbrains.com/pycharm/download/
* Git (https://git-scm.com/) and an account in GitHub
* jMetalPy:  https://github.com/jMetal/jMetalPy
* pyMSA: https://github.com/benhid/pyMSA
* Sequoya: https://github.com/benhid/Sequoya
* Gnuplot, R, … to plot data

## Videos for installing the required software
* [Installation of Anaconda Python and Pycharm](https://uma365-my.sharepoint.com/:v:/g/personal/ajnebro_uma_es/EZ8VQ82Q2NJAs6tOYjoOc0sBMoke57pt-wN4TSERQo0TKg?e=6VqHof) (Linux)
* [Installation of jMetalPy](https://uma365-my.sharepoint.com/:v:/g/personal/ajnebro_uma_es/EW-de6Lcyq1Jli9Zrk6og6UB6Er_PKFX0lddOc6812B0Lw?e=52dI6p) (Linux)

## Fast installation guide
```
# Create a directory to install the software projects
(base) F:\>mkdir masteromics
(base) F:\>cd masteromics
(base) F:\masteromics>

# Create a Conda virtual environment
(base) F:\masteromics>conda create -n omics python=3.6
...

# Activate the environment
(base) F:\masteromics>conda activate omics
(omics) F:\masteromics>

# Clone pyMSA
(omics) F:\masteromics>git clone https://github.com/benhid/pyMSA
Cloning into 'pyMSA'...
remote: Enumerating objects: 40, done.
remote: Counting objects: 100% (40/40), done.
remote: Compressing objects: 100% (28/28), done.
remote: Total 299 (delta 16), reused 28 (delta 12), pack-reused 259Receiving objects:  97% (291/299), 956.01 KiB | 1.76 Receiving objects:  98% (294/299), 956.01 KiB | 1.76 MiB/s
Receiving objects: 100% (299/299), 1.37 MiB | 1.76 MiB/s, done.
Resolving deltas: 100% (151/151), done.
(omics) F:\masteromics>

# Install pyMSA
(omics) F:\masteromics>cd pyMSA
(omics) F:\masteromics\pyMSA>python setup.py install
...

# Clone jMetalPy
(omics) F:\masteromics\pyMSA>cd ..
(omics) F:\masteromics>git clone https://github.com/jmetal/jMetalPy
Cloning into 'jMetalPy'...
remote: Enumerating objects: 330, done.
remote: Counting objects: 100% (330/330), done.
remote: Compressing objects: 100% (224/224), done.
Rremote: Total 8425 (delta 209), reused 184 (delta 106), pack-reused 8095
Receiving objects: 100% (8425/8425), 11.30 MiB | 2.90 MiB/s, done.
Resolving deltas:  80% (4568/5708)
Resolving deltas: 100% (5708/5708), done.
(omics) F:\masteromics>

# Install jMetalPy
(omics) F:\masteromics>cd jMetalPy
(omics) F:\masteromics\jMetalPy>python setup.py install
... 

# Clone Sequoya
(omics) F:\masteromics\jMetalPy>cd ..
(omics) F:\masteromics>git clone https:/(github.com/benhid/sequoya

(omics) F:\masteromics\jMetalPy>cd ..

(omics) F:\masteromics>git clone https://github.com/benhid/sequoya
Cloning into 'sequoya'...
...

```

