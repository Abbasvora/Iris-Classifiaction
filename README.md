# Iris Classification

## Dataset

Dataset contains three classes (Iris-setosa, Iris-versicolor, Iris-virginica). These are classified based on sepal and petal features such as length and width.

![Screenshot (258)](/assets/Screenshot%20(258).png)

We convert Species to int values for classification

![Screenshot (258)](/assets/Screenshot%20(259).png)

## Tools Used

- Pandas
- Numpy
- Matplotlib
- Seaborn
- Sikit Learn


## Algorithm

### KNeighborsClassifier

We use Euclidean distance to calculate nearest neighbour and based on smallest distance we can classify their class.

### DecisionTreeClassifier

- We start at the tree root and split the data on the feature that results in the largest information gain (IG).

- We can then repeat this splitting procedure at each child node until the leaves are pure. This means that the samples at each leaf node all belong to the same class.

- We may set a limit on the depth of the tree to prevent overfitting. We compromise on purity here somewhat as the final leaves may still have some impurity.

## Result

#### KNeighborsClassifier

Using `n_neighbour= 11` in our model we get an **accuracy of 1.0** and **f1 score of 0.93**.

![Screenshot (258)](/assets/Screenshot%20(260).png)

Confusion Matrix

![Screenshot (258)](/assets/Screenshot%20(262).png)

#### DecisionTreeClassifier

Using default values for our model we get **accuracy of 0.96** and f1 **score of 0.97**.

Confusion Matrix

![Screenshot (258)](/assets/Screenshot%20(261).png)