---
layout: post
title: Reading Courant's "Introduction to Calculus and Analysis, Volume I"
categories: [Notes, Book Notes]
tags: [mathematics, analysis, calculus]
math: true
media_subpath: /assets/img/posts/reading-courant-s-introduction-to-calculus-and-analysis-volume-i
---
| Title | *Introduction to Calculus and Analysis*, Volume I |
| Author | Richard Courant & Fritz John |
| Publisher | Springer |
| Published Year | 1999 |

## Preface

Calculus is composed of differential and integral concepts that involve infinite processes.

Euler wrote the first [calculus textbook](https://book.douban.com/subject/2009047/).

Courant's *Vorlesungen über Differential und Integralrechnung* (1927) was the first textbook that presented differential and integral calculus as a unified subject?

This book won't avoid intuition and applications.

> disregard for applications and intuition leads to isolation and atrophy of mathematics.

It reminds me of [Rudin's book](https://book.douban.com/subject/1652002/).

> It seems extremely important that students and instructors should be protected from smug purism.

Hardy?

## Chapter 1. Introduction

### 1.1 The Continuum of Numbers

We need to build a system based on natural numbers that can measure continuous variation.

#### a. The System of Natural Numbers and Its Extension. Counting and Measuring

We want to use our rational numbers to describe continuous quantities. After selecting a segment as a unit length, we can put every rational number on a corresponding unique point of a line to form a number axis. The question is: Can every point of the line be marked by a rational number? The answer is no. The Greeks discovered some quantities can't be measured by rational numbers; they were the so-called *incommensurable quantities*, e.g. $\sqrt{2}$.

We need to extend the rational number system to a continuum of numbers.

All mathematicians, from Fermat and Newton to Gauss and Riemann, assumed that every point on the number axis corresponds to a number (rational or irrational) and obeys the same arithmetical laws as rational numbers do. Only in the 19th century did [Dedekind](https://book.douban.com/subject/2193307/) build a satisfied real number system.

#### b. Real Numbers and Nested Intervals

We note that every irrational number on the number axis can be infinitely approximated by a sequence of closed intervals with rational numbers as endpoints, whose length tends to zero. So does the converse hold? We can make a postulate:

*For any sequence of closed intervals with rational numbers as endpoints whose length tends to zero, there always exists a point on the number axis that is contained in all these intervals.*

Although we have not yet given a definition of irrational numbers, we can use this assumption as an axiom to investigate the properties of continuum, and this axiom is very geometrically intuitive.

#### e. Inequalities

The Cauchy-Schwarz inequality:

$$
(\sum_{i=1}^{n} a_i b_i)^2 \leq (\sum_{i=1}^{n} a_i^2) (\sum_{i=1}^{n} b_i^2)
$$

Proof: For every real number $t$, we have $(a_i t + b_i)^2 \geq 0$. Thus,

$$
0 \leq \sum_{i=1}^{n} (a_i t + b_i)^2 = (\sum_{i=1}^{n} a_i^2) t^2 + 2 (\sum_{i=1}^{n} a_i b_i) t + (\sum_{i=1}^{n} b_i^2)
$$

Let $A = \sum_{i=1}^{n} a_i^2$, $B = \sum_{i=1}^{n} b_i^2$, and $C = \sum_{i=1}^{n} a_i b_i$, then we have

$$
0 \leq A t^2 + 2C t + B
$$

According to the quadratic formula, we have $4C^2 - 4AB \leq 0$. After expanding it, we get the Cauchy-Schwarz inequality. $\square$

In the special case $n = 2$, we can choose

$$
a_1 = \sqrt{x}, a_2 = \sqrt{y}, b_1 = \sqrt{y}, b_2 = \sqrt{x}
$$

where $x,y$ are positive. Then we have

$$
(2\sqrt{xy})^2 \leq (x+y)^2
$$

or

$$
\sqrt{xy} \leq \frac{x+y}{2}
$$

It states that the geometric mean $\sqrt{xy}$ never exceeds their arithmetic mean $(x+y)/2$.

![Fig 1.6](fig-1-6.jpg){: w="400" }

### 1.2 The Concept of Function
