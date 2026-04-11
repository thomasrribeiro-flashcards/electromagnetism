+++
order = 7
tags = ["electromagnetism", "magnetostatics", "lorentz-force", "biot-savart", "magnetic-field"]
+++

# Electromagnetism — Magnetostatics

## 7.1 What Magnetostatics Is

Q: What is magnetostatics and what idealization does it make?
A: Magnetostatics studies the magnetic field produced by steady (time-independent) currents. It assumes $\partial\mathbf{E}/\partial t = 0$, so the electric and magnetic fields decouple and one can solve for $\mathbf{B}$ alone. Only currents can produce $\mathbf{B}$ in this limit — there are no magnetic charges.

C: Magnetostatics assumes [steady currents] and time-independent fields, letting $\mathbf{B}$ be studied independently of the electric sector.

Q: Why is there no "magnetic Coulomb's law" analogous to the inverse-square force between electric charges?
A: Because no magnetic monopoles have ever been found: the fundamental source of magnetic field is currents (and intrinsic spin), not magnetic charges. Magnetic field lines form closed loops — they never start or end anywhere. The absence of magnetic charges is a separate Maxwell equation: $\nabla\cdot\mathbf{B} = 0$.

C: There are no [magnetic monopoles]: $\nabla\cdot\mathbf{B} = 0$, so magnetic field lines form closed loops with no beginning or end.

## 7.2 The Lorentz Force

Q: What is the Lorentz force on a moving charge in an electromagnetic field?
A: $\mathbf{F} = q(\mathbf{E} + \mathbf{v}\times\mathbf{B})$. The electric part is the familiar Coulomb force; the magnetic part is proportional to velocity, perpendicular to both $\mathbf{v}$ and $\mathbf{B}$, and vanishes for charges at rest. This formula is the DEFINITION of the fields $\mathbf{E}$ and $\mathbf{B}$ in terms of measurable forces on test charges.

C: Lorentz force on a charge $q$ with velocity $\mathbf{v}$: $\mathbf{F} = [q(\mathbf{E} + \mathbf{v}\times\mathbf{B})]$.

Q: Why does the magnetic force do NO WORK on a charged particle, even as it changes the particle's direction?
A: Because the force $q\mathbf{v}\times\mathbf{B}$ is always perpendicular to $\mathbf{v}$. Work is $\mathbf{F}\cdot d\mathbf{l} = \mathbf{F}\cdot\mathbf{v}\,dt = 0$. Magnetic forces change the direction of motion but not the speed — charged particles in a pure magnetic field travel at constant kinetic energy, typically on circular or helical paths.

## 7.3 Motion in a Uniform Magnetic Field

Q: Why does a charged particle moving in a uniform magnetic field trace a circle (if $\mathbf{v}\perp\mathbf{B}$)?
A: The magnetic force is always perpendicular to the velocity and constant in magnitude ($qvB$). A constant centripetal force with speed held fixed produces uniform circular motion. The radius is determined by balancing the magnetic force with the required centripetal acceleration: $qvB = mv^2/r$, giving $r = mv/(qB)$.

C: Radius of circular motion of a charged particle in a magnetic field (gyroradius): $r = [mv/(qB)]$.

Q: What is the cyclotron frequency of a charged particle in a uniform magnetic field?
A: $\omega_c = qB/m$, independent of speed. This is one of the remarkable properties of non-relativistic motion in a magnetic field: faster particles trace larger circles, but at the same angular rate. The cyclotron (Lawrence 1929) exploits this to accelerate particles — an alternating voltage at $\omega_c$ kicks them forward on every revolution.

C: Cyclotron frequency: $\omega_c = [qB/m]$, independent of the particle's speed in the non-relativistic limit.

Q: Why does a charged particle with a velocity component parallel to $\mathbf{B}$ follow a helix rather than a circle?
A: The magnetic force acts only on the velocity component PERPENDICULAR to $\mathbf{B}$; the parallel component is unaffected. The particle circles in the perpendicular plane at the cyclotron frequency while drifting uniformly along the field line — tracing out a helix. This is why magnetic fields can confine charged particles along their lines (magnetic mirrors, tokamaks).

## 7.4 Force on a Current-Carrying Wire

Q: Why is the magnetic force on a current-carrying wire $d\mathbf{F} = I\,d\mathbf{l}\times\mathbf{B}$?
A: Sum the Lorentz forces on all the moving charges inside the wire. Each carrier experiences $q\mathbf{v}_d\times\mathbf{B}$, and there are $nA\,dl$ carriers in a length $dl$. The total force on that segment is $(nA\,dl)(q\mathbf{v}_d)\times\mathbf{B} = I\,d\mathbf{l}\times\mathbf{B}$, using $I = nqv_dA$. Direction: given by the right-hand rule on $d\mathbf{l}\times\mathbf{B}$.

C: Force per unit length on a current-carrying wire: $d\mathbf{F}/dl = [I\,\hat{l}\times\mathbf{B}]$, where $\hat{l}$ is the direction of current flow.

## 7.5 The Biot–Savart Law

Q: What does the Biot–Savart law give for the magnetic field produced by a steady current?
A: $\mathbf{B}(\mathbf{r}) = \frac{\mu_0}{4\pi}\int \frac{I\,d\mathbf{l}'\times(\mathbf{r} - \mathbf{r}')}{|\mathbf{r} - \mathbf{r}'|^3}$. Each current element $I\,d\mathbf{l}'$ contributes a field whose magnitude falls as $1/r^2$ and whose direction is perpendicular to both the current direction and the separation vector. The integral extends over the entire current distribution.

C: Biot–Savart law: $\mathbf{B}(\mathbf{r}) = \frac{\mu_0}{4\pi}\int I\,d\mathbf{l}'\times(\mathbf{r} - \mathbf{r}')/[|\mathbf{r} - \mathbf{r}'|^3]$, analogous to the Coulomb field integral for electrostatics.

Q: Why does the Biot–Savart law involve a CROSS PRODUCT between the current direction and the separation vector, unlike Coulomb's law which is simply a scalar times a unit vector?
A: Because the magnetic field has a "handedness" — it circles the current direction according to the right-hand rule, rather than pointing radially from its source. The cross product encodes this chiral structure: $d\mathbf{l}'\times(\mathbf{r} - \mathbf{r}')$ is perpendicular to both the current and the line of separation, which is the direction of the magnetic field circulating around the current.

## 7.6 Field of a Long Straight Wire

Q: What is the magnetic field at a perpendicular distance $s$ from an infinite straight wire carrying current $I$?
A: $\mathbf{B} = \frac{\mu_0 I}{2\pi s}\hat{\phi}$, where $\hat{\phi}$ circles the wire in the right-hand sense. The $1/s$ falloff matches the infinite-line charge electric field structurally, but the direction is azimuthal (around the wire) rather than radial (away from the line).

C: Magnetic field of an infinite straight wire: $B = [\mu_0 I/(2\pi s)]$, with field lines forming [concentric circles] around the wire.

## 7.7 Field on the Axis of a Circular Loop

Q: What is the magnetic field on the axis of a circular loop of radius $R$ carrying current $I$, at distance $z$ from the center?
A: $B_z = \frac{\mu_0 I R^2}{2(R^2 + z^2)^{3/2}}$. At the center ($z = 0$): $B = \mu_0 I/(2R)$. Far away ($z \gg R$): $B \approx \mu_0 I R^2/(2z^3)$ — a dipole falloff. The direction on-axis is perpendicular to the loop, by the right-hand rule.

C: Magnetic field at the center of a circular loop: $B = [\mu_0 I/(2R)]$, at the center of a single turn.

Q: Why does the on-axis field of a current loop fall off as $1/z^3$ at large distances, not $1/z^2$?
A: Because a current loop has no net "magnetic charge" — only a magnetic dipole moment. Fields of magnetic dipoles, like electric dipoles, fall off as $1/r^3$: the leading $1/r^2$ contributions from different parts of the loop partially cancel, leaving the next-order contribution to dominate.

## 7.8 Magnetic Dipole Moment

C: The [magnetic dipole moment] of a flat current loop of area $A$ carrying current $I$ is $\mathbf{m} = I A\hat{n}$, where $\hat{n}$ is normal to the loop via the right-hand rule.

Q: Why does the torque on a magnetic dipole in an external field take the form $\boldsymbol{\tau} = \mathbf{m}\times\mathbf{B}$, directly analogous to the electric-dipole torque?
A: Integrate the Lorentz force on each segment of the current loop in an external $\mathbf{B}$: the force adds to zero for a uniform field, but the torques on opposite sides of the loop don't cancel. The net torque points to rotate $\hat{n}$ toward $\mathbf{B}$, with magnitude $IAB\sin\theta$. This is $|\mathbf{m}\times\mathbf{B}|$, matching the electric case.

C: Torque on a magnetic dipole in an external field: $\boldsymbol{\tau} = [\mathbf{m}\times\mathbf{B}]$, tending to align the moment with $\mathbf{B}$.

Q: What is the potential energy of a magnetic dipole in an external field?
A: $U = -\mathbf{m}\cdot\mathbf{B}$. Its minimum is achieved when $\mathbf{m}$ is aligned parallel to $\mathbf{B}$ (stable equilibrium). Anti-aligned is a maximum (unstable). Rotating the dipole does work against this potential — the basis for magnetic resonance techniques.

## 7.9 Field Far from a Current Loop — P:/S:

P: A circular loop of radius $R$ carries steady current $I$ and lies in the $xy$-plane, centered at the origin. Find the magnetic field on the $z$-axis at distance $z$ and take the limit $z \gg R$ to extract the dipole form of the field. Express the answer in terms of the magnetic dipole moment of the loop.

S:
**IDENTIFY**: Biot–Savart applied to a symmetric closed current loop. On-axis symmetry makes the problem one-dimensional.

**PLAN**:
- Parameterize the loop and write $d\mathbf{l}'$ and the separation vector in terms of the loop angle.
- Use symmetry to show that only the $z$-component of $\mathbf{B}$ survives after integration around the loop.
- Integrate around the loop.
- Take $z \gg R$ and identify the dipole form.

**EXECUTE**:
1. Field point: $(0, 0, z)$. Source point on loop: $(R\cos\phi, R\sin\phi, 0)$. Separation: $(\mathbf{r} - \mathbf{r}') = (-R\cos\phi, -R\sin\phi, z)$, with magnitude $\sqrt{R^2 + z^2}$.
2. Current element: $I\,d\mathbf{l}' = IR\,d\phi\,(-\sin\phi, \cos\phi, 0)$.
3. Cross product $d\mathbf{l}'\times(\mathbf{r} - \mathbf{r}')$: computing and keeping only the $z$-component (others cancel by symmetry after integration) gives $(R\cos\phi\cdot R\cos\phi + R\sin\phi\cdot R\sin\phi)\,d\phi\,\hat{z} = R^2\,d\phi\,\hat{z}$.
4. Biot–Savart: $\mathbf{B}(0,0,z) = \frac{\mu_0 I}{4\pi(R^2 + z^2)^{3/2}}\int_0^{2\pi}R^2\,d\phi\,\hat{z} = \frac{\mu_0 I R^2}{2(R^2 + z^2)^{3/2}}\hat{z}$.
5. Magnetic dipole moment of the loop: $\mathbf{m} = IA\hat{z} = I\pi R^2\,\hat{z}$.
6. Far-field limit $z \gg R$: $(R^2 + z^2)^{3/2} \approx z^3$, so
$$\mathbf{B}(0,0,z) \approx \frac{\mu_0 I R^2}{2 z^3}\hat{z} = \frac{\mu_0}{4\pi}\cdot\frac{2IR^2\pi}{z^3}\hat{z} = \frac{\mu_0}{4\pi}\cdot\frac{2m}{z^3}\hat{z}.$$

**EVALUATE**:
- On-axis far-field result: $B_z = \mu_0 m/(2\pi z^3)$, matching the general formula $B_{\text{dipole}} = \frac{\mu_0}{4\pi}\frac{2m\cos\theta}{r^3}$ along the axis ($\theta = 0$).
- Limit $z = 0$: $B = \mu_0 I/(2R)$, the field at the center of the loop.
- Limit $z \to \infty$: $B \to 0$ as $1/z^3$ — a dipole falloff, not $1/z^2$. The loop has no net "charge" (no monopole), so the leading multipole is the dipole.
- Structural parallel: the electric dipole on axis gives $E = 2p/(4\pi\varepsilon_0 r^3)$; the magnetic result has the same $2m/r^3$ form, with $\mu_0/(4\pi)$ replacing $1/(4\pi\varepsilon_0)$. The underlying geometry is identical — both sources are "pure dipoles" at large distances.
- Application: the dipole formula is the starting point for calculating atomic and nuclear magnetic moments, planetary magnetic fields, and the magnetization of bar magnets from current-loop models.
