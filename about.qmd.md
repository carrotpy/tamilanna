# Introduction to Neural Networks

*The first computational model of a neuron was proposed by Warren  McCulloch and Walter Pitts in 1943. Inspired by McCulloch and Pitts,  Rosenblatt built the first neural network, a single layer, linear binary classifier in 1957. These linear models are severely limited by the  family of functions that they can approximate. Minsky (1966) pointed out the limitations of the linear family of models, such as their inability to learn the XOR function. This revelation led to a backlash against  the neural networks approach.*

*Ivakhnenko (1971) introduced the first Multi-layer Perceptron (8  layers), which could learn nonlinear functions. The idea of using the  chain rule for training neural networks was independently discovered by  Lecun, Parker, and Rumelhart in the 1980s. Rumelhart and Hinton (1986)  presented the first successful experiments with backpropagation in their book, Parallel Distributed Processing. Neural Networks gained  ascendancy following the success of backpropagation.*

*Hochreiter (1991) addressed the vanishing and exploding gradient problems in  backpropagation. Hochreiter and Schmidhuber (1997) introduced the  Long-short Term Memory networks (LSTMs), which could remember relevant  information for a longer number of time steps. This prevented the decay  of the error signal between the layers. LeCun (1998) used LeNet-5, a  7-layered convolutional neural network for classifying handwritten  numbers. The network was trained by combining Stochastic Gradient  Descent (SGD) with backpropagation.*

*Hinton (2006) introduced the first Deep Neural Network called the Deep Belief Network trained using greedy layer-wise  pretraining\cite{Hinton}. This work is widely considered to have ushered in the modern era of Deep Learning*.

*The Deep Learning method has equipped both systems of abstract  forms of intelligence (Chess, Go) and application-oriented  systems(Speech Recognition, Computer Vision) with super-human ability.*



## What is a Neural Network?

**Artificial Neural Network** is an umbrella term that  encompasses a variety of learning systems grouped under the  Connectionism category. The neural networks can be classified into  different types based on their architecture, nature of inputs and  outputs, operating mechanisms and training algorithms, etc.  Integrate-and-fire networks map inputs to outputs through several  non-linear transformations without any regard to timing, whereas in the  Spiking neural networks, timing plays a crucial role. In most neural  network types, the architecture is fixed, only the weights of the edges  connecting the neurons are adjusted, whereas, in Neuro-evolution methods like NEAT, both the architecture and weights can be changed. Depending  on the nature of the target, variable neural networks can be classified  into two major categories such as regressors (real number output) and  classifiers (categorical output). Hopfield neural networks use the  Hebbian learning rule for training, whereas the network we are  discussing in this blog namely, Deep Neural Networks, uses the  backpropagation algorithm for training.

They all have one thing in common, a collection of simple **neuron-like units** connected to each other that cooperate to model the relationship between input  and output. The neuron is the building block of a Neural Network. There  are different models of neurons with varying closeness to the biological counterpart. The most famous model is the integrate-and-fire neuron.  They have input and output edges connecting to other neurons. An  integrate-and-fire neuron collects input from all its input edges, and  after reaching a threshold, it lights up all its output edges.



![img](https://tamilphy.files.wordpress.com/2022/05/fnn.png?w=890)

