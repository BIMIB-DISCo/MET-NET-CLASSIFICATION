# MET-NET-CLASSIFICATION

### Requirements 
* (1) [Python 3.8.x] Follow the instructions at: https://www.python.org/downloads/
* (2) [Jupyter] Follow the instructions at: https://jupyter.org/install
* (3) [scikit-learn 0.23] Run this command via PIP to install the proper version:

	<pre><code>pip install scikit-learn</code></pre>
	Further details at: https://scikit-learn.org/stable/index.html
 
 * (3) [pandas 0.25] Run this command via PIP to install the proper version:

	<pre><code>pip install pandas</code></pre>
	Further details at: https://pandas.pydata.org/
 
### Running
Please launch Jupyter from the terminal with the following command:
<pre><code>Jupyter notebook</code></pre>

Now, you can execute each cell to reproduce the results shown in the paper.

### Outputs 
The notebook produces a pandas dataframe with all the performance metrics used to perform the hyperparameters selection and to compare the classification methods.

# SYNTHETIC DATASETS
To reproduce the analysis of the paper we provide a file named R22_breast_cancer.csv in which each row is a sample and the columns include:

* (1) The first 5 PCs computed considering the expression profiles of the metabolic genes included in Recon2.2 [https://doi.org/10.1007/s11306-016-1051-4].
  
* (2) The threshold levels used to prune the networks

* (3) The topological properties extracted from each network

* (4) The cancer / normal ground truth sample labels
