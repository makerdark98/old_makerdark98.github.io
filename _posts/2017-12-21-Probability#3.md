---
layout: post
title: "Probability#3"
comments: true
description: "3st"
keywords: "math, probability"
tags :
- probability
- math

---

# Chapter 3 Continuous Distributions

## 3.3 Random Variables of the Continuous Type

* $$f(x)$$ should be a nonnegative function such that the total area between its graph and th x-axis equals 1. Moreover, the probability $$P(a < X < b)$$ is the area bounded by the graph of $$f(x)$$, the x-axis, and the lines $$x=a$$ and $$x=b$$. Thus, we say that the probability density function(p.d.f) of a random variable X of the continuous type, with space S that is an interval or union of intervals, is an integrable function $$f(x)$$ satisfying the following conditions:
    * $$f(x) > 0, & x \in S$$
    * $$\int_S f(x) dx = 1$$
    * If $$(a,b) \subset S$$, then the probability of the event $$\{a<X <b \}$$ is
        * $$P(a < X < b) = \int_a^b f(x) dx$$

* $$F(x) = P(X \ge x) = \int_{-\infty}^x f(t) dt, & -\infty < x < \infty$$
    * $$F(x)$$ accumulates (or, more simply, cumulates) all of the probability less than or equal to x. (This function sometimes called a cumulative distribution function or c.d.f)
    * $$F'(x)=f(x)$$

* $$\mu = E(X) = \int_{-\infty}^\infty x f(x) dx$$
* $$\sigma ^2 = Var(X) = E[(X - \mu)^2] = \int_{-\infty}^\infty (x-\mu)^2 f(x) dx$$
* $$M(t) = \int_{-infty}^\infty e^{tx} f(x) dx, & -h < t < h$$

