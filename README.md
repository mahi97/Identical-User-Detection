# Identical-User-Detection
A Case study to find identical authors in the graph of user_id and paper_id relations

Documents and Cleaning the Code is a WIP.


## TL;DR

There exists 64K author id and 420K paper id.
There is no additional information besides graph structure between author ids and paper ids.
1k positive cases are given, and 1k validation cases should be classified. There are 3k positive cases in total.

We used graph classification over the sub-graph between author id to decide whether two ids belong to the same author or not.
Although this sub-graph is a local view, we used global information to generate features for nodes.

Sampling strategy for negative cases is critical. We use many different techniques to develop good sampling that shows promising performance while avoiding overfitting to reach generalization.
