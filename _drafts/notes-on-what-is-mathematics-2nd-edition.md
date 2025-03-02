---
layout: post
title: Notes on "What Is Mathematics?, 2nd Edition"
categories: [Notes, Book Notes]
tags: [mathematics]
math: true
media_subpath: /assets/img/posts/notes-on-what-is-mathematics-2nd-edition
image: cover.jpg
---
[Richard Courant](https://en.wikipedia.org/wiki/Richard_Courant) & [Herbert Robbins](https://en.wikipedia.org/wiki/Herbert_Robbins)'s *What Is Mathematics?: An Elementary Approach to Ideas and Methods* is a classic introduction to mathematical thinking, originally published in 1941 and later revised in the second edition with additional contributions from [Ian Stewart](https://en.wikipedia.org/wiki/Ian_Stewart_(mathematician)). The book aims to present mathematics as a unified and intellectually rich discipline rather than a collection of isolated techniques.

## Chapter I. The Natural Numbers

### Introduction

The natural number system is a safe ground for building up the whole mathematical palace.

### &sect;1. Calculation with Integers

#### 1. Laws of Arithmetic

Instead of proving laws of arithmetic, the authors use a concrete model—box of dots—to explain why these laws hold.

#### 2. The Representation of Integers

The positional system makes computation easier.

#### 3. Computation in Systems Other than the Decimal

The binary system has a special position: it only needs two digits 0 and 1 to represent all natural numbers. Leibniz gave these two digits a mysterious interpretation:

> Leibniz saw in his binary arithmetic the image of creation. He imagined that Unity represented God, and zero the void; that the Supreme Being drew all beings from the void, just as unity and zero express all numbers in his system of numeration.”

Is this a far-fetched imagination? Perhaps not. Perhaps the matter in the universe is created by some kind of code.

### &sect;2. The Infinitude of the Number System. Mathematical Induction

#### 2. The Arithmetical Progression

$$
A_n := \sum_{i=1}^{n} i = \frac{n(n+1)}{2}
$$

Proof by induction: When \\(n=1\\), this equality obviously holds. Suppose this equality holds for a positive integer \\(n\\), then we have

$$
A_{n+1} = A_n + (n+1) = \frac{n(n+1)}{2} + (n+1) = \frac{(n+1)(n+2)}{2}
$$

Thus, this equality holds for \\(n+1\\). This closes the induction. \\(\square\\)

Derivation:

$$
\begin{align*}
    A_n &= 1 + 2 + 3 + \cdots + n \\
    A_n &= n + (n-1) + (n-2) + \cdots + 1 \\
\end{align*}
$$

$$
\Downarrow
$$

$$
2A_n = n(n+1)
$$

#### 3. The Geometrical Progression

$$
G_n := \sum_{i=0}^{n} q^i = \frac{1-q^{n+1}}{1-q}
$$

where \\(q \neq 1\\).

Proof by induction: When \\(n=0\\), this equality obviously holds. Suppose this equality holds for a natural number \\(n\\), then we have

$$
G_{n+1} = G_n + q^{n+1} = \frac{1-q^{n+1}}{1-q} + q^{n+1} = \frac{1-q^{n+2}}{1-q}
$$

Thus, this equality holds for \\(n+1\\). This closes the induction. \\(\square\\)

Derivation:

$$
\begin{align*}
    G_n &= 1 + q + q^2 + q^3 + \cdots + q^n \\
    qG_n &= q + q^2 + q^3 + \cdots + q^n + q^{n+1} \\
\end{align*}
$$

$$
\Downarrow
$$

$$
(1-q)G_n = 1-q^{n+1}
$$

#### 4. The Sum of the First \\(n\\) Squares

$$
S_n := \sum_{i = 1}^{n} i^2 = \frac{n(n+1)(2n+1)}{6}
$$

Proof by induction: When \\(n=1\\), this equality obviously holds. Suppose this equality holds for a positive integer \\(n\\), then we have

$$
\begin{align*}
S_{n+1} = S_n + (n+1)^2 &= \frac{n(n+1)(2n+1)}{6} + (n+1)^2 \\
&= \frac{(n+1)(n(2n+1)+6(n+1))}{6} \\
&= \frac{(n+1)(2n^2 + 7n + 6)}{6} \\
&= \frac{(n+1)(n+2)(2n+3)}{6} \\
\end{align*}
$$

Thus, this equality holds for \\(n+1\\). This closes the induction. \\(\square\\)

---

Derivation:

$$
\begin{align*}
    S_n = & 1 + \\
          & 2 + 2 + \\
          & 3 + 3 + 3 + \\
          & 4 + 4 + 4 + 4 + \\
          & \cdots \\
          & n + n + n + n + \cdots + n \\
\end{align*}
$$

$$
\Downarrow
$$

$$
\begin{align*}
S_n &= A_n + (A_n - A_1) + (A_n - A_2) + (A_n - A_3) + \cdots + (A_n - A_{n-1}) \\
&= n A_n - (A_1 + A_2 + A_3 + \cdots + A_{n-1}) \\
&= (n+1) A_n - \sum_{i=1}^{n} A_i \\
\end{align*}
$$

So we need a formula of \\(\sum_{i=1}^{n} A_i\\).

$$
\begin{align*}
\sum_{i=1}^{n} A_i = & 1 + \\
                     & 1 + 2 + \\
                     & 1 + 2 + 3 + \\
                     & 1 + 2 + 3 + 4 + \\
                     & \cdots \\
                     & 1 + 2 + 3 + 4 + \cdots + n \\
\end{align*}
$$

$$
\Downarrow
$$

$$
\begin{align*}
\sum_{i=1}^{n} A_i &= n A_n - (1 \cdot 2 + 2 \cdot 3 + 3 \cdot 4 + \cdots + (n-1) \cdot n)\\
&= n A_n - 2(A_1 + A_2 + A_3 + \cdots + A_{n-1})\\
&= nA_n - 2(\sum_{i=1}^{n} A_i - A_n) \\
\end{align*}
$$

$$
\Downarrow
$$

$$
\sum_{i=1}^{n} A_i = \frac{n+2}{3}A_n
$$

Now back to \\(S_n\\), we have

$$
\begin{align*}
S_n &= (n+1) A_n - \frac{n+2}{3} A_{n} \\
    &= \frac{2n+1}{3} A_{n} \\
    &= \frac{n(n+1)(2n+1)}{6} \tag*{$\square$}
\end{align*}
$$

The sum of the first \\(n\\) cubes:

$$
C_n := \sum_{i=1}^{n} i^3 = [\frac{n(n+1)}{2}]^2
$$

Proof by induction: When \\(n=1\\), this equality obviously holds. Suppose this equality holds for a positive integer \\(n\\), then we have

$$
\begin{align*}
C_{n+1} = C_n + (n+1)^3 &= [\frac{n(n+1)}{2}]^2 + (n+1)^3 \\
    &= \frac{(n+1)^2(n^2 + 4(n+1))}{4} \\
    &= \frac{(n+1)^2(n+2)^2}{4} \\
    &= [\frac{(n+1)(n+2)}{2}]^2 \\
\end{align*}
$$

Thus, this equality holds for \\(n+1\\). This closes the induction. \\(\square\\)

Derivation:

$$
\begin{align*}
    C_n = & 1^2 + \\
          & 2^2 + 2^2 + \\
          & 3^2 + 3^2 + 3^2 + \\
          & 4^2 + 4^2 + 4^2 + 4^2 + \\
          & \cdots \\
          & n^2 + n^2 + n^2 + n^2 + \cdots + n^2 \\
\end{align*}
$$

$$
\Downarrow
$$

$$
\begin{align*}
    C_n &= S_n + (S_n - S_1) + (S_n - S_2) + (S_n - S_3) + \cdots + (S_n - S_{n-1}) \\
        &= n S_n - (S_1 + S_2 + S_3 + \cdots + S_{n-1}) \\
        &= (n+1) S_n - \sum_{i=1}^{n} S_i \\
\end{align*}
$$

Now let's find the formula of \\(\sum_{i=1}^{n} S_i\\):

$$
\begin{align*}
    \sum_{i=1}^{n} S_i = & 1^2 + \\
                         & 1^2 + 2^2 + \\
                         & 1^2 + 2^2 + 3^2 + \\
                         & \cdots \\
                         & 1^2 + 2^2 + 3^2 + \cdots + n^2 \\
\end{align*}
$$

$$
\Downarrow
$$

$$
\begin{align*}
    \sum_{i=1}^{n} S_i &= n + 2^2 (n - 1) + 3^2 (n - 2) + \cdots + n^2 (n - (n-1)) \\
                       &= n S_n - (1 \cdot 2^2 + 2 \cdot 3^2 + \cdots + (n-1) n^2) \\
\end{align*}
$$

Since

$$
\begin{align*}
S_{n-1} = \frac{(n-1)n(2n-1)}{6} &= \frac{(n-1)n^2}{3} - \frac{(n-1)n}{6} \\
    &= \frac{(n-1)n^2}{3} - \frac{A_{n-1}}{3} \\
\end{align*}
$$

$$
\Downarrow
$$

$$
(n-1)n^2 = 3S_{n-1} + A_{n-1}
$$

We have

$$
\begin{align*}
    \sum_{i=1}^{n} S_i &= n S_n - (3\sum_{i=1}^{n-1}S_i + \sum_{i=1}^{n-1}A_i) \\
                       &= (n+3) S_n - 3 \sum_{i=1}^{n} S_i - \sum_{i=1}^{n-1}A_i \\
\end{align*}
$$

$$
\Downarrow
$$

$$
\begin{align*}
    \sum_{i=1}^{n} S_i &= \frac{1}{4}((n+3)S_n - \sum_{i=1}^{n-1}A_i) \\
                       &= \frac{1}{4}((n+3)S_n - \sum_{i=1}^{n}A_i + A_n) \\
                       &= \frac{1}{4}((n+3)S_n - \frac{n+2}{3}A_n + A_n) \\
                       &= \frac{n+3}{4}S_n - \frac{n-1}{12}A_n \\
\end{align*}
$$

Thus,

$$
\begin{align*}
C_n &= (n+1) S_n - \frac{n+3}{4}S_n + \frac{n-1}{12}A_n \\
    &= \frac{3n+1}{4}S_n + \frac{n-1}{12}A_n \\
    &= \frac{3n+1}{4}\frac{n(n+1)(2n+1)}{6} + \frac{n-1}{12}\frac{n(n+1)}{2} \\
    &= \frac{n(n+1)((2n+1)(3n+1)+(n-1))}{24} \\
    &= \frac{n(n+1)(6n^2+6n)}{24} \\
    &= [\frac{n(n+1)}{2}]^2 \tag*{$\square$}
\end{align*}
$$

Let's try to derive a general formula of the sum of the first \\(n\\) \\(k\\)-powers.

$$
S_{k,n} := \sum_{i=1}^{n} i^k
$$

$$
\begin{align*}
    S_{k,n} = & 1^{k-1} + \\
              & 2^{k-1} + 2^{k-1} + \\
              & 3^{k-1} + 3^{k-1} + 3^{k-1} + \\
              & 4^{k-1} + 4^{k-1} + 4^{k-1} + 4^{k-1} + \\
              & \cdots \\
              & n^{k-1} + n^{k-1} + n^{k-1} + n^{k-1} + \cdots + n^{k-1} \\
\end{align*}
$$

$$
\Downarrow
$$

$$
S_{k,n} = n S_{k-1,n} - \sum_{i=1}^{n-1} S_{k-1,i} = (n+1)S_{k-1,n} - \sum_{i=1}^{n} S_{k-1,i}
$$

We have

$$
\begin{align*}
\sum_{i=1}^{n} S_{k-1,i} =  & 1^{k-1} + \\
                            & 1^{k-1} + 2^{k-1} + \\
                            & 1^{k-1} + 2^{k-1} + 3^{k-1} + \\
                            & 1^{k-1} + 2^{k-1} + 3^{k-1} + 4^{k-1} + \\
                            & \cdots \\
                            & 1^{k-1} + 2^{k-1} + 3^{k-1} + 4^{k-1} + \cdots + n^{k-1} \\
\end{align*}
$$

$$
\Downarrow
$$

$$
\sum_{i=1}^{n} S_{k-1,i} = n S_{k-1,n} - (2^{k-1} + 2 \cdot 3^{k-1} + 3 \cdot 4^{k-1} + \cdots + (n-1) \cdot n^{k-1})
$$

#### 5. An Important Inequality
