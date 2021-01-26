---
layout: post 
title: A bit about spin states
date: 2020-12-14
category: quantum-mechanics
permalink: spin-states-I
---
The Stern-Gerlach experiment showed that the $$z$$ component of the intrinsic
spin angular momentum ($$S_{z}$$) of an electron has only two possible values: 
$$+\hbar/2$$ and $$-\hbar/2$$. Let's represent state with $$S_{z} = +\hbar/2$$ 
by |$$+z \rangle$$ and the state with $$S_{z} = -\hbar/2$$ by |$$-z \rangle$$.

|$$+z \rangle$$ is a label for a particle whose spin angular momentum in 
$$z$$ direction has a value $$+\hbar/2$$. Similarly, |$$-x \rangle$$ is a
label for a particle whose spin angular momentum in $$x$$ direction has a value
$$-\hbar/2$$. In fact, |$$+z \rangle$$ or |$$-x \rangle$$ are more than labels --
they are abstract vectors with specific mathematical properties. In quantum 
mechanics lingo, they are called *kets*. A ket is supposed to contain
"as much information about the state of the particle as we are permitted in
quantum mechanics". However, for the sake of simplicity, we assume that our
kets are concerned only with the spin states of the particle.

Let \|$$ \psi \rangle$$ be a ket representing an arbitrary spin state 
($$z$$ direction) of an electron. Our common sense tells us that the electron
can *either* be in the state |$$+z \rangle$$ *or* in the state |$$-z \rangle$$.
However, it turns out that the particle can be in a rather strange state which
is a superposition of both |$$+z \rangle$$ and |$$-z \rangle$$. 

We say that the most general state of the spin of the particle is, 

\begin{equation}
|\psi\rangle = c_{+} |+z\rangle + c_{-} |-z\rangle, 
\end{equation}

where |$$+z \rangle$$ corresponds to a state with $$S_{z} = + \hbar/2$$ and 
|$$-z \rangle$$ corresponds to a state with 
$$S_{z} = - \hbar/2$$. The constants $$c_{+}$$ and $$c_{-}$$ are complex
numbers. They themselves have no
physical significance but their *absolute values* have.

It's natural to wonder if an electron will actually be found with its spin
simultaneously in states |$$+ \rangle$$ and |$$- \rangle$$.
Actually, when we *look* for 
the spin state of the electron, we never find it in such a state. Instead, we
find it in *either*
state |$$+z \rangle$$ *or* in state |$$-z \rangle$$, but never in a combination of the two.
This is because, the act of measurement forces the electron to transition to
a single specific state from a superposition of multiple states. 

Yes, this is strange, but that's how it is!


**Reference**:
1. John S Townsend. *A Modern Approach to Quantum Mechanics*