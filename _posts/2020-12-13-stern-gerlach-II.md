---
layout: post
title: Stern-Gerlach Experiment - II
date: 2020-12-13
category: quantum-mechanics
permalink: stern-gerlach--II
---

The magnetic moment $$\boldsymbol{\mu}$$ and the the intrinsic spin angular momentum
$$\mathbf{S}$$ of a particle are related by the equation,

\begin{equation}
\boldsymbol{\mu} = \frac{gq}{2mc}\mathbf{S}
\label{eq:isam}
\end{equation}

where $$q$$ is the unit charge, $$m$$ the mass of the particle, and $$c$$ the speed
of light in vacuum. $$g$$ is a dimensionless constant whose value varies with 
the particle. For example, $$g = 2.00$$ for an electron,  $$g = 5.58$$ for a proton,
and $$g = -3.82$$ for a neutron[^1]. 

It is tempting to presume that the intrinsic spin angular momentum is 
just the orbital angular momentum of the particle spinning around its own axis.
However, *spin*,  as in this context, is a type of angular momentum that has no 
classical analogue. In fact, Eq. \eqref{eq:isam} can't be derived from classical
arguments, and it is best to think of $$g$$ as a dimensionless factor inserted
to balance the magnitudes and as well as the units.

In the Stern-Gerlach experiment, we are interested only in the 47th electron
in the silver atom. This is because, the spin magnetic moment of the entire
atom is effectively due to this single electron. If $$\mathbf{B}$$ is the
strength of the magnetic field, then the energy of interaction of the
magnetic dipole with the external magnetic field is $$- \boldsymbol{\mu}
\cdot \mathbf{B}$$. The corresponding force experienced by the *neutral*
silver atom is,

$$
\begin{aligned}
\mathbf{F} & = \mathbf{\nabla (\mu \cdot B)} \\
& = \frac{\partial}{\partial x} \mathbf{\left(\mu \cdot B \right)}\, \hat{\mathbf{i}}
+ \frac{\partial}{\partial y} \mathbf{\left(\mu \cdot B \right)}\, \hat{\mathbf{j}}
+ \frac{\partial}{\partial z} \mathbf{\left(\mu \cdot B \right)}\, \hat{\mathbf{k}}.
\end{aligned}
$$

Since the applied magnetic field is in the $$z$$ direction, we can consider
only the $$z$$ component of the force, and neglect the rest. Thus, we have,

$$
\begin{equation}
\begin{aligned}
F_{z} &=  \frac{\partial}{\partial z} \mathbf{\left(\mu \cdot B \right)} \\ \nonumber
&= \frac{\partial}{\partial z} \left(\mu_{x}B_{x} + \mu_{y}B_{y} + \mu_{z}B_{z} \right) \\ \nonumber
& \approx \mu_{z} \frac{\partial B_z}{\partial z}.
\end{aligned}
\end{equation}
\label{eq:force}
$$

If the magnetic field gradient $$ \partial B_z / \partial z$$ is 
negative, the force $$F_{z}$$ will be positive for silver atoms with negative 
$$\mu_{z}$$. Such atoms are deflected in the $$+z$$ direction.

$$\mu_{z}$$, the $$z-$$ component of the magnetic moment, can be written as
$$\mu_{z} = |\boldsymbol{\mu}| \cos\, \theta$$, where $$\theta$$ is the angle 
between the magnetic moment vector ($$\boldsymbol{\mu}$$) and the $$+z$$ axis.
Intuitively, there are infinitely many values of $$\mu_{z}$$ as $$\theta$$
can take a continuous range of values. Now, Eq. \eqref{eq:force} can be written as,

$$
\begin{equation}
F_{z} \approx \mu_{z} \frac{\partial B_z}{\partial z} =  \
|\boldsymbol{\mu}| \cos\, \theta\,  \frac{\partial B_z}{\partial z}.
\end{equation}
$$

Clearly, $$F_{z}$$ has a continuous range of values resulting in a continuous
range of deflections. That is, the trail on the screen left by the deflected 
silver atoms should be a straight line. The extreme points of this line
correspond to $$\theta = 0^{\circ}$$ and $$\theta = 180^{\circ}$$.

What Stern and Gerlach observed was completely different. On the screen were
two clusters of traces, but not a continuous line.  
This is a very important result because it tells that the $$z$$ component
of the silver atom's magnetic dipole moment has *only* two values. Since  the
magnetic dipole moment of a neutral silver atom is effectively due to an
electron, this result holds good for electron as well.

Writing only the $$z$$ component of Eq \eqref{eq:isam}, we get,

$$
\begin{equation}
\mu_{z} = \frac{gq}{2mc}S_{z}.
\end{equation}
$$

Calculations show that the two experimentally observed values of $$\mu_{z}$$ 
correspond to $$S_{z} = \pm \hbar/2$$. 

In summary, Stern-Gerlach experiment showed that the spin angular momentum
of an electron has only two values, but not a contious range of values as
predicted by the classical theory. 

This is why the Stern-Gerlach experiment is a landmark experiment in quantum 
mechanics. 

[^1]: I am yet to understand how Eq. \eqref{eq:isam} works for a neutral
    particle like neutron.

**Reference**:
1. John S Townsend. *A Modern Approach to Quantum Mechanics*