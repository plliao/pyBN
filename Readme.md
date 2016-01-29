<h1>Bayesian Networks in Python</h1>

<h2>Overview</h2>
This module provides a convenient and intuitive interface for reading/writing Discrete Bayesian Networks and performing fast inference over them. There seems to be a lack of many high-quality options for BNs in Python, so I hope this project will be a useful addition.

I am a graduate student in the Di2Ag laboratory at Dartmouth College, and would love to collaborate on this project with anyone who has an interest in graphical models -- the class structure and syntax is easy to pick up! Shoot me an email at ncullen.th@dartmouth.edu

<h2>Usage</h2>
Getting up-and-running with this package is simple:

1. Click "Download ZIP" button towards the upper right corner of the page.
2. Unpack the ZIP file wherever you want on your local machine. You should now have a folder called "pyBN-master"
3. In your python terminal, change directories to be IN pyBN-master. Typing "ls" should show you "data", "examples" and "pyBN" folders. Stay in the "pyBN-master" directory for now!
4. In your python terminal, simply type "from pyBN import ". This will load all of the module's functions, classes, etc.
5. You are now free to use the package! Perhaps you want to start by creating a BayesNet object using "bn = BayesNet()" and so on.

<h2>Examples</h2>
This package includes a number of examples to help users get acquainted with the intuitive syntax and functionality of pyBN. For an updated list of examples, check out the collection of ipython notebooks in the "examples" folder located in the master directory.

Here is a list of current examples:
- ReadWrite : an introduction to reading (writing) BayesNet object from (to) files, along with an overview of the attributes and data structures inherit to BayesNet objects.
- Drawing : an introduction to the drawing/plotting capabilities of pyBN with both small and large Bayesian networks.
- FactorOperations : an introduction to the Factor class, an exploration of the numerous attributes belonging to a Factor in
pyBN, an overview of every Factor operation function at the users' hands, and a short discussion of what makes Factor operations
so fast and efficient in pyBN.

<h2>Current features:</h2>

<h4>FileIO and Operations</h4>
| Reading BNS   | Drawing BNs   | Factor Operations |
| ------------- | ------------- | ----------------- |
| BIF format    | Graphviz Engine     | Factor Multiplication    |
| JSON format   | Networkx      | Factor Reduction     |
|				|				| Convert to/from log space |
|				|				| Normalize 			|

<h4>Inference</h4>
| Exact Marginal Inference  | Approximate Marginal Inference  | Exact MAP Inference |
| ------------- | ------------- | ----------------- |
| Sum-Product Variable Elimination   | Forward Sampling    | Max-Sum Variable Elimination   |
| Clique Tree Message Passing  | Likelihood Weighted Sampling     |     
|				|				| Gibbs (MCMC) Sampling 			|
|				|				| Loopy Belief Propagation			|

<h4>Learning</h4>
| Structure Learning   | Parameter Learning   | Independence Tests |
| ------------- | ------------- | ----------------- |
| Path Condition (PC) Algorithm   | Maximum Likelihood Estimation     | Marginal Mutual Information (KL-Divergence)    |
| Grow-Shrink (GS) Algorithm   | Bayesian Estimation     | Conditional Mutual Information (Cross Entropy)     |
| Chow-Liu Tree Algorithm			|				| Pearsion Chi-Square|
| Naive Bayes				|				| 			|


<h4 style="float:left">Reading BNs</h4>
- Bif format
- Json format

<h4 style="float:right">Drawing BNs</h4>
- Graphviz Engine
- Networkx (matplotlib/pylab) Engine

<h4 style="float:left">Fast Factor Operations</h4>
- Factor multiplication
- Factor reduction (sum out variables)
- Convert to/from log space
- Normalize

<h4 style="float:right">Approximate Marginal Inference</h4>
- Loopy Belief Propagation
- Forward Sampling
- Gibbs Sampliing
- Likelihood Weighted Sampling

<h4>Exact Marginal Inference</h4>
- Sum-Product Variable Elimination
- Clique Tree Message Passing

<h4>Exact MAP Inference</h4>
- Max-Sum Variable Elimination

<h4>Structure Learning</h4>
- Path Condition (PC) Algorithm
- Grow Shrink (GS) Algorithm
- Chow-Liu Tree Algorithm
- Naive Bayes

<h4>Conditional Independence Tests</h4>
- Marginal Mutual Information (i.e. KL-Divergence)
- Conditional Mutual Information (i.e. Cross Entropy)
- Pearson X^2

<h4>Parameter Learning</h4>
- Maximum Likelihood Estimator
- Bayesian Estimator

<h4>Classification</h4>
- Bayesian Network MAP Classification
- Naive Bayes Classification
- Tree-Augmented Naive Bayes Classification

<h4>Structure-based Distance Metrics</h4>
- Missing Edges
- Extra Edges
- Incorrect Edge Direction
- Hamming Distance

<h4>Parameter-based Distance Metrics</h4>
- Kullbach-Leibler Divergence
- Jensen-Shannon Divergence
- Hellinger
- Euclidean
- Manhattan
- Minkowski

