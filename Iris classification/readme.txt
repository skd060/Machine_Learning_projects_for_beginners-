The Iris classification folder contains code in notebook with 98% accuracy. My model contains input layers with 4 node 
and 1 hidden layers with 20 nodes and output layers with 3 nodes. The details of model are following: 
                    Layer (type)                 Output Shape              Param #   
                    =================================================================
                    dense_189 (Dense)            (None, 20)                100       
                    _________________________________________________________________
                    dense_190 (Dense)            (None, 3)                 63        
                    =================================================================
                    Total params: 163
                    Trainable params: 163
                    Non-trainable params: 0
      
The IRIS dataset contains 5 Attribute:
    Attribute Information:
     1. sepal length in cm
     2. sepal width in cm
     3. petal length in cm
     4. petal width in cm
     5. class: 
        -- Iris Setosa
        -- Iris Versicolour
        -- Iris Virginica

First 4 (1-4) is our input parameters(says x1,x2,x3,x4) for our NN model and the last one (5th) is our output with 3 class. The output 
contains in strings and so it need to be convert in numerical values first. So i use one hot encoding for this purpose. And also this
dataset sorted in class name order. So it first need shuffling. And then split data set in 100 - 50 for your training and testing data set
respectivaly. 
And at last i evaluate my model with testing dataset and it gives 98% acc.

Link for IRIS dataset: http://archive.ics.uci.edu/ml/machine-learning-databases/iris/
