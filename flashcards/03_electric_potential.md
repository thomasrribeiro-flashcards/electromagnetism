+++
order = 3
subject = "Physics"
tags = ["electromagnetism", "potential", "poisson", "laplace", "energy"]
+++

# Electromagnetism — The Electric Potential

## 3.1 Why a Potential Exists

Q: Why does the electrostatic field admit a scalar potential, while a general vector field does not?
A: Because the electrostatic field is curl-free: $\nabla\times\mathbf{E} = 0$. A curl-free field on a simply connected domain can always be written as the gradient of a scalar. The proof comes from Coulomb's law: each point charge produces a radial field, and radial fields are gradients of spherically symmetric scalars, so by superposition the total field is also a gradient.

C: The electrostatic field is [curl-free], $\nabla\times\mathbf{E} = 0$, which guarantees the existence of a scalar function $V$ such that $\mathbf{E} = -\nabla V$.

Q: Why does the line integral of $\mathbf{E}$ between two points depend only on the endpoints, not on the path?
A: Because $\mathbf{E}$ is curl-free, Stokes's theorem gives $\oint \mathbf{E}\cdot d\mathbf{l} = 0$ for any closed loop. Splitting the loop into two paths with the same endpoints shows that both paths give the same integral. Path-independence is the hallmark of a conservative field.

## 3.2 Defining the Potential

C: The electric potential is defined by $V(\mathbf{r}) = -\int_{\mathbf{r}_0}^{\mathbf{r}} \mathbf{E}\cdot d\mathbf{l}$, where $\mathbf{r}_0$ is a [reference point] at which $V$ is set to zero.

Q: Why does the choice of reference point introduce an arbitrary additive constant in $V$ without any physical consequence?
A: Only potential DIFFERENCES $V(\mathbf{r}_2) - V(\mathbf{r}_1)$ are measurable — they correspond to the work needed to move a unit test charge between the two points. An overall additive constant cancels in every such difference, so the choice of reference is a convention, not physics.

C: For isolated charge distributions, the reference is typically chosen at [infinity], where $V \to 0$.

Q: What is the relation between the electric field and the potential?
A: $\mathbf{E} = -\nabla V$. The electric field is the negative gradient of the potential, pointing in the direction of steepest DECREASE of $V$. Equipotential surfaces are everywhere perpendicular to field lines.

C: Electric field from potential: $\mathbf{E} = [-\nabla V]$; equipotential surfaces are [perpendicular] to field lines at every point.

## 3.3 Potential of a Point Charge

Q: What is the electric potential produced by a point charge $q$ at distance $r$, with the reference at infinity?
A: $V(r) = \frac{1}{4\pi\varepsilon_0}\frac{q}{r}$. Integrating $E_r = q/(4\pi\varepsilon_0 r^2)$ inward from infinity gives the $1/r$ potential directly. Positive $q$ gives positive $V$ (a "hill"); negative $q$ gives negative $V$ (a "well").

C: Potential of a point charge: $V(r) = [\frac{q}{4\pi\varepsilon_0 r}]$, with reference at infinity.

## 3.4 Superposition of Potentials

Q: How does superposition work for potentials, and why is it simpler than superposition of fields?
A: For $N$ point charges, $V(\mathbf{r}) = \frac{1}{4\pi\varepsilon_0}\sum_i q_i/|\mathbf{r} - \mathbf{r}_i|$. The sum is SCALAR — no vector decomposition needed. This is why computing $V$ first and then taking $\mathbf{E} = -\nabla V$ is often easier than computing $\mathbf{E}$ directly from Coulomb's law.

C: For a continuous distribution, the potential is $V(\mathbf{r}) = \frac{1}{4\pi\varepsilon_0}\int\frac{\rho(\mathbf{r}')}{|\mathbf{r} - \mathbf{r}'|}\,d^3r'$, with the integrand a [scalar quantity] rather than a vector.

## 3.5 Poisson's and Laplace's Equations

Q: Why does combining $\mathbf{E} = -\nabla V$ with Gauss's law give Poisson's equation $\nabla^2 V = -\rho/\varepsilon_0$?
A: Take the divergence of $\mathbf{E} = -\nabla V$ to get $\nabla\cdot\mathbf{E} = -\nabla^2 V$, and equate this with $\rho/\varepsilon_0$ from Gauss's law. The result $\nabla^2 V = -\rho/\varepsilon_0$ turns the first-order vector equation for $\mathbf{E}$ into a second-order scalar equation for $V$, which is often easier to solve with boundary conditions.

C: Poisson's equation: $\nabla^2 V = [-\rho/\varepsilon_0]$, a second-order partial differential equation for the scalar potential.

C: In a region with no free charge, Poisson's equation reduces to [Laplace's equation]: $\nabla^2 V = 0$.

Q: Why is solving Laplace's equation with boundary conditions a central task in electrostatics?
A: In many practical situations, the charges reside on conductor surfaces and the "interesting region" is empty. All that matters is the boundary shape and the potentials (or charges) specified on the boundaries. The shape of $V$ inside is then fixed by Laplace's equation and these boundary conditions.

## 3.6 Properties of Harmonic Functions

Q: Why does Laplace's equation imply that $V$ has no local maxima or minima in a charge-free region?
A: A harmonic function (one satisfying $\nabla^2 V = 0$) equals the average of its surrounding values on any sphere. If $V$ had an interior maximum, it would be larger than its neighborhood average — impossible for a harmonic function. Maxima and minima of $V$ must therefore lie on the boundary, not in the interior.

C: In a charge-free region, $V$ is [harmonic] and its extrema can only occur on the [boundary], a result known as Earnshaw's theorem.

Q: Why does Earnshaw's theorem imply that stable electrostatic equilibrium is impossible with stationary charges alone?
A: A test charge in stable equilibrium would need $V$ to have a local minimum in free space. But harmonic functions forbid local minima. So no arrangement of static charges can trap another charge in a stable equilibrium — some additional mechanism (time variation, magnetic fields, quantum effects) is required.

## 3.7 Uniqueness Theorem

Q: What does the uniqueness theorem of electrostatics guarantee?
A: If $V$ is specified on the boundary of a region, and the charge density is specified inside, then the solution to Poisson's equation inside that region is UNIQUE. Any two candidate solutions must differ by a function that vanishes on the boundary and satisfies Laplace's equation — and the only such function is zero. So if you can guess a valid solution, it IS the solution.

C: The uniqueness theorem guarantees that Poisson's equation with specified [boundary values] for $V$ has a [unique solution] in the interior.

Q: Why is the uniqueness theorem the theoretical justification for the method of images?
A: The method of images replaces a complicated boundary-value problem with a simpler free-space problem involving fictitious "image" charges that reproduce the required boundary values. Since the new problem agrees with the original on the boundary and satisfies Poisson's equation in the same region, uniqueness guarantees it gives the same potential inside.

## 3.8 Energy of a Charge Distribution

Q: What is the total electrostatic energy of a system of $N$ point charges?
A: $U = \frac{1}{2}\sum_{i\ne j}\frac{q_iq_j}{4\pi\varepsilon_0|\mathbf{r}_i - \mathbf{r}_j|}$. It is the work needed to assemble the system by bringing the charges from infinity one at a time. The factor $\frac{1}{2}$ corrects for double counting each pair.

C: Energy of a discrete charge distribution: $U = [\tfrac{1}{2}\sum_i q_i V(\mathbf{r}_i)]$, where $V(\mathbf{r}_i)$ is the potential at charge $i$ due to all OTHER charges.

Q: For a continuous charge distribution, why is the total energy $U = \frac{1}{2}\int \rho V\,d^3r$?
A: Generalizing the discrete sum: each volume element $\rho\,d^3r$ "sees" the potential $V$ produced by the rest of the distribution. The $\frac{1}{2}$ again avoids double counting. The integral is over the regions where $\rho$ is nonzero.

## 3.9 Energy Density of the Electric Field

Q: Why can the total electrostatic energy be rewritten as an integral over the field itself: $U = \frac{\varepsilon_0}{2}\int E^2\,d^3r$?
A: Start from $U = \frac{1}{2}\int\rho V\,d^3r$, use Gauss's law to write $\rho = \varepsilon_0\nabla\cdot\mathbf{E}$, integrate by parts, and use $\mathbf{E} = -\nabla V$. The boundary term vanishes for well-behaved charge distributions, leaving $U = \frac{\varepsilon_0}{2}\int|\mathbf{E}|^2\,d^3r$. The energy is distributed throughout space wherever the field is nonzero.

C: The electrostatic energy density is $u = [\tfrac{\varepsilon_0}{2}E^2]$, so the field itself carries energy everywhere it exists.

Q: Why is the "energy in the field" picture philosophically important, even though numerically it equals the "energy in the charges" picture for electrostatics?
A: Because when we move to time-dependent electromagnetism and radiation, the field picture generalizes while the charge-based picture does not. A plane wave propagating through empty space carries energy — attributed to the field, with no "charges" in sight. The electrostatic identity is a clue that the field is the true repository of energy.

## 3.10 Capacitor Energy from the Field — P:/S:

P: A parallel-plate capacitor has plates of area $A$ separated by distance $d$ (with $d \ll \sqrt{A}$ so edge effects are negligible). The plates carry charges $+Q$ and $-Q$. Compute the total energy stored in the capacitor two ways: (a) by integrating the energy density of the electric field between the plates, and (b) via the standard formula $U = Q^2/(2C)$. Show the results agree.

S:
**IDENTIFY**: Energy-density calculation for a parallel-plate geometry. Two independent routes must give the same answer.

**PLAN**:
- Use Gauss's law (or the surface-charge boundary condition) to write $E$ between the plates in terms of $\sigma = Q/A$.
- Integrate the energy density $u = \frac{\varepsilon_0}{2}E^2$ over the volume between the plates.
- Compute the capacitance $C = \varepsilon_0 A/d$ independently and evaluate $Q^2/(2C)$.
- Compare.

**EXECUTE**:
1. Surface charge density: $\sigma = Q/A$.
2. Field between the plates (two oppositely charged planes): $E = \sigma/\varepsilon_0 = Q/(\varepsilon_0 A)$.
3. Energy density: $u = \frac{\varepsilon_0}{2}E^2 = \frac{\varepsilon_0}{2}\cdot\frac{Q^2}{\varepsilon_0^2 A^2} = \frac{Q^2}{2\varepsilon_0 A^2}$.
4. Volume between plates: $V_{\text{box}} = A\cdot d$.
5. Total energy: $U = u\cdot V_{\text{box}} = \frac{Q^2 d}{2\varepsilon_0 A}$.
6. Capacitance of parallel plates: $C = \varepsilon_0 A/d$.
7. Standard formula: $U' = Q^2/(2C) = Q^2 d/(2\varepsilon_0 A)$.
8. $U = U'$. ✓

**EVALUATE**:
- Both methods give $U = Q^2 d/(2\varepsilon_0 A)$ — agreement confirms the field-energy interpretation.
- The energy depends on $d$: stretching the plates apart at fixed $Q$ INCREASES the stored energy, because you do positive work against the attractive force between the plates. This force is $F = -dU/dd = -Q^2/(2\varepsilon_0 A)$, which is indeed attractive.
- At fixed voltage $V = Ed = Qd/(\varepsilon_0 A)$, separating the plates instead DECREASES $Q$ (at fixed $V$), so the $Q^2/C$ energy formula needs to be swapped for $U = \frac{1}{2}CV^2$, which then gives a different sign on the force. Both formulas are correct for their respective constraints.
- The calculation extends directly to capacitors filled with a dielectric — one simply replaces $\varepsilon_0$ with $\varepsilon = \varepsilon_0\varepsilon_r$ throughout, showing that a dielectric stores more energy per unit volume at fixed $E$.
