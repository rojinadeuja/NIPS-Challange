# NIPS-Challenge
Feature Selection Challenge by Neural Information Processing Systems (NIPS)

**DATA SET:** MADELON is an artificial dataset containing data points grouped in 32 clusters placed on the vertices of a five-dimensional hypercube and randomly labeled +1 or -1. The five dimensions constitute 501 features. The dataset was obtained from the UCI Machine Learning Repository [1] [http://archive.ics.uci.edu/ml/datasets/madelon]

**PROBLEM STATEMENT:** Feature selection is the process of picking those attributes in our dataset (such as columns in a tabular data), which are of most relevance to a problem at hand. For e.g., if we are trying to differentiate a human from a cat, the number of feet would be a relevant feature in our prediction. Although it is possible to select the features using some prior knowledge and other manual techniques, it is not always feasible. Many times, when carrying out feature selection we might be biased with our assumptions while selecting a feature or there may be too many features in a dataset to be conveniently filtered out.

**MOTIVATION:** We derive our motivation for choosing this problem through the **"Occam's razor (or Ockham's razor)"** principle. It is a problem-solving principle from philosophy which says that if there exist two explanations for an occurrence, the one that needs the smallest number of assumptions is usually correct. i.e. The more assumptions that you have to make, the higher the chances that it is an unlikely explanation.
Our motivation also stems largely from modelling various machine learning problems in our assignments. Even though we use statistical methods like observing the co-linearity of the variables, it might not be sufficient for making our proposed set of features the most optimal. Also going back and forth to confirm the increase or decrease in accuracy upon selecting our features to decide if we should drop a feature after creating the whole model is not an efficient technique.

**PROPOSED STEPS:** Since our target variable is a two-class variable, we will be presenting this task as a Classification problem. For creating the feature selection model, we propose on exploring two main methodologies:
Stepwise regression: In this method, we take all the features as candidate features. They are checked over each iteration to observe their influence on the target variable. If the feature is found to be of a significance lower than our tolerance level, it will not be selected further for creating the model.
Tree-based selection: Here, we borrow the concepts from Decision trees (e.g. Random Forest Trees). In tree-based feature selector, we split and traverse at each node based on the information gain given by a feature. The feature which gives maximum information gain is picked as the next branch in our path towards the final model.


If github is unable to render a Jupyter notebook, copy the link of the notebook and enter into the nbviewer: https://nbviewer.jupyter.org/
