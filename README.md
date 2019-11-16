# Decision Tree - Online Advertisement Prediction

The project includes implementation of Decision tree classifier without using any libraries. The Objective of this project is to make prediction and train the model over a dataset (Iris data Set, Advertisement dataset), the dataset was split randomly between training and testing set in the ratio of 8:2 respectively. After constructing the decision tree with the training data and applying the appropriate pruning strategy following details are observed in two independent runs,

## Iris Data Set

* 1st Run, (test set_1 for a training set_1)
    * Accuracy before pruning: 83.0%
    * Accuracy after pruning: 90.0%
	* Total Accuracy Increase: 7%

* 2nd Run, (test set_2 for a training set_2)
	* Accuracy before pruning on 93.0%
	* Accuracy after pruning on the same set: 100.0%
	* Total Accuracy Increase: 7%

## Advertisement dataset (super data science)

* 1st Run, (test set_1 for a training set_1)
	* Accuracy before pruning: 88.0%
	* Accuracy after pruning: 90.0%
	* Total Accuracy Increase: 2%

* 2nd Run, (test set_2 for a training set_2)
	* Accuracy before pruning on 86.0%
	* Accuracy after pruning on the same set: 91.0%
	* Total Accuracy Increase: 5%

## Pruning Strategy
To prune each node one by one (except the root and the leaf nodes), and check weather pruning helps in increasing the accuracy, if the accuracy is increased, prune the node which gives the maximum accuracy at the end to construct the final tree. (If the accuracy of 100% is achieved by pruning a node, stop the algorithm right there and do not check for further new nodes).


## How to configure
1) If the system don't have python Installed in it, first install any python version (version greater than v2.7).
	- https://www.python.org/downloads/
2) The code has the following dependencies, which need to be installed before running this code:
        - Pandas. More details at: https://pandas.pydata.org
	- from command line: pip install pandas
	- Scikit Learn for only one method in the driver code - train test split 
	- from command line: pip install -U scikit-learn
3) Open root directory (DecisionTree) of the project and run command
	- from command line: python driver.py
