---
layout: post
title: Notes on "The Feynman Lectures on Physics, Volume I"
categories: [Notes, Book Notes]
tags: [physics]
media_subpath: /assets/img/posts/notes-on-the-feynman-lectures-on-physics-volume-i
image: cover.jpg
math: true
---
| Title | [*The Feynman Lectures on Physics*](https://www.feynmanlectures.caltech.edu/), Volume I |
| Author | Richard Feynman |

## Chapter 4. Conservation of Energy

### 4–1 What is energy?

> The law is called the *conservation of energy*. It states that there is a certain quantity, which we call energy, that does not change in the manifold changes which nature undergoes.

> It is important to realize that in physics today, we have no knowledge of what energy is. ... It is an abstract thing in that it does not tell us the mechanism or the *reasons* for the various formulas.

We cannot obtain the concept of energy and the law of conservation of energy from direct contact with physical phenomena; we first obtain concepts such as acceleration, force, temperature, etc., describe the laws of physical processes, and then summarize the law of conservation of energy from these laws. It is a law that is more abstract than the general laws of physics and may explain the deeper secrets of the universe.

### 4–2 Gravitational potential energy

> I wish to discuss the formula for gravitational energy near the surface of the Earth, and I wish to derive this formula in a way which has nothing to do with history but is simply a line of reasoning invented for this particular lecture to give you an illustration of the remarkable fact that a great deal about nature can be extracted from a few facts and close reasoning. It is an illustration of the kind of work theoretical physicists become involved in. It is patterned after a most excellent argument by Mr. Carnot on the efficiency of steam engines.

Definition: A weight-lifting machine is a machine that lifts a weight by lowering another.

Definition: If a weight-lifting machine has lifted and lowered many weights and been restored to its original condition, the net result is that it has lifted a weight, then we call this machine a perpetual-motion weight-lifting machine.

Hypothesis: There is no perpetual-motion machine. (This hypothesis is summarized from a lot of experiences.)

Definition: If a weight-lifting machine lifts a weight \\(W\\) a height \\(X\\) by lowering a weight \\(W'\\) distance \\(Y\\) and also it can lifts \\(W'\\) a height \\(Y\\) by lowering \\(W\\) a distance \\(X\\), we call this machine reversible.

Now let's talk about the efficiency of weight-lifting machines. Suppose \\(A\\) is a reversible weight-lifting machine, which lifts a weight \\(W\\) a distance \\(X\\) by lowering a unit weight a unit distance; \\(B\\) is a weight-lifting machine (not necessarily reversible), which lifts a weight \\(W\\) a distance \\(Y\\) by lowering a unit weight a unit distance. We will prove \\(X \geq Y\\); in other words, reversible machines are the most efficient. Suppose \\(Y > X\\). We run the machine \\(B\\) forward, then we could lower the weight \\(W\\) from \\(Y\\) to \\(X\\) to run another machine. Next, we run the machine \\(A\\) backward to restore the system to the original condition. The net result is to have lifted \\(W\\) a distance \\(Y - X\\). This is contradictory to our hypothesis that there is no perpetual-motion machine. Thus, \\(X \geq Y\\).

For deriving the exact efficiency of a reversible machine, Feynman designed a reversible machine:

![Fig 4-2](fig-4-2.jpg)

The conclusion is that the gravitational potential energy, i.e. weight times height, is conservative in a reversible weight-lifting machine.

Next, Feynman introduced some applications of the principle of the conservation of energy.

![Fig 4-3](fig-4-3.jpg){: w="300" }

How heavy must be \\(W\\) to balance the one pound on the plane?

When this system is balanced, it is a reversible machine. We could put the one pound weight at the top of the plane; The gravitational potential energy of this state will be equal to the gravitational potential energy of the initial state.

$$
3W = (3-5)W + 3 \times 1 \Rightarrow W = \frac{3}{5}
$$

![Fig 4-6](fig-4-6.jpg){: w="300" }

How big would the weight \\(W\\) have to be for it to balance?

When this system is balanced, it is a reversible machine. We imagine the weight \\(W\\) falls at a unit distance, then the weight on the middle would be lifted at \\(1/2\\) unit distance, and the weight on the rightmost would be lifted at \\(1/4\\) unit distance. We can't do this in reality, but we can imagine it happens. This approach is called the *principle of virtual work*. Now apply the principle of conservation of energy:

$$
0 = -1 W + \frac{1}{2} \times 60 + \frac{1}{4} 100 \Rightarrow W = 55
$$

### 4–3 Kinetic energy
