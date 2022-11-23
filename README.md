# Decision-tree-math-and-intuition


# what is Decision Tree?

Decision tree is a hierarchical tree structure that can be used to split an extensive collection of records into smaller sets of the class by implementing a sequence of simple decision rules.
- It also know as CART classification and regression trees

# Basic terminology of decision tree

![image](https://user-images.githubusercontent.com/110124468/203445838-ca6772f4-0899-47c8-8962-aac8f3e15962.png)

# Example of Decision Tree classfier

![decT](https://user-images.githubusercontent.com/110124468/203446621-dabff4c1-cb64-4a5c-a91d-b0819ebebbdc.png)

# New Query point given

![DT2](https://user-images.githubusercontent.com/110124468/203446811-37a01eb2-0131-4481-9ea7-21261d7119c2.png)


# Example of Decision Tree Regressor

![RDT](https://user-images.githubusercontent.com/110124468/203447223-233c7dfd-b005-4226-b2b3-33d3b93aebda.png)


# Geometric intuition
![DT3](https://user-images.githubusercontent.com/110124468/203447783-0de70a56-130b-46e1-85f5-c92eb8b24ac6.png)


# Steps

- Begins with your training dataset, which should have some features and lasssfiction and regression output variable.
- Determine the "Best Feature " in thwe dataset to split the data on; more on how to define " best feature" later.
- Split the data into subsets that contains the correct values for this best feature.This splitting basically defines a node on the tree. i.e each node is a spliting point based on certain features from our data.
-  Recursively generate new tree nodes by using the subset of created from step 3.


# Conclusion 

Programatically:- Decision trees are noting but a giant structure of nested if-selse statement condition

Mathmatically:- DT use hyperplanes which run parallel to any of the one axies to cut your coordinates system into hyper cuboids. 

# Some question 

1. How to decide which column shoud be considered as root node ?
2. How to select subsequent decision tree ?
3. How to decide splitting criteria in case of numerical columns ? 


# Disadvantages of DT

- Overfitting
- prone to errors for imbalanced datasets



# Decision Tree Entropy 

**The measure of disorder**. Or you can also call it the measure of purity / impurity.

# Entropy calculation
we can use both log2 and loge
![Entrpy](https://user-images.githubusercontent.com/110124468/203451636-ebed9e14-411c-484c-89f4-3320e1116cbb.png)

# gini impurity  (By defalut in sklearn)

Gini Impurity is a measurement used to build Decision Trees to determine how the features of a dataset should split nodes to form the tree.

![image](https://user-images.githubusercontent.com/110124468/203452948-17fac694-f109-43e6-87f3-795bafea9670.png)

**In the image above,  has minumum gini impurity, so  is selected as the root in the decision tree.

![giniimp](https://user-images.githubusercontent.com/110124468/203453149-e6e37862-5f9a-43f7-97f2-97db75f7e5e0.png)

The only practical difference between Entropy and Gini lies in the formula, and as a result, Gini ranges between 0 and 0.5, and Entropy between 0 and 1. In both cases, values closer to 0 indicate greater purity of the nodes, and values near the upper bound employ more impurity. 

# ENTROPY
![image](https://user-images.githubusercontent.com/110124468/203454029-8be2053f-e4a8-4793-882c-ea62677424d4.png)
 
 # Gini
 # ![image](https://user-images.githubusercontent.com/110124468/203454104-b7c9f174-bf9f-4964-8550-e603f01e8a1c.png)


# Information gain
Information Gain refers to the decline in entropy after the dataset is split. It is also called Entropy Reduction
This meaure the quality of a split.




# Hyper parameters in Decision tree classifiers/regressor

https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbngza0hWYTRwTHRMN1Z0MFNxRHRlWUFaY2lIZ3xBQ3Jtc0trZTRvMTg1QWlvVUg1bnd0MWNFQ3pVc0VuVlJEYnRDTXhqTldHd0dib29kcHY3eXR6cVlIWFNaeFotaW9RMHZOQWdIZUdkcGpaQ01iWGxzX1c5c2NWbHZwYjFTV09LTzJSZXN2YlZhU1JGbTFwbkY4QQ&q=https%3A%2F%2Fdt-visualise.herokuapp.com%2F&v=mDEV0Iucwz0

1) Depth of the tree: max_depth=none overvfitting and unfitting if max_depth are less 
2) splitter: randomly or best (overfitting issues)









