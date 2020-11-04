# MET-NET-CLASSIFICATION

### Requirements 
* (1) [Python 3.8.x] Follow the instructions at: https://www.python.org/downloads/
* (2) [Jupyter] Follow the instructions at: https://jupyter.org/install
* (3) [scikit-learn 0.23] Run this command via PIP to install the proper version:

	<pre><code>pip install scikit-learn</code></pre>
	Further details at: https://scikit-learn.org/stable/index.html
 
* (4) [pandas 0.25] Run this command via PIP to install the proper version:

	<pre><code>pip install pandas</code></pre>
	Further details at: https://pandas.pydata.org/
	
* (5) [tqdm] Run this command via PIP to install the proper version:

	<pre><code>pip install tqdm</code></pre>
	Further details at: https://github.com/tqdm/tqdm
	 
### Running
Please launch Jupyter from the terminal with the following command:
<pre><code>Jupyter notebook</code></pre>

Now, you can simply execute each cell to reproduce the results shown in the paper [xxx].

### Outputs 
The notebook populates a pandas dataframe with all the performance metrics used to perform the hyperparameters selection and to compare the classification methods.

# BREAST CANCER DATASETS
We considered 105 breast cancer patients with gene expression profile obtained from either cancer and normal/health tissue, for a total of 210 gene expression profiles (source TCGA-BRCA database).

In the *breast_cancer_expression* directory one can find those data in two compressed files, one includes cancer and one includes normal samples.

To reproduce the classification analysis we provide in *data* directory also a file named R22_breast_cancer.csv in which each row is a sample and the columns include:

* (1) The first 5 PCs computed considering the expression profiles of the metabolic genes included in Recon2.2 [https://doi.org/10.1007/s11306-016-1051-4].

* (2) The extracted topological properties from each network pruned with a given threshold.

* (3) The cancer / normal ground truth sample labels

