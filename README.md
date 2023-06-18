# Activation-functions


Activation functions are mathematical functions applied to the output of a neuron in an artificial neural network (ANN). They introduce non-linearity into the network, allowing it to learn and model complex relationships between the input and output.

The choice of activation function is a crucial decision in designing a neural network, as it affects the network's ability to learn, converge during training, and generalize to unseen data. Here are some commonly used activation functions:

1. Sigmoid (Logistic) Function:
   - Formula: f(x) = 1 / (1 + exp(-x))
   - Range: (0, 1)
   - The sigmoid function is smooth, bounded, and maps any real number to a value between 0 and 1. It is commonly used in the output layer of binary classification problems or when a probability-like output is desired.

2. Hyperbolic Tangent (Tanh) Function:
   - Formula: f(x) = (exp(x) - exp(-x)) / (exp(x) + exp(-x))
   - Range: (-1, 1)
   - The tanh function is similar to the sigmoid function but maps any real number to a value between -1 and 1. It is commonly used in hidden layers of neural networks.

3. Rectified Linear Unit (ReLU):
   - Formula: f(x) = max(0, x)
   - Range: [0, ∞)
   - ReLU is a simple and widely used activation function that replaces negative values with zero and keeps positive values unchanged. It helps overcome the vanishing gradient problem and accelerates convergence. ReLU is commonly used in hidden layers.

4. Leaky ReLU:
   - Formula: f(x) = max(αx, x) (where α is a small positive constant)
   - Range: (-∞, ∞)
   - Leaky ReLU is similar to ReLU but allows small negative values to prevent complete "dying" of neurons. It helps address the issue of dead neurons that never activate and can be used in hidden layers.

5. Softmax:
   - Formula: f(x_i) = exp(x_i) / (∑ exp(x_j))
   - Range: (0, 1) for each element, and the sum of all elements is 1
   - Softmax is used in the output layer for multi-class classification problems. It converts a vector of real values into a probability distribution over multiple classes.

These are just a few examples of activation functions, and there are many others available, each with its own characteristics and use cases. Choosing the appropriate activation function depends on the problem at hand, the network architecture, and the desired behavior of the network.
