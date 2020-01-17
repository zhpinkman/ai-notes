# AI Useful Notes

# Probablities

- in **Conditional Independence Relationships** General rule: each node is conditionally independent of its _**non-descendants**_ given its parents

# Genetic Algorithms

_useful in regression problems_

## Steps

1. Initial Population
2. fitting (defining fitness function)
3. mate selection (can be eighter a replacement policy or just taking the fittest ones)
4. crossover
5. mutation

- Mutation occurs to maintain diversity within the population and prevent premature convergence.

# Bias, Variance trade off

![simplicity vs complexity](https://miro.medium.com/max/1805/1*fkg_s9tR4ootsi9jPkFgVA.png)

In statistics and machine learning, the bias-variance tradeoff is the property of a set of predictive models whereby models with a lower bias in parameter estimation have a higher variance of the parameter estimates across samples and vice versa. The bias-variance dilemma or problem is the conflict in trying to simultaneously minimize these two sources of error that prevent supervised learning algorithms from generalizing beyond their training set:

- The bias is an error from erroneous assumptions in the learning algorithm. High bias (overly simple) can cause an algorithm to miss the relevant relations between features and target outputs (underfitting).

- The variance is an error from sensitivity to small fluctuations in the training set. High variance (overly complex) can cause an algorithm to model the random noise in the training data, rather than the intended outputs (overfitting).

# Decision Trees

## Entropy

Entropy : A decision tree is built top-down from a root node and involves partitioning the data into subsets that contain instances with similar values (homogeneous). ID3 algorithm uses entropy to calculate the homogeneity of a sample. If the sample is completely homogeneous the entropy is zero and if the sample is equally divided then it has entropy of one.

![entropy equation](https://miro.medium.com/max/446/0*sNMN2eKjMOHhNMZy.png)
![entropy equation](https://miro.medium.com/max/491/0*7ZWryjSBCxzyw7h5.png)

- More uniform = higher entropy
- More values = higher entropy
- More peaked = lower entropy

        A chi-squared test can tell us how likely it is that deviations from a             perfect split are due to chance. Each split will have a significance value, p_chance

## Two Ways of Controlling Overfitting

- Limit the hypothesis space

  - E.g. limit the max **depth of trees**
  - Easier to analyze

- Regularize the hypothesis selection
  - E.g. **chance cutoff**
  - Disprefer most of the hypotheses unless data is clear
  - Usually done in practice

# Iteration, Epoch, Batch size

- Iterations is the number of batches needed to complete one epoch.
- One Epoch is when an ENTIRE dataset is passed forward and backward through the neural network only ONCE.
- Total number of training examples present in a single batch.

# Neural Networks

- weights are being updated with **gradient descent** due due to which direction the error derivation goes.
  if it is negative the weight will increase to reach the desired weight. and if the dervation in positive the weight will decrease to reach the desired weight.

        this way we are going to the oposite direction of ERROR derivation

# Markov Decision Process

- State
- Actions
- Transition Model P(S' | S, a)
- Policy

# Logic

- Typically, ∧ is the main connective with ∃

- Typically, ⇒ is the main connective with ∀
