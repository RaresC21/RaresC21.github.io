---
title: '$\min_{x \in P} f(x)$'
date: 2025-02-15
permalink: /posts/optimization/intro/
tags:
  - optimization
---

How does optimization shape the world? The majority of decision-making is based off of optimization, from opening google maps to go to our favorite restaurants, to allocating inventory across vast warehouse networks, to regulating energy markets, to training neural networks. Optimization gets it all done. Informally, problems have three aspects: decision variables, constraints, and an objective. Our goal is to find the decision that satisfies the given constraints and which minimizes (or maximizes) the objective function. This in short defines the title of this post:

$\min_{x \in P} f(x)$.

We have decisions $x$ which must belong to a set of constraints $P$ and we wish to minimize the objective function $f(x)$.

## Examples

Such a simple framework can model a vast array of problems. We'll take a few examples here to get a taste for it.


### Inventory fulfilment

### Traveling Salesman


## Algorithms

Gradient descent is the backbone of optimization methods. But specialized algorithms exist for a variety of convex problems, especially when faced with constraints. For now, we will briefly discuss gradient descent for the unconstrained case. The idea is to create a sequence of decisions which converges to the optimal solution. Intuitively, at each step, we move the decision greedily in the direction that produces the steepest improvement in the objective function. Mathematically, this is equivalent to moving the direction of the gradient of $f(x)$. Overall, gradient descent is given by

initialize $x_0$ 

update: $x_{t+1} = x_{t} - \eta \cdot \nabla f(x)$

where $\eta$ is a parameter deciding the step sizes we should take. To illustrate, consider the following toy example. 
