1. Data-preprocessing
    - Imputation must be executed after splitting train and test dataset. Or the trained model would end up with overfitting because it already learned about test datasets during training.
  
2. What if weights and bias are all zero? Will a model learn with the pre-weights and bias of 0?
    - Yes, the model will learn, regardless if preweights and bias are 0. Let's see the case that the loss function is the squared error. For update, $w \leftarrow w - \frac{\eta}{m}\sum_{i\in m}x^{(i)}(w^Tx^{(i)}+b-y^{(i)}), b \leftarrow b - \frac{\eta}{m}\sum_{i\in m}(w^Tx^{(i)}+b-y^{(i)})$. So, $w$ and $b$ won't be zero after the first update, because they are affected by other elements as well as their previous values.

3. What is the difference between A.I, machine learning, and deep learning?
    - Depth (more than 2 hidden layers in general) and activation functions (making the learning process non-linear)

4. Neural network input size? input image size


What is the difference between percentron and neuron?

Why actionvation functions must have non-linear property?


Coefficient of determination, Gini coefficient

Optimization: https://machinelearningmastery.com/adam-optimization-from-scratch/#:~:text=Gradient%20descent%20is%20an%20optimization%20algorithm%20that%20uses%20the%20gradient,of%20partial%20derivatives%2C%20called%20Adam.
