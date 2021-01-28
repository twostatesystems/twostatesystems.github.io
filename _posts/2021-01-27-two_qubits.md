---
layout: post
title: Two qubits
date: 2021-01-27
permalink: two-qubits
---
Whatever we have learnt till now is only about *one* qubit. What happens if we
have more than one qubit? It is an important question because any quantum 
processor that is worth its salt should have quite a few qubits. For example,
Google's Sycamore has $$53$$ qubits, and IBM's Hummingbird has $$65$$ qubits.
IBM is also planning to build a $$1000-$$plus qubit processor by 
[2023](https://www.ibm.com/blogs/research/2020/09/ibm-quantum-roadmap/).

Consider a system of two qubits. The qubits could be physically realised
as the left and right polarisations of a photon, or the up and down spins of a
spin-$$1/2$$ particle, or by means of any other two state quantum mechanical
system.

For simplicity, let's take a step back, and start with two classical bits,
which can be in states $$0$$ and $$1$$. Since they are classical
bits, there is no superposition state. The possible states of this two-bit
system are: $$00, 01, 10, 11$$. Therefore, the *computational basis states* of
the corresponding two-qubit system are: $$|0 \rangle |0 \rangle$$,
$$|0 \rangle |1 \rangle$$, $$|1 \rangle |0 \rangle$$, and $$|1 \rangle |1 \rangle$$.

The two-qubit system can also exist in a state that is a linear combination of
the computational basis states. Such a state can be represented by:

$$
\begin{equation}
|\psi \rangle = \alpha_{00}|0 \rangle |0 \rangle + \alpha_{01} |0 \rangle |1 \rangle 
+ \alpha_{10} |1 \rangle |0 \rangle + \alpha_{11} |1 \rangle |1 \rangle
\end{equation},
\label{eq:two-qubits}
$$

where $$\alpha_{00}, \alpha_{01}, \alpha_{10}$$, and $$\alpha_{11}$$ are complex
numbers, and are called *amplitudes*. The normalisation condition now becomes,

$$
\begin{equation}
|\alpha_{00}|^{2} + |\alpha_{01}|^{2} + |\alpha_{10}|^{2} + |\alpha_{11}|^{2} = 1
\end{equation}.
$$

From Eq. \eqref{eq:two-qubits}, it is clear that four complex numbers are
required to describe the state of a two-qubit system.

Suppose we want to examine the state of our system of two qubits. This
obviously involves measuring the state of each qubit, one after the other.
*What is the probability of finding the first qubit in state $$|0 \rangle$$*?

Since we are interested in those states in which the first qubit is in
state $$|0 \rangle$$, we can neglect the last two terms in Eq.\eqref{eq:two-qubits}.
Now, we can write,

$$
\begin{equation}
\begin{aligned}
\left(
\begin{array}{c}
\text{Probability of} \\
\text{finding the first} \\ 
\text{qubit in state } |0 \rangle
\end{array}
\right) &=
%
\left(
\begin{array}{c}
\text{Probability of} \\
\text{getting } \\ 
|0 \rangle |0 \rangle 
\end{array}
\right) +
%
\left(
\begin{array}{c}
\text{Probability of} \\
\text{getting } \\ 
|0 \rangle |1 \rangle 
\end{array}
\right) \\[10pt]
%
&= |\alpha_{00}|^{2} + |\alpha_{01}|^{2}
\end{aligned}
\end{equation}.
$$

After the measurement, the system collapses to the state:

$$
\begin{equation}
|\psi' \rangle = \frac{\alpha_{00} |0 \rangle |0 \rangle + \alpha_{01} |0 \rangle |1 \rangle} 
{\sqrt{|\alpha_{00}|^{2} + |\alpha_{01}|^{2}}}
\end{equation}.
$$

That is, the post-measurement state is *re-normalised* by the factor
$$\sqrt{|\alpha_{00}|^{2} + |\alpha_{01}|^{2}}$$.

## Bell State

Bell state (or EPR Pair) is an interesting two-particle system in quantum
mechanics. According to Nielsen and Chuang, "Bell state is responsible for
many surprises in quantum computation and quantum information". It is represented
by,

$$
\begin{equation}
|B \rangle = \frac{1}{\sqrt{2}}|0 \rangle |0 \rangle + 
\frac{1}{\sqrt{2}}|1 \rangle |1 \rangle 
\end{equation}.
$$

If we make a measurement on a two-qubit system in Bell state, then there is a
50% chance of finding both the qubits in state $$|0 \rangle$$, and 50% chance of
finding both of them in state $$|1 \rangle$$.

Here comes the interesting part. If we make a measurement, and find the first
qubit to be in state $$|0 \rangle$$, then the post measurement state would be
$$|0 \rangle |0 \rangle$$. Because of this, the measurement of the second qubit
always gives the same result as the measurement of first qubit. That is, the 
measurement outcomes are *correlated*. Similar thing happens when we find the
first qubit to be in state $$|1 \rangle$$.

**Reference:**
1. Nielsen and Chuang. *Quantum Computation and Quantum Information*