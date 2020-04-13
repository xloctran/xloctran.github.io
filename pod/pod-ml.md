---
layout: default
---

# Machine Learning - a mathematical definition.
## Distribution

Let's say that we are interested in finding out a dependency of an outcome on a set of input variables. In machine learning, the outcome is usually called target, and the input variables are called features. How do we formulate this in mathematical terms, or statistical terms?

We formulate this using the distribution concept. Let $X$ and $Y$ are two probability spaces generated from $X$ and $Y$ and $D$ is a joint distribution over $X\times Y$. This distribution formulates the allocation of features and targets.

How to express a dependency? By a model! I mean a function $h: R^n \to R^m$ that 'maximize' the chance that f(X) equals Y. In machine learning, we need to search (using computer) through a predefined pool of functions to find one function that do this job best. This pool of functions is called a hypothesis space. Depending on the nature of the problem, we may consider different hypothesis space. Examples are linear functions, n degree polynomial functions, neural networks, etc. In summary, we search $h \in H$ such that the error
\[
P(u \neq h(x)) = D({(x, y): h(x) \neq y})
\]
is minimized.


Since we can not access to $D$, how can we chose such a function? This is where the data comes in. Let $S$ be the data set of $n$ samples that are drawn from the distribution $D$. We approximate the abstract error by the empirical error on the data set $S$:
\[
L_s(h) = \frac{|i: h(x_i)\neq y_i|}{n}
\]

This error function is called loss function. A different loss function can be chosen instead.  


In summary, given the data set $S$, the goal of machine learning is to search for a function $h_S \in H$ that minimize the associated loss function.




Let $D$ be a joint probability distribution over $X\times Y$. D represents the distribution over the whole population of features and targets. In machine learning, we want to approximate this distribution.

Let $S$ be a subset of $X\times Y$. This set corresponds to our data with each points $(x, y)\in S$ is a sample with feature $x$ and label $y$.




{% include lib/mathjax.html %}
