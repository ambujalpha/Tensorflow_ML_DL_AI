# Tensorflow_2.1
Models of Tensorflow-Keras using latest version of tensorflow

Models-

1)TensorFlow_Minimal_Least_squares_DL-
                                      
Very basic Deep Learning model using Tensorflow. Here we are creating linear regression using tensorflow.Random dataset is used.
Steps include-
a)Import the relevant libraries
b)Data generation
c)Solving with TensorFlow
d)Extract the weights and bias
e)Extract the outputs (make predictions)
f)Plotting the data

2)MNIST_Hand-Writen_digit_recognition-

It's Deep learning model of 4 layers(including input and output layers). We are using Tensorflow. Activation function relu for hidden layers and softmax for output layer is used. One-Hot Encoding to encode the digits. 28cross28 pixel each image is there.784 input nodes and 10 output nodes(1 for each digit). 50 unit in each hidden layer. Adam(most advanced optimizer) is used.We obtain accuracy of 97%+.

3)Tensorflow_Audiobooks_DL1 and Tensorflow_Audiobooks_DL2

First part is Tensorflow_Audiobooks_DL1(Preprocessing) and second part is Tensorflow_Audiobooks_DL2(training and testing).
Files asscoiated with it-> Audiobooks_data_train.npz,Audiobooks_data_validation.npz,Audiobooks_data_test.npz.
Dataset file is Audiobooks_data.csv.
It have data set of real world buisness case. It includes customers who have bought at least once from audio book app.We are predicting how likely they are to buy again. The main target is identifying our target users for advertisment.

Dataset CSV files is attached and header column is removed.First column is ID(no use for model), second is book length of overall purchase and third is book length of purchase average.The overall price paid, average price paid.Next is Review(boolean) then we have review_on_10 means rating giving.Next we have total minutes listened, then we have completion,i.e, total minutes listened divided by total time of book.Next is support request, then we have last time person interacted minus first purchase date.This all is inputs.

Dataset represent 2 years worth of engagement here.Actually, dataset is of 2.5 years, the later part is seeing that is a person is converted or not, it's in dataset in last column as boolean.Basically we have two classify model in two classes, will buy and won't buy as 0 and 1.

We are using 4 layer model including input and output layers. Both hidden layer usses relu as activation fcution and output layer uses softmax function. We are using Adam as optimizer and sparse categorical cross entropy as loss(cost) function, it uses one-hot encoding.

Here We are using early stopping mechanism to avoid overfitting,i.e, callback function of tensorflow.We will obtain accuracy of more than 90%.
