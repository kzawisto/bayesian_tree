# bayesian_tree

Decision tree that works well without need for parameter tuning and gives almost statistically meaningful splits. ATM is messy notebook.

This is work in progress, at the moment it produces comparable results to sklearn CART with hyperparameter optimization (see notebook) - without need for such parameter optimization or pruning. Goal is a testbed for  design of general statistical test that works for any number of treelike splits - which is a model for repeated hypothesis testing scenario. 

I built it independently, but later I that noticed current version is almost identical to what they give in paper: https://arxiv.org/pdf/1901.03214.pdf.

I reproduced result for Haberman dataset they report, but it is not, as they claim, big improvement over sklearn CART, but only big improvement over CART with default parameters. It is in fact on par with hyperparameter tuned CART (but without tuning required).
CART can give anything from 65 to 74% accuracy on this dataset. 

