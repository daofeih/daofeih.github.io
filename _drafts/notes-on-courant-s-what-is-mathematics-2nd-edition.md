---
layout: post
title: Notes on Courant's "What Is Mathematics?, 2nd Edition"
categories: [Notes, Book Notes]
tags: [mathematics]
math: true
media_subpath: /assets/img/posts/notes-on-courant-s-what-is-mathematics-2nd-edition/
image: cover.jpg
---
| Title | *What Is Mathematics?: An Elementary Approach to Ideas and Methods*, 2nd Edition |
| Authors | Richard Courant & Herbert Robbins |
| Publisher | Oxford University Press |
| Publish Year | 1996 |

## Preface to the Second Edition

> *What Is Mathematics?* is one of the great classics, a sparkling collection of mathematical gems, one of whose aims was to counter the idea that "mathematics is nothing but a system of conclusions drawn from definitions and postulates that must be consistent but otherwise may be created by the free will of the mathematician." In short, it wanted to put the meaning back into mathematics.

The "meaning" here means the connection between mathematics and reality. Mathematics is not just a mental game.

## Chapter I. The Natural Numbers

### &sect;2. The Infinitude of the Number System. Mathematical Induction

#### 2. The Arithmetical Progression

> *For every value of $n$, the sum $1+2+3+\cdots+n$ of the first $n$ integers is equal to $\frac{n(n+1)}{2}$.*

Proof by induction: For $n=1$, this statement is obviously true. Now suppose this statement is true for an integer $n$, then we have

$$
1+2+3+\cdots+n+(n+1)=\frac{n(n+1)}{2}+(n+1) = \frac{(n+1)(n+2)}{2}
$$

Thus, this statement is true for every integer $n$. $\square$

A hint for deriving this formula:

$$
\begin{align*}
A_n &= 1 + 2 + \cdots + n \\
A_n &= n + (n-1) + \cdots + 1 \\
\end{align*}
$$

$$
2A_n = n(n+1)
$$

#### 3. The Geometrical Progression
