# END2_session1

# Neuron in a Neural Network

In an neural network, every neuron is a mathematical operation
that takes inputs and multiplies them with weights and then passes
sum through another mathematical function (activation) and the output 
is passed to another neuron

# What is the use of learning rate

Learning rate is used to define the extent of correction of 
weights after each back propagation pass. Lower learning rates 
correct the weights by small amount and higher ones correct
by very high amount. So an optimal learning rate will 
enable the process to converge to minimum point of loss
swiftly and not fast or slow

# How are weights initialized

Methods for initialization of weights
in neural networks are
1. Xavier
   - calculated as random number with a uniform
    probability distribution between the range
     -(1/sqrt(n)) and 1/sqrt(n) where n is the 
     number of inputs to the node
2. Normalized Xavier
   - calculated as random number with a uniform
    probability distribution between the range
     -(sqrt(6)/sqrt(n+m)) and (sqrt(6)/sqrt(n+m)) where n is the 
     number of inputs to the node and m is the number of outputs from
     the layer
3. He 
   - calculated as random number with a Gaussian
    probability distribution with mean 0 and standard 
     deviation of sqrt(2/n) where n is the number of inputs
     to the node
    
Xavier and Normalized Xavier are used for sigmoid and tanh
activation functions

He is used for Relu activation function

# What is "loss" in a neural network?

Loss is simply the error between the obtained output and desired output
of the network. The loss or error can be measured in terms of 
mean square error or other measures like cross entropy or any
other custom loss function

# What is the chain rule in gradient flow?

Let's say there are 3 functions
- x=f(t)
- y=g(t)
- z=h(x,y)

If we need to take a derivative of z with respect to t,
then by calculus chain rule, we can write it as below

partial derivative of 'z' w.r.t 't'
is 

sum of (
(partial derivative of 'z' w.r.t 'x')*(partial derivative of 'x' w.r.t 't') and
(partial derivative of 'z' w.r.t 'y')*(partial derivative of 'y' w.r.t 't'))



