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

- The bias is an error from erroneous assumptions in the learning algorithm. High bias (overly simple) can cause an algorithm to miss the relevant relations between features and target outputs (underfitting).

- The variance is an error from sensitivity to small fluctuations in the training set. High variance (overly complex) can cause an algorithm to model the random noise in the training data, rather than the intended outputs (overfitting).

# Decision Trees

## Entropy

Entropy : A decision tree is built top-down from a root node and involves partitioning the data into subsets that contain instances with similar values (homogeneous). ID3 algorithm uses entropy to calculate the homogeneity of a sample. If the sample is completely homogeneous the entropy is zero and if the sample is equally divided then it has entropy of one.

![entropy equation](https://miro.medium.com/max/391/1*nNY_7_aWRwp8E2DyGduEPg.png)

entropy equation

- More uniform = higher entropy
- More values = higher entropy
- More peaked = lower entropy
