# Challenge_13
Repo for challenge 13

This challenge asked us to build a deep learning (multi-hidden-layered) learning application to assess how likely creditors are to default on payments along with two (2) alternative models to experiment with the build of the model to gauge accuracy.

- We start by importing a CSV file & reading in the data, we then clean up some columns & encode dtypes with OneHotEncoder. 
- Next we target the 'Is Succesful' column because that gives a binary representation of the creditors standing with respect to default. 
- Then, we split 4 datasets to train & test X & y, respectively.
- Finally, we scale using StandardScaler. Now we are finished cleaning data. 

Next - build the Neural Net.
- We start by defining the number of input features as the 0 index of the X_train dataset.
- We then create two hidden layers with ReLU as the activation function for each.
- Next, create Output layer
- instantiate the Sequence model
- Add the hidden/output layers with their respective activation function via Dense.
- Finally we compile & fit the model using a binary cross entropy loss function, adam optimizer, & accuracy performance metrics.
- & lastly, save the output. 

Lastly - building alterantive models & comparing accuracy
(I will rather list the changes made to each of the respective models rather than redundantly describe the process again.)
Neural Net alt. 1 -
- Reduced the hidden layers to only a single layer while upping the nodes by 12%.
- Changed the hidden layer activation function to sigmoid.

Neural Net alt. 2 - 
- Created 3 hidden layers with 75, 50, & 25 nodes, respectively. 
- Set the activation function for the first two hidden layers to ReLU & the third to Sigmoid.
- Doubled the epochs to 100.
