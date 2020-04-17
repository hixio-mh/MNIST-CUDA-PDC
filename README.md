# MNIST-CUDA-PDC
Simple implementation of a neural network that recognises hand written digits.This is implemented using Pytorch and uses NVIDIA CUDA GPU acceleration.

#### OBJECTIVES
•	To Compare the computing time between training on CPU vs training on GPUs on CUDA for recognition of handwritten digits.
•	To show that training of deep learning models is faster using GPU compared to a CPU
•	How GPU helps to accelerate to build the model for Deep Learning


#### Libraries used:
•	Pytorch
•	NumPy
#### Neural Network Architecture:
 - Input nodes :784(28*28)
 - Hidden layers :1 with 200 nodes
 - Output layer :10 nodes, each representing a number from 0 to 9
 - Activation Function: Sigmoid function
 - Error Function: MSE (Mean squared error)
 - To the minimise the loss and find the global minimum used SGD (Stochastic Gradient Descent), data divide into mini batches and trained.
 - The data is trained on CPU it takes an average time of 5 min 21 seconds to train
 - The data trained using CUDA GPU acceleration takes 4 min 23 second to train
 - Accuracy of the model trained: 0.98

#### Conclusion:
 - Training of Neural networks is faster on GPU compared to CPU
 - As the training of neural network involves mainly of vector operation, GPUs are a way better solution.

