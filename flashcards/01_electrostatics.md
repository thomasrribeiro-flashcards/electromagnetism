+++
order = 1
subject = "Physics"
tags = ["electromagnetism", "electrostatics", "coulomb", "electric-field", "superposition"]
+++

# Electromagnetism — Electrostatics

## 1.1 What Electrostatics Is

Q: What is electrostatics and what simplifying assumption does it rely on?
A: Electrostatics is the study of electric phenomena produced by charges that are stationary (or, more precisely, unchanging in time). It assumes all currents are zero and all fields are time-independent, which decouples the electric field from the magnetic field and lets us solve for $\mathbf{E}$ alone.

C: Electrostatics assumes [stationary charges] and time-independent fields, so the electric and magnetic sectors can be treated [independently].

## 1.2 Charge and Its Properties

C: Electric [charge] is a fundamental property of matter responsible for all electromagnetic interactions; it comes in two signs, conventionally positive and negative.

Q: What does it mean for electric charge to be quantized, and why does that matter for classical electromagnetism?
A: All observed free charges are integer multiples of the elementary charge $e$. Classical electromagnetism works with continuous charge distributions regardless, because macroscopic charges contain enormous numbers of elementary charges — quantization is invisible at that scale, just as discrete atoms are invisible when describing water as a fluid.

C: Electric charge is [quantized] in units of $e$, and the total charge of an isolated system is [conserved] — both independently verified to high precision.

Q: Why is charge conservation a deeper principle than merely a bookkeeping rule?
A: Charge conservation follows from a gauge symmetry of the underlying theory (Noether's theorem applied to $U(1)$ symmetry). It is not an assumption added to Maxwell's equations but a consequence of their structure, and is exact to all orders — no experiment has ever detected a violation.

## 1.3 Coulomb's Law

Q: What does Coulomb's law state for the force between two point charges?
A: The electrostatic force on charge $q_1$ due to charge $q_2$ is $\mathbf{F}_{12} = \frac{1}{4\pi\varepsilon_0}\frac{q_1 q_2}{r^2}\hat{r}_{12}$, where $r$ is the separation and $\hat{r}_{12}$ points from $q_2$ to $q_1$. The force is along the line joining them, proportional to the product of charges, and falls off as the inverse square of distance.

C: Coulomb's law: $\mathbf{F}_{12} = \frac{1}{4\pi\varepsilon_0}\frac{q_1 q_2}{r^2}\hat{r}_{12}$, with the force directed [along the line joining] the two charges.

Q: Why is the $1/r^2$ dependence in Coulomb's law not an arbitrary empirical fit but a geometric necessity?
A: Field lines emanating isotropically from a point source spread out over spheres whose area grows as $r^2$. If the total flux is conserved (no lines created or destroyed in empty space), the field density must fall as $1/r^2$. This is the same reason gravity, sound intensity, and light intensity all obey inverse-square laws — they all come from flux spreading over spherical surfaces in 3D.

C: The inverse-square falloff in Coulomb's law follows from [flux conservation] on spheres in 3D space; in $d$-dimensional space, the analogous law would be $1/r^{d-1}$.

## 1.4 Superposition

Q: What is the principle of superposition for electrostatic forces?
A: The total force on a test charge due to a collection of source charges is the vector sum of the forces each source charge would exert individually. Each pair interaction is independent: the presence of a third charge does not modify the force between the first two. This principle converts the two-body Coulomb law into a many-body tool.

C: Electrostatic superposition: the total force on a test charge equals the [vector sum] of the pairwise Coulomb forces from each source charge; each pair interaction is [independent].

Q: Why is superposition a non-trivial property that we should not take for granted?
A: It fails in nonlinear media (e.g., ferromagnetic materials) and for strong fields where the vacuum itself becomes nonlinear (QED effects at enormous field strengths). That linear superposition works perfectly for electrostatic interactions in vacuum is an empirical fact tied to the linearity of Maxwell's equations in free space.

## 1.5 The Electric Field

Q: Why introduce an electric field $\mathbf{E}$ instead of working directly with forces between charges?
A: Because the field is a property of the surrounding space, not a relation between two specific objects. It lets us describe "what would happen if a test charge were placed here" without actually placing one, and cleanly generalizes to time-dependent situations where forces at a distance fail (retardation effects). The field is also what carries energy and momentum away as radiation.

C: The electric field at a point is defined as $\mathbf{E} = \mathbf{F}/q$ in the limit where the [test charge] $q$ is small enough to not disturb the source distribution.

C: The electric field of a point charge $Q$ at the origin: $\mathbf{E}(\mathbf{r}) = \frac{1}{4\pi\varepsilon_0}\frac{Q}{r^2}\hat{r}$, directed [radially outward] for positive $Q$.

Q: Why must the test charge be taken in the limit $q \to 0$ when measuring a field?
A: A finite test charge can itself polarize or displace the source charges, changing the very distribution whose field we want to measure. Taking $q \to 0$ formally removes this back-reaction, giving us the field as it would be in the test charge's absence.

## 1.6 Continuous Charge Distributions

Q: How does Coulomb's law generalize when charges form a continuous distribution?
A: Replace the sum over discrete charges with an integral weighted by the charge density. For a volume density $\rho(\mathbf{r}')$, the field at $\mathbf{r}$ is $\mathbf{E}(\mathbf{r}) = \frac{1}{4\pi\varepsilon_0}\int\frac{\rho(\mathbf{r}')}{|\mathbf{r} - \mathbf{r}'|^3}(\mathbf{r} - \mathbf{r}')\,d^3r'$. Surface charges $\sigma$ and line charges $\lambda$ give analogous integrals.

C: The electric field from a continuous charge distribution is $\mathbf{E}(\mathbf{r}) = \frac{1}{4\pi\varepsilon_0}\int \frac{\rho(\mathbf{r}')\,(\mathbf{r} - \mathbf{r}')}{|\mathbf{r} - \mathbf{r}'|^3}\,d^3r'$, where the integrand depends on the [source position] $\mathbf{r}'$.

Q: Why does the integral form inherit the inverse-square falloff even though we are integrating over extended sources?
A: Each infinitesimal element $\rho\,d^3r'$ acts as a point charge and produces its own $1/r^2$ field. The total is a vector sum (integral) of many such point-charge contributions, so the $1/r^2$ structure is preserved at the level of the integrand. Only the geometry of the source changes the result, not the fundamental scaling.

## 1.7 Field Lines

Q: What are electric field lines, and what rules do they follow?
A: Imaginary curves that are everywhere tangent to the electric field. They start on positive charges and end on negative charges (or at infinity), never cross each other, and their density encodes field strength: closely packed lines mean a strong field. They are a visualization aid, not a physical object.

Q: Why do electric field lines never cross?
A: Because the electric field is a single-valued vector at every point in space — it cannot point in two directions simultaneously. Two crossing lines would demand two different tangent vectors at the crossing point, which is impossible.

## 1.8 Symmetry in Electrostatics

Q: Why does exploiting symmetry often turn impossible integrals into one-line answers?
A: Symmetries constrain the direction and spatial dependence of $\mathbf{E}$ before any calculation. If a distribution is spherically symmetric, the field must be radial and depend only on $r$ — reducing three components and three variables to one unknown function of one variable. The same reasoning applies to cylindrical and planar symmetries.

C: A [spherically symmetric] charge distribution produces a field that is purely radial and depends only on $r$; a [cylindrically symmetric] distribution produces a field depending only on the perpendicular distance from the axis.

## 1.9 Force on a Dipole in an External Field

C: An [electric dipole] consists of two equal and opposite charges $\pm q$ separated by a small displacement $\mathbf{d}$; its dipole moment is $\mathbf{p} = q\mathbf{d}$, pointing from the negative to the positive charge.

Q: Why does a uniform electric field exert zero net force on a dipole but a nonzero torque?
A: The forces on the two charges are $+q\mathbf{E}$ and $-q\mathbf{E}$, which cancel as a sum — no net force. But they act at different points, so they produce a couple. The torque is $\boldsymbol{\tau} = \mathbf{p}\times\mathbf{E}$, which tends to align the dipole with the field.

C: The torque on an electric dipole in a uniform field is $\boldsymbol{\tau} = [\mathbf{p}\times\mathbf{E}]$; the potential energy is $U = -\mathbf{p}\cdot\mathbf{E}$.

Q: Why does a dipole in a NON-uniform field experience a net force as well as a torque?
A: The two charges of the dipole sit at slightly different points, so they sample slightly different field strengths. The net force is $\mathbf{F} = (\mathbf{p}\cdot\nabla)\mathbf{E}$, proportional to the gradient of $\mathbf{E}$. In a uniform field this gradient vanishes, recovering the zero-force result.

## 1.10 Field of a Line Charge — P:/S:

P: Compute the electric field at a perpendicular distance $s$ from the middle of a uniformly charged line of total length $2L$ carrying charge per unit length $\lambda$. Take the limit $L \to \infty$ at the end.

S:
**IDENTIFY**: A continuous-distribution integral with symmetry. By symmetry, only the component of $\mathbf{E}$ perpendicular to the line survives the integral.

**PLAN**:
- Place the line along the $z$-axis, field point at distance $s$ from the middle in the $\hat{s}$ direction.
- Write the contribution from an element $dz$ at position $z$, whose distance to the field point is $\sqrt{s^2 + z^2}$.
- Symmetry kills the $z$-component — integrate only the perpendicular component.
- Take $L \to \infty$ to recover the infinite-wire result.

**EXECUTE**:
1. Element of charge: $dq = \lambda\,dz$. Distance from element to field point: $r = \sqrt{s^2 + z^2}$.
2. Field magnitude from element: $dE = \frac{\lambda\,dz}{4\pi\varepsilon_0(s^2 + z^2)}$.
3. Perpendicular component (project onto $\hat{s}$): multiply by $s/r = s/\sqrt{s^2+z^2}$:
$$dE_s = \frac{\lambda s\,dz}{4\pi\varepsilon_0 (s^2 + z^2)^{3/2}}.$$
4. Integrate from $z = -L$ to $z = +L$:
$$E_s = \frac{\lambda s}{4\pi\varepsilon_0}\int_{-L}^{L}\frac{dz}{(s^2 + z^2)^{3/2}} = \frac{\lambda s}{4\pi\varepsilon_0}\cdot\frac{2L}{s^2\sqrt{s^2 + L^2}}.$$
5. Simplify: $E_s = \frac{\lambda}{4\pi\varepsilon_0 s}\cdot\frac{2L}{\sqrt{s^2 + L^2}}$.
6. Limit $L \to \infty$: $2L/\sqrt{s^2 + L^2} \to 2$, giving $E_s = \frac{\lambda}{2\pi\varepsilon_0 s}$.

**EVALUATE**:
- The field falls off as $1/s$ for an infinite line, slower than the $1/r^2$ of a point charge — because adding line length contributes new charge along the way, partially compensating the geometric spreading.
- Units: $[\lambda/(\varepsilon_0 s)] = (\text{C}/\text{m}) \cdot (\text{V m}/\text{C})/\text{m} = \text{V}/\text{m}$. ✓
- Limit $s \gg L$: the expression reduces to $\frac{(2L\lambda)}{4\pi\varepsilon_0 s^2}$, the field of a point charge with total charge $2L\lambda$ — the line looks like a point at large distance. ✓
- The $1/s$ law will reappear via Gauss's law in the next chapter, requiring a single line of algebra instead of the full integral.
