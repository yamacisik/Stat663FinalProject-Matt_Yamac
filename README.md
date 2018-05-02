# Stat663FinalProject-Matt_Yamac
Final Project, Sta 663 Matt Welch and Yamac Isik 

# Bayesian Hierarchical Clustering

An hiearchichal clustering method which uses a multvariate normal distribution as a prior distribution. The clusters are formed based on the likelihood calculations for the Hypothesis of two different clusters belonging to a same cluster. For more information see :
http://www2.stat.duke.edu/~kheller/bhcnew.pdf

Package is downloadable and installable via pip

$ pip install bayes_cluster

or

$ pip install --index-url https://test.pypi.org/simple/ bayes_cluster

# Cluster Function

```python
  >>> from bayes_cluster import cluster
  >>> cluster.clust()
  >>> clust(X,alpha,kappa0,v0,mu0,eta0,k)
   ```
X: Features of the data set, must be a numpy array

alpha:parameter to be set based on the number of clusters

kappa0,v0,mu0,eta0 : See the report for explanations

k: number of clusters to be determined


Returns a numpy array y, and a tree node structure tree

y:numpy array giving the classifications of each observations

tree: A tree structure which uses nodes, can be further used in the impurity calculations

# Impurity Calculation
```python
  >>>from bayes_cluster import measures
  >>>measures.impurity(tree,yhat,y,n=500)
  ```

tree: tree node given by the algorithm

yhat: predictions of the classifications

y:original classification coming from the data set

n=number of iterations







