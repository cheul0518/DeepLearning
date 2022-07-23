1. Data-preprocessing
    - Imputation must be executed after splitting train and test dataset. Or the trained model would end up with overfitting because it already learned about test datasets during training.
  
2. What if weights and bias are all zero? Will a model learn with the pre-weights and bias of 0?
    - Yes, the model will learn, regardless if preweights and bias are 0. Let's see the case that the loss function is the squared error. For update, $w \leftarrow w - \frac{\eta}{m}\sum_{i\in m}x^{(i)}(w^Tx^{(i)}+b-y^{(i)}), b \leftarrow b - \frac{\eta}{m}\sum_{i\in m}(w^Tx^{(i)}+b-y^{(i)})$. So, $w$ and $b$ won't be zero after the first update, because they are affected by other elements as well as their previous values.

3. What is the difference between A.I, machine learning, and deep learning?
    - Deep learning is a subset of machine learning, and extracts patters with a use of neural networks. Compared to machine learning, deep learning has hidden layers and activation functions making it universal classifier and approximator with non-linearity.

4. Neural network input size? input image size

5. Why do I get different results? (why not deterministic)
    - Differences in training data: you run the same algorithm on different data. e.g: shuffling
    - Learning algorithim: some algorithms are stochastic, not deterministic. However it's not truely random. The specific small decisions made by the algorithm during the learning process can vary randomly. and the algorithm learns a slightly different model.

6. What if accuracy and loss discrepancy occurs? 
    - It depends on the conxext. If the model becomes overconfident in its predictions, for example, then accuracy remains high while loss can drastically increase with a single false prediction. If a dataset's imballanced such as the dataset of apple 99%, pear 1%, then the model's likley to achieve high accuracy pretty fast while loss evaluation could comparatively slow down. For the first case, accuracy's a better estimator than loss because keeping training for loss is likely to lead overfitting because the model's already overconfident. For the second case, however, loss is a better estimator because, if we trust solely accuracy, no more training leads to underfitting.

https://machinelearningmastery.com/different-results-each-time-in-machine-learning/#:~:text=2.-,Differences%20Caused%20by%20Training%20Data,of%20the%20machine%20learning%20algorithm.
    - stochastic evaluation procedures
    - differences in platform

What is the difference between percentron and neuron?

Why actionvation functions must have non-linear property?


Coefficient of determination, Gini coefficient

Optimization: https://machinelearningmastery.com/adam-optimization-from-scratch/#:~:text=Gradient%20descent%20is%20an%20optimization%20algorithm%20that%20uses%20the%20gradient,of%20partial%20derivatives%2C%20called%20Adam.

Sparse Categorical crossentropy

curse of dimentionality

min pooling layer vs max pooling layer

Why not use even-number filter in cnn?

Upsampling?

batchnorm
