# Lab-4
This is the fourth Lab for the class Introduction to Machine Learning DIT 45100 AIW01

Install the following python packages needed for this Lab. I would advice that as practice for industry, you install these packages in a virtual environment.

`pip install jupyterlab` `pip install matplotlib` `pip install keras` `pip install pandas` `pip install scikit-learn`

You will be provided with some sample code in sample_code.ipynb that will provide you information that should be enough for you to complete the labs. The following tasks below are our objectives for the lab

You will be implementing the following algorithms we discussed in class:

- Classification with neural networks (100 marks)
  - Download the cifar dataset
  - Sample and show examples from the dataset to ensure it is correct
  - Implement algorithms i.e: Using python libraries.
  - Use feature scaling. This is most easily done by dividing the images by 255, which will effectively put your images in range [0, 1]
  
  - Use tf.Keras to build a fully connected network (without regularization) 
    
    - Use sigmoid activation function for hidden layers: (25 marks)
      - Use tf.keras.layers.Flatten for the input layer 
      - Use  dense layers with sizes: [128, 64] respectively
      - Use 1 Softmax output layer with size 10
      - Use sgd to train the network
        - Use learning rate of 1
        - Train for 100 epochs (Training will take approximately 7 minutes to train so prepare accordingly)
        - Use validation_split of about 0.2
        - Plot the training accuracy against the validation accuracy
        - Get the accuracy on the testing set
        Hint: You should be able to hit accuracy above 0.40 on the training, validation and test set
        
    - Use relu activation function for hidden layers: (25 marks)
      - Use  dense layers with sizes: [128, 64] respectively
      - Use 1 Softmax output layer with size 10
      - Use sgd to train the network
        - Use learning rate of 1
        - Train for 100 epochs (Training will take approximately 7 minutes to train so prepare accordingly)
        - Use validation_split of about 0.2
        - Plot the training accuracy against the validation accuracy
        - Get the accuracy on the testing set
        Hint: You should be able to hit accuracy above 0.50 on the training, validation and test set 
   
  - Use tf.Keras to build a fully connected network (with regularization) 
    - Use sigmoid activation function for hidden layers: (25 marks)
      - Use tf.keras.layers.Flatten for the input layer
      - Use  dense layers with sizes: [128, 64] respectively
        - Use regularization on all dense layers  
        - Use glorot_uniform initialization for weights
        - Use zero initialization for biases
      - Use 1 Softmax output layer with size 10
      - Use sgd to train the network
        - Use learning rate of 1
        - Train for 100 epochs (Training will take approximately 7 minutes to train so prepare accordingly)
        - Use validation_split of about 0.2
        - You should be able to hit accuracy above 0.40 on the training, validation and test set 
      - You should be able to hit accuracy above 0.40 on the training, validation and test set 
      - Plot the training accuracy against the validation accuracy
      - Get the accuracy on the testing set
   
    - Use relu activation function for hidden layers: (25 marks)
      - Use tf.keras.layers.Flatten for the input layer
      - Use  dense layers with sizes: [128, 64] respectively
        - Use regularization on all dense layers  
        - Use he_initialization for weights
        - Use zero initialization for biases
      - Use 1 Softmax output layer with size 10
      - Use sgd to train the network
        - Use learning rate of 1
        - Train for 100 epochs (Training will take approximately 7 minutes to train so prepare accordingly)
        - Use validation_split of about 0.2
        - You should be able to hit accuracy above 0.40 on the training, validation and test set 
      - You should be able to hit accuracy above 0.40 on the training, validation and test set 
      - Plot the training accuracy against the validation accuracy
      - Get the accuracy on the testing set
 
 
   
