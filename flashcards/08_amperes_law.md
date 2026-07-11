+++
order = 8
subject = "physics"
tags = ["electromagnetism", "amperes-law", "vector-potential", "solenoid", "curl"]
+++

# Electromagnetism — Ampère's Law and the Vector Potential

## 8.1 Circulation of the Magnetic Field

Q: Why does integrating $\mathbf{B}$ around a closed loop in magnetostatics give something proportional to the enclosed current, rather than zero?
A: Because the magnetic field has a non-zero curl where currents flow: $\nabla\times\mathbf{B} = \mu_0\mathbf{J}$. By Stokes's theorem, $\oint\mathbf{B}\cdot d\mathbf{l} = \int(\nabla\times\mathbf{B})\cdot d\mathbf{A} = \mu_0\int\mathbf{J}\cdot d\mathbf{A} = \mu_0 I_{\text{enc}}$. The circulation is proportional to the current piercing any surface bounded by the loop.

## 8.2 Ampère's Law (Integral Form)

C: Ampère's law (integral form): $\oint_C \mathbf{B}\cdot d\mathbf{l} = [\mu_0 I_{\text{enc}}]$, where $I_{\text{enc}}$ is the total current passing through any surface bounded by the loop $C$.

Q: Why is Ampère's law the magnetic counterpart of Gauss's law for electrostatics?
A: Both relate an integral of the field to its sources: Gauss's law relates flux to enclosed charge; Ampère's law relates circulation to enclosed current. Both are consequences of fundamental differential equations ($\nabla\cdot\mathbf{E} = \rho/\varepsilon_0$ and $\nabla\times\mathbf{B} = \mu_0\mathbf{J}$). Both become powerful calculational tools when symmetry reduces the field to a single unknown.

Q: Why is Ampère's law useful only when symmetry fixes the direction and $s$-dependence of $\mathbf{B}$?
A: Like Gauss's law, it provides just one scalar equation (circulation = enclosed current). That can only pin down one unknown scalar function. If a symmetry — azimuthal around a wire, translational along a solenoid, etc. — forces $\mathbf{B}$ to have a definite direction and depend on a single coordinate, the line integral collapses to $B \times \text{length}$ and becomes solvable.

## 8.3 Ampère's Law (Differential Form)

C: Ampère's law (differential form): $\nabla\times\mathbf{B} = [\mu_0\mathbf{J}]$ in magnetostatics.

Q: How does the differential form follow from the integral form?
A: Apply Stokes's theorem to the integral form: $\oint\mathbf{B}\cdot d\mathbf{l} = \int(\nabla\times\mathbf{B})\cdot d\mathbf{A}$ and $I_{\text{enc}} = \int\mathbf{J}\cdot d\mathbf{A}$. Equating and using that the surface is arbitrary gives $\nabla\times\mathbf{B} = \mu_0\mathbf{J}$ point by point. The differential form holds locally at every point in space.

Q: Why is the magnetostatic $\nabla\times\mathbf{B} = \mu_0\mathbf{J}$ inconsistent with charge conservation for time-varying currents?
A: Taking the divergence of both sides gives $0 = \mu_0\nabla\cdot\mathbf{J}$ (because $\nabla\cdot(\nabla\times\text{anything}) = 0$). But the continuity equation says $\nabla\cdot\mathbf{J} = -\partial\rho/\partial t$, which is nonzero when $\rho$ changes in time. This is why Maxwell added the "displacement current" term $\mu_0\varepsilon_0\partial\mathbf{E}/\partial t$ to salvage the law for time-dependent fields.

## 8.4 Field of a Long Wire via Ampère's Law

Q: Derive the field of an infinite straight wire using Ampère's law.
A: By azimuthal symmetry, $\mathbf{B}$ circles the wire at constant $|B|$ on any circle of radius $s$. Taking such a circle as the Amperian loop: $\oint\mathbf{B}\cdot d\mathbf{l} = B(s)\cdot 2\pi s = \mu_0 I_{\text{enc}} = \mu_0 I$. Solving: $B = \mu_0 I/(2\pi s)$, matching the Biot–Savart result without any integration.

C: Using Ampère's law for an infinite straight wire, an Amperian [circle] gives $B \cdot 2\pi s = \mu_0 I$, yielding $B = \mu_0 I/(2\pi s)$.

## 8.5 Field Inside a Solenoid

C: A [solenoid] is a long, tightly wound coil of wire that approximates an infinite current sheet wrapped into a cylinder.

Q: Why is the magnetic field inside an ideal (infinite) solenoid uniform, axial, and equal to $\mu_0 n I$, where $n$ is the number of turns per unit length?
A: Take a rectangular Amperian loop with one side of length $L$ inside the solenoid parallel to the axis, one side outside, and two perpendicular legs. The field outside an infinite solenoid vanishes (from symmetry arguments and the falloff at infinity). The perpendicular legs contribute zero (field is perpendicular to them). Only the inside leg contributes $BL$, and the enclosed current is $nLI$. Ampère gives $BL = \mu_0 nLI$, so $B = \mu_0 nI$.

C: Magnetic field inside an ideal solenoid: $B = [\mu_0 n I]$, with $n$ the number of turns per unit length and $I$ the current per turn.

Q: Why is the field outside an ideal (infinite) solenoid exactly zero?
A: The symmetry of the infinite solenoid makes the exterior field independent of radius, and it must vanish at infinity, so it must be zero everywhere outside. More physically: the azimuthal currents create a field that fully "leaks out" only through the ends — which are at infinity for an ideal solenoid, leaving the exterior field zero.

## 8.5a Pattern Recognition: When to Use Ampère's Law

Q: A problem describes a long straight wire and asks for $\mathbf{B}$. What technique?
A: Ampère's law with a circular Amperian loop coaxial with the wire — azimuthal symmetry collapses the line integral.

Q: A problem describes a long solenoid or toroid. What technique?
A: Ampère's law with a rectangular (solenoid) or circular (toroid) Amperian loop.

Q: A problem describes a finite-length wire or loop, or non-symmetric current. Should you use Ampère's law?
A: No — Biot–Savart law instead. Ampère's law needs translational/rotational symmetry to reduce to one scalar.

Q: A problem describes a current sheet (infinite plane). What technique?
A: Ampère's law with a rectangular loop straddling the sheet (analogous to Gauss-pillbox for surface charge).

## 8.6 Field of a Toroid

Q: Derive the field inside a toroid (a solenoid bent into a circle) with $N$ total turns carrying current $I$.
A: Choose an Amperian loop that is a circle of radius $r$ inside the toroid, concentric with its axis. Symmetry makes $\mathbf{B}$ tangent to this circle with constant magnitude. Enclosed current: $NI$ (one passage per turn). Ampère: $B\cdot 2\pi r = \mu_0 NI$, giving $B = \mu_0 NI/(2\pi r)$. Unlike a solenoid, the field magnitude depends on the radial position inside the toroid.

C: Magnetic field inside a toroid of $N$ turns at radius $r$ from the central axis: $B = [\mu_0 N I/(2\pi r)]$.

## 8.7 The Magnetic Vector Potential

Q: Why does $\nabla\cdot\mathbf{B} = 0$ guarantee the existence of a vector potential $\mathbf{A}$ such that $\mathbf{B} = \nabla\times\mathbf{A}$?
A: Any divergence-free field on a simply connected domain can be written as the curl of some other vector field. Since $\nabla\cdot(\nabla\times\mathbf{A}) \equiv 0$ identically for any smooth $\mathbf{A}$, choosing $\mathbf{B} = \nabla\times\mathbf{A}$ automatically ensures $\nabla\cdot\mathbf{B} = 0$. The vector potential $\mathbf{A}$ is not uniquely determined — adding the gradient of any scalar leaves $\mathbf{B}$ unchanged (gauge freedom).

C: The magnetic vector potential is defined by $\mathbf{B} = [\nabla\times\mathbf{A}]$; it is not unique and can be shifted by the gradient of any scalar (gauge freedom).

Q: What is the Coulomb gauge for the vector potential, and why is it convenient?
A: The Coulomb gauge imposes the additional condition $\nabla\cdot\mathbf{A} = 0$. This removes the gauge freedom (up to harmonic functions vanishing at infinity) and simplifies Ampère's law: $\nabla\times(\nabla\times\mathbf{A}) = \nabla(\nabla\cdot\mathbf{A}) - \nabla^2\mathbf{A} = -\nabla^2\mathbf{A}$, so $\nabla^2\mathbf{A} = -\mu_0\mathbf{J}$ — a vector Poisson equation with the same structure as electrostatic Poisson's equation.

C: The [Coulomb gauge] imposes $\nabla\cdot\mathbf{A} = 0$, simplifying Ampère's law to $\nabla^2\mathbf{A} = -\mu_0\mathbf{J}$.

Q: Why does the Coulomb gauge let us write the magnetic vector potential directly as an integral over current, in analogy with the electrostatic potential?
A: In Coulomb gauge, $\nabla^2\mathbf{A} = -\mu_0\mathbf{J}$ is mathematically identical to three copies of $\nabla^2 V = -\rho/\varepsilon_0$, one for each component. The known Green's function solution gives $\mathbf{A}(\mathbf{r}) = \frac{\mu_0}{4\pi}\int \mathbf{J}(\mathbf{r}')/|\mathbf{r} - \mathbf{r}'|\,d^3r'$ — the magnetostatic analog of the Coulomb potential integral.

C: Vector potential from a current distribution (in Coulomb gauge): $\mathbf{A}(\mathbf{r}) = \frac{\mu_0}{4\pi}\int \mathbf{J}(\mathbf{r}')/[|\mathbf{r} - \mathbf{r}'|]\,d^3r'$.

## 8.8 Why Bother with $\mathbf{A}$?

Q: Why work with the vector potential at all, if $\mathbf{B}$ is what experiments measure?
A: Several reasons: (1) computing $\mathbf{A}$ is often simpler because it's parallel to the current direction, not a cross product; (2) $\mathbf{A}$ is the natural variable in the Lagrangian formulation of charged particles; (3) quantum mechanics couples particles directly to $\mathbf{A}$ (minimal coupling), and the Aharonov–Bohm effect shows that $\mathbf{A}$ has physical reality even in regions where $\mathbf{B} = 0$.

## 8.9 Boundary Conditions on $\mathbf{B}$

Q: What are the boundary conditions on $\mathbf{B}$ at a surface carrying a current sheet of surface current density $\mathbf{K}$?
A: The normal component of $\mathbf{B}$ is continuous (from $\nabla\cdot\mathbf{B} = 0$ applied to a pillbox). The tangential component jumps: $\mathbf{B}_{\text{above}}^{\parallel} - \mathbf{B}_{\text{below}}^{\parallel} = \mu_0\mathbf{K}\times\hat{n}$, from Ampère's law applied to a narrow rectangular loop straddling the surface.

C: At a surface with current density $\mathbf{K}$, the [normal component of $\mathbf{B}$] is continuous; the [tangential component of $\mathbf{B}$] jumps by $\mu_0\mathbf{K}\times\hat{n}$.

## 8.10 Field of a Coaxial Cable — P:/S:

P: A coaxial cable consists of an inner solid cylindrical conductor of radius $a$ carrying steady current $I$ (uniformly distributed over its cross-section, direction along the axis) and an outer thin cylindrical shell of radius $b > a$ carrying the return current $-I$. Using Ampère's law, find the magnetic field in all regions: (i) $r < a$, (ii) $a < r < b$, (iii) $r > b$.

S:
**IDENTIFY**: Cylindrical symmetry, azimuthal field — Ampère's law is the tool of choice.

**PLAN**:
- By symmetry, $\mathbf{B} = B(r)\hat{\phi}$ with $B(r)$ depending only on $r$.
- Take Amperian circles of radius $r$ in each region.
- Compute enclosed current for each region.
- Solve the resulting algebraic equations.

**EXECUTE**:
1. **Inside the inner conductor ($r < a$)**: current enclosed by a circle of radius $r$ is a fraction of $I$ proportional to area: $I_{\text{enc}} = I(r^2/a^2)$. Ampère:
$$B(r)\cdot 2\pi r = \mu_0 I r^2/a^2 \Rightarrow B(r) = \frac{\mu_0 I r}{2\pi a^2}.$$
2. **Between conductors ($a < r < b$)**: Amperian circle encloses the full inner current: $I_{\text{enc}} = I$.
$$B(r)\cdot 2\pi r = \mu_0 I \Rightarrow B(r) = \frac{\mu_0 I}{2\pi r}.$$
3. **Outside the cable ($r > b$)**: enclosed current is $I$ (inner) $+ (-I)$ (outer shell) $= 0$.
$$B(r)\cdot 2\pi r = 0 \Rightarrow B(r) = 0.$$

**EVALUATE**:
- The field grows linearly with $r$ inside the inner conductor (from zero at the axis), peaks at $r = a$ with $B_{\max} = \mu_0 I/(2\pi a)$, decays as $1/r$ in the gap, then vanishes abruptly beyond $r = b$ where the return current cancels the enclosed total.
- Continuity at $r = a$: inside expression gives $\mu_0 Ia/(2\pi a^2) = \mu_0 I/(2\pi a)$; gap expression gives $\mu_0 I/(2\pi a)$ — they agree. ✓
- Discontinuity at $r = b$: gap expression gives $\mu_0 I/(2\pi b)$, outside expression gives zero — the jump corresponds to the surface current density on the outer shell, $K = I/(2\pi b)$, consistent with the boundary condition $\Delta B_{\parallel} = \mu_0 K$.
- The field is entirely contained between the two conductors — this is why coaxial cables don't radiate and are used for high-frequency signal transmission.
- Structural parallel with concentric charged shells (electrostatics): both geometries display a "one-region" nonzero field with a radial-gap analog. Ampère's law here plays the role that Gauss's law plays there.
