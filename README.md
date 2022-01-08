# bayesian_tree

Decision tree that works well without need for parameter tuning and gives mostly meaningful splits (in a sense of Bayesian hypothesis testing)
This is work in progress, at the moment it produces comparable results to sklearn CART with hyperparameter optimization (see notebook) - without need for such parameter optimization or pruning. Goal is a testbed for  design of general statistical test that works for any number of treelike splits - which is a model for repeated hypothesis testing scenario. 

Built independently. Later I noticed that current version is almost identical to what they give in paper: https://arxiv.org/pdf/1901.03214.pdf.

I reproduced result for Haberman dataset they report, but it is not clear if, as they claim, it is big improvement over sklearn CART - as they compare to default parameter version. CART can give anything from 65 to 74% accuracy on this dataset, while this model gives about 72%. 

