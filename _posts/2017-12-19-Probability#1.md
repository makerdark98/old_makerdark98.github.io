---
layout: post
title: "Probability#1"
comments: true
description: "1st"
keywords: "math, probability"
tags :
- probability
- math

---

# Chatper 1

## 1.2 Properties of Probability

* Probability is a real-valued set function P that assigns, to each event A in the sample space sS, a number P(A), called the probabbility of the event A, such that the following properties are satisfied:
    * $$P(A)>=0$$
    * $$P(S)=1$$
    * If $$A_1,A_2,A_3,...$$ are events and $$A_i \cup A_j = \emptyset, i \not = j,$$ then

    $$P(A_1 \cup A_2 \cup \cdots \cup A_k) = P(A_1) + P(A_2) + \cdots + P(A_k)$$

* Other Properties
    * $$P(A) = 1 - P(A')$$
    * $$P(\emptyset) = 0$$
    * If events A and B are such that $$A \subset B$$, then $$P(A) <= P(B)$$.
    * If A and B are any two events, then $$P(A \cup B) = P(A) + P(B) - P(A \ cap B)$$

## 1.4 Conditional Probability

* The conditional probability of an event A, given that event B has occurred, in defined by
    * $$P(A | B) = \frac{P(A \cap B)}{P(B)}$$
    * provided that $$P(B)>0$$

* The proability that two events, A and B, both occur is given by the multiplication rule
    * $$P(A \cap B) = P(A)P(B|A)$$
    * $$P(A \cap B) = P(B)P(A|B)$$

## 1.5 Independent Events

* Events A and B are independent if and only if $$P(A \cap B)=P(A)P(B)$$. Otherwise A and B are called dependent events.
* Events A, B, and C are mutually independent if and only if the following two conditions hold
    * A,B, and C are pairwise independent
    * $$P(A \cap B \cap C) = P(A)P(B)P(C)$$

