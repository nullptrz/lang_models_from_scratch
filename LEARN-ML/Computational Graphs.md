A node is a {tensor, matrix, vector, scalar} value

## What is a tensor?
Tensors are a generalization of vectors and matrices. Computationally, we can think of tensors as a data container for storing multi-dimensional arrays.


There are different types of tensors, each with a different rank.

- A rank zero tensor is a scalar, which is simply a number.
- A rank one tensor is a vector, which is a list of numbers.
- A rank two tensor is a matrix, which is a list of lists of numbers.
- A rank three tensor can be thought of as a vector of matrices

![[Pasted image 20240830231137.png]]

So essentially in a computational graph, there is a forward pass and a backward propagation. 
In the forward pass, which also happens in inference, the input data flows through the network which undergoes a series of operations (addition, multiplication and activation functions) to produce an output. 

We start at the loss/output basically, we try to reduce how wrong the model was from the actual ground truth. We can do so by calculating the gradient starting from the output and then going backwards through the graph to figure out how each of those neurons affect the output and we try to move in the direction which reduces that loss. Thereby the model learns and improves by repeating these steps. 







# References
[Computational Graphs](https://maucher.pages.mi.hdm-stuttgart.de/artificial-intelligence/00_Computational_Graphs.html)
[Computational Graph Engine](https://alexminnaar.com/2018/07/14/simple-computational-graph-engine.html)

