# GCN_NodeClassification

The Cora dataset is used in the implementation of this task.The dataset contains academic publications which are represented by nodes and the links between nodes represent
citations. If paper A cites paper B, then there is an edge from node A to B. The nodes have an attribute subject and this has seven values namely Neural Networks, probabilistic Methods, Genetic Algorithms, Theory, Case Based, Reinforcement Learning, and Rule Learning. We can say these seven values to be the classes.

There are 2708 nodes and 5429 links. We use 140 nodes for training, 500 for testing and rest for validation. This splitting of node is done by scikit-learn's train test split function. Two GCN layers with 16 layer size is used and a dropout of 50% is used in both GCN layers. To define the layers the keras library is used. The activation
function used in both layers is RelU. A cross entropy loss is defined to calculate the loss and an adam optimizer is used.
