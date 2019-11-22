In this section you will learn about tensors and how they are the building blocks of neural networks in Pytorch. In this video we will review: Tensors in 1-Dimension and 2- Dimensions Derivatives, The Dataset Class In the simplest of terms, a neural network is a mathematical function. It takes in one or multiple inputs, processes it and produces one or more outputs. The following image is used to represent a neural network. In Pytorch, neural networks are composed of Pytorch tensors. A Pytorch tensor is a data structure that is a generalization for numbers and dimensional arrays in Python. For the neural network, the input x is be a tensor, the output y will be a tensor, the network will be comprised of a set of parameters which are also tensors. For producing one or more outputs the neural network will need to process its input. For processing the neural network will apply a series of tensor operations on the input it receives. Many of these tensor operations are generalizations of familiar mathematical operations like multiplication and addition. In this course we will focus on tensor operations that are essentially vector and matrix operations For the rest of this course, you will convert your data into pytorch tensors and will then use that as input into a neural networks For example if we want to use a database as an input for a neural network, we could do so in the following manner. In this example each row of the database can be treated as a Pytorch tensor and we input each of these tensors into a neural network. Thus we see that a tensor is simply just a vector or a rectangular array consisting of numbers. Let’s take a look at another example, in which we convert images to rectangular tensors. Nn this example, we convert each image to Pytorch tensors for using the images as inputs to the neural network. Images in Python are usually represented as 2D arrays and 3D arrays. Thus in this case, each tensor of the input is simply a matrix or rectangular array We also see that the neural network takes the input image which was transformed to a pytorch tensors and classifies it as zero Further, it’s extremely easy to convert pytorch tensors to numpy arrays and vice-versa. Further, it’s extremely easy to convert pytorch tensors to numpy arrays and vice-versa This gives pytorch the ability to work within the python ecosystem. We can also easily integrate Pytorch with "GPU" this is an important factor for training neural networks. Parameters in neural networks are a kind of tensor that allow you to calculate gradients or derivatives. Gradients and derivatives will allow you to train the neural network We will use parameters for our neural networks in Pytorch by setting the value of the requires grad parameter equal to True We will also review the dataset class, as using this class makes it much easier to work with large data sets in pytorch