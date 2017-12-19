---
layout: post
title: "Probability#2"
comments: true
description: "2st"
keywords: "math, probability"
tags :
- probability
- math

---

# Chatper 2 Discrete Distributions

## 2.1 Random variables of the discrete type

* Given a random experiment with an outcome space S, a function X that assigns one and only one real number $$X(s)=x$$ to each element s in S is called a random variable. Thespace of X is trhe set of real numbers $$\{x: X(s) = x, s \in S \}$$, where $$s \in S$$ means that the element s belongs to the set S.

* The probability mass function(p.m.f) $$f(x)$$ of a discrete random variable X is a function that satisfies the following properties:
    * $$f(x) > 0, x \in S$$
    * $$\sum_{x \in S} f(x) = 1$$
    * $$P(X \in A) = \sum_{x\in A} f(x), \text{ where } A \subset S$$

## 2.2 Mathmatical Expectation
* If $$f(x)$$ is the p.m.f of the random variable X of the discrete type with space S, and if the summation $$\sum_{x \in S} u(x)f(x),$$ which is eomtimes written $$\sum_S u(x)f(x).$$ exists, then the sum is called the mathematical expectation or the expected value of the function $$u(X)$$, and it is denoted by $$E[u(X)]$$. That is
    $$E[u(X)] = \sum_{x \in S} u(x)f(x)$$

## 2.3 The mean, variance, and standard deviation
* $$\mu = \sum_{x \in S} xf(x) = E(X)$$
* $$\sigma ^2 = Var(X) = \sum_{x \in S} (x-\mu)^2f(x)$$

## 2.5 The Moment-Generating function
* Let X be a random variable of the discrete type with p.m.f $$f(x)$$ and space S. If there is a positive number $$h$$ such that
    * $$E(e^{tX})=\sum_{x \in S} e^{tx}f(x)$$
* exists and is finite for $$-h < t < h$$, then the function of t defined by
    * $$M(t) = E(e^{tX})$$
* is alled the moment-generating function of X (or of the distribution of X). This function is often abbreviated as m.g.f

* $$M'(0) = E[X] = \mu$$
* $$M''(0) - [M'(0)]^2= E(X^2) - [E(X)]^2 = \sigma ^2$$

## Discrete Distiributions

### Bernoulli $$(0 < p < 1)$$
* $$f(x) = p^x(1-p)^{1-x}\text{   }x=0,1$$
* $$M(t) = 1-p + pe^t$$
* $$\mu = p$$
* $$\sigma ^2 = p(1-p)$$

### Binomial $$b(n,p),0<p<1$$
* $$f(x)=\frac{n!}{x!(n-x)!}p^x(1-p)^{n-x},\text{   }x=0,1,2,...,n$$
* $$M(t) = (1-p+pe^t)^n$$
* $$\mu = np$$
* $$\sigma ^2 = np(1-p)$$

### Geometric $$0<p<1$$
* $$f(x) = (1-p)^{x-1}p, x=1,2,3,...$$
* $$M(t)=\frac{ pe^t }{ 1-(1-p) e^t }, t < -ln(1-p)$$
* $$\mu = \frac{1}{p}$$
* $$\sigma ^2 = \frac{1-p}{p^2}$$

### Hypergeometric $$N_1>0, N_2>0, N=N_1+N_2$$
* $$f(x)=\frac{ \binom{N_1}{x} \binom{N_2}{n-x} }{ \binom{N}{n} }, x<=n, x<=N_1, n-x<=N_2$$
* $$\mu = n(\frac{N_1}{N})$$
* $$\sigma ^2 = n(\frac{N_1}{N})(\frac{N_2}{N})(\frac{N-n}{N-1})$$

### Negative Binomial $$0<p<1, r=1,2,3,...$$
* $$f(x) = \binom{x-1}{r-1}p^r(1-p)^{x-r}, x=r,r+1,r+2,...$$
* $$M(t) = \frac{ (pe^t)^r }{ [1-(1-p) e^t] ^r }, t < -ln(1-p)$$
* $$\mu = r(\frac{1}{p})$$
* $$\sigma ^2 = \frac{r(1-p)}{p^2}$$

### Poisson $$0<\lambda$$
* $$f(x)=\frac{\lambda^x e^{-\lambda}}{x!}, x=0,1,2,...$$
* $$M(t)=e^\lambda(e^t-1)$$
* $$\mu=\lambda$$
* $$\sigma^2 = \lambda$$

### Uniform $$m>0$$
* $$f(x)=\frac{1}{m}, x=1,2,...,m$$
* $$\mu = \frac{m+1}{2}$$
* $$\sigma ^2 - \frac{m^2-1}{12}$$
