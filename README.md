# Lab-4
This is the fourth Lab for the class Introduction to Machine Learning DIT 45100 AIW01

Install the following python packages needed for this Lab. I would advice that as practice for industry, you install these packages in a virtual environment.

`pip install jupyterlab` `pip install matplotlib` `pip install keras` `pip install pandas` `pip install scikit-learn`

You will be provided with some sample code in sample_code.ipynb that will provide you information that should be enough for you to complete the labs. The following tasks below are our objectives for the lab

You will be implementing the following algorithms we discussed in class:

- Classification with neural networks (100 marks)
  - Download the cifar dataset
  - Sample and show examples from the dataset to ensure it is correct
  - Use feature scaling. This is most easily done by dividing the images by 255, which will effectively put your images in range [0, 1]
  
  - Use tf.Keras to build a fully connected network ***(without regularization)*** 
    
    - Testing with sigmoid: (25 marks)
      - Create model definition
        - Use tf.keras.layers.Flatten for the input layer 
        - Use  Dense layers with sizes: [128, 64] respectively for hidden layers
          - Use glorot_uniform(xavier initialization) as kernel_initializer
          - Use zero initialization for biases
          - Use sigmoid as activation function
        - Use Dense layer with softmax activation for output layer with size 10
          - Use glorot_uniform(xavier initialization) as kernel_initializer
          - Use zero initialization for biases
          - Use softmax as activation function
      - Compile model
        - Use sgd as optimizer
          - Use learning rate of 0.01
        - Use SparseCategoricalCrossentropy(log loss) as loss
        - Use accuracy as metric
      - Fit model
        - Use validation_split of about 0.2 
        - Train for 100 epochs (Training will take approximately 7 minutes to train so prepare accordingly) 
      - Plot the training accuracy against the validation accuracy
      - Get the accuracy on the testing set <br>
     - ***Hint: You should be able to hit the following accuracies:<br>
       Your last training epoch should give you around 0.55 accuracy<br>
       Your last validation epoch should give you around 0.45 accuracy<br>
       Your testing set should give you 0.45 accuracy***<br>
   
     - Testing with relu: (25 marks)
        - Create model definition
          - Use tf.keras.layers.Flatten for the input layer 
          - Use  Dense layers with sizes: [128, 64] respectively for hidden layers
            - Use he_uniform as kernel_initializer
            - Use zero initialization for biases
            - Use relu as activation function
          - Use Dense layer with softmax activation for output layer with size 10
            - Use glorot_uniform(xavier initialization) as kernel_initializer
            - Use zero initialization for biases
            - Use softmax as activation function
        - Compile model
          - Use sgd as optimizer
            - Use learning rate of 0.01
          - Use SparseCategoricalCrossentropy(log loss) as loss
          - Use accuracy as metric
        - Fit model
          - Use validation_split of about 0.2 
          - Train for 100 epochs (Training will take approximately 7 minutes to train so prepare accordingly) 
        - Plot the training accuracy against the validation accuracy
        - Get the accuracy on the testing set <br>
    - ***Hint: You should be able to hit the following accuracies:<br>
       Your last training epoch should give you around 0.74 accuracy<br>
       Your last validation epoch should give you around 0.50 accuracy<br>
       Your testing set should give you 0.50 accuracy***<br>
   
  - Use tf.Keras to build a fully connected network ***(with regularization)***
    - Testing with sigmoid: (25 marks)
      - Create model definition
        - Use tf.keras.layers.Flatten for the input layer 
        - Use  Dense layers with sizes: [128, 64] respectively for hidden layers
          - Use glorot_uniform(xavier initialization) as kernel_initializer
          - Use zero initialization for biases
          - Use sigmoid as activation function
          - Use L2 regularization with weight of 0.001
        - Use Dense layer with softmax activation for output layer with size 10
          - Use glorot_uniform(xavier initialization) as kernel_initializer
          - Use zero initialization for biases
          - Use softmax as activation function
          - Use L2 regularization with weight of 0.001
      - Compile model
        - Use sgd as optimizer
          - Use learning rate of 0.01
        - Use SparseCategoricalCrossentropy(log loss) as loss
        - Use accuracy as metric
      - Fit model
        - Use validation_split of about 0.2 
        - Train for 100 epochs (Training will take approximately 7 minutes to train so prepare accordingly) 
      - Plot the training accuracy against the validation accuracy
      - Get the accuracy on the testing set <br>
     - ***Hint: You should be able to hit the following accuracies:<br>
       Your last training epoch should give you around 0.45 accuracy<br>
       Your last validation epoch should give you around 0.43 accuracy<br>
       Your testing set should give you 0.43 accuracy***<br>
   
     - Testing with relu: (25 marks)
        - Create model definition
          - Use tf.keras.layers.Flatten for the input layer 
          - Use  Dense layers with sizes: [128, 64] respectively for hidden layers
            - Use he_uniform as kernel_initializer
            - Use zero initialization for biases
            - Use relu as activation function
            - Use L2 regularization with weight of 0.005
          - Use Dense layer with softmax activation for output layer with size 10
            - Use glorot_uniform(xavier initialization) as kernel_initializer
            - Use zero initialization for biases
            - Use softmax as activation function
            - Use L2 regularization with weight of 0.005
        - Compile model
          - Use sgd as optimizer
            - Use learning rate of 0.01
          - Use SparseCategoricalCrossentropy(log loss) as loss
          - Use accuracy as metric
        - Fit model
          - Use validation_split of about 0.2 
          - Train for 100 epochs (Training will take approximately 7 minutes to train so prepare accordingly) 
        - Plot the training accuracy against the validation accuracy
        - Get the accuracy on the testing set <br>
    - ***Hint: You should be able to hit the following accuracies:<br>
       Your last training epoch should give you around 0.50 accuracy<br>
       Your last validation epoch should give you around 0.48 accuracy<br>
       Your testing set should give you 0.48 accuracy***<br>
 
 
   
