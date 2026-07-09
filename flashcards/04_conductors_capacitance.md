+++
order = 4
subject = "Physics"
tags = ["electromagnetism", "conductors", "capacitance", "image-charges", "boundary-conditions"]
+++

# Electromagnetism — Conductors and Capacitance

## 4.1 What a Conductor Is

C: A [conductor] is a material with charges that are free to move throughout its bulk in response to any applied electric field.

Q: Why does the electric field inside the bulk of a conductor in electrostatic equilibrium vanish?
A: Any nonzero interior field would push the free charges around. In equilibrium, by definition, the charges are at rest, so the net force on each — and hence the field — must be zero everywhere inside. Reaching equilibrium takes a timescale much shorter than most experiments, so the idealization is excellent.

C: In a conductor in electrostatic equilibrium, the interior electric field is [zero] and excess charge resides only on the [surface].

## 4.2 Why Charge Sits on the Surface

Q: Why does any excess charge on a conductor migrate to the surface in electrostatic equilibrium?
A: Gauss's law with $\mathbf{E} = 0$ inside gives $\rho = 0$ throughout the interior. So there can be no volume charge density inside — all excess charge must sit in a thin layer on the outer (or inner) surface where the boundary allows it. The thickness of this layer is in practice a few atomic diameters; for classical purposes it is a mathematical surface.

## 4.3 Field at a Conductor Surface

Q: Why must the electric field just outside a conductor be perpendicular to the surface?
A: If $\mathbf{E}$ had a tangential component, free charges at the surface would feel a lateral force and slide along it — violating equilibrium. So only the normal component can be nonzero, and its magnitude is set by the local surface charge density.

C: Just outside a conductor in equilibrium, the field is $\mathbf{E} = [\sigma/\varepsilon_0]\,\hat{n}$, where $\sigma$ is the local surface charge density and $\hat{n}$ is the outward [normal].

Q: Why is the field just outside a conductor $\sigma/\varepsilon_0$ rather than the $\sigma/(2\varepsilon_0)$ of an isolated charged plane?
A: For an isolated plane, the field comes entirely from that plane and splits equally between the two sides, giving $\sigma/(2\varepsilon_0)$ on each. For a conductor, the interior field must cancel: the contribution from OTHER charges in the system exactly cancels the $\sigma/(2\varepsilon_0)$ from the local surface charge inside, and ADDS to it outside — giving $0$ inside and $\sigma/\varepsilon_0$ outside.

## 4.4 Conductors Are Equipotentials

Q: Why is the entire body of a conductor at a single potential in electrostatic equilibrium?
A: Because $\mathbf{E} = 0$ inside, the line integral of $\mathbf{E}$ between any two points in the conductor is zero, so $V$ is the same everywhere. The surface of a conductor is therefore an equipotential surface, and the field lines just outside meet it perpendicularly (as they must at any equipotential).

C: The interior and surface of a conductor in equilibrium form a single [equipotential region], so field lines meet conductor surfaces at [right angles].

## 4.5 Induced Charges on a Neutral Conductor

Q: Why does a neutral conductor placed in an external field develop surface charges without becoming charged overall?
A: The free charges inside redistribute: electrons pile up on the side facing away from the external $\mathbf{E}$ direction, leaving the opposite side positively charged. The redistribution continues until the induced charges produce a field that exactly cancels the external field inside — at that point, equilibrium is restored. Total charge is still zero; only its distribution has changed.

C: A neutral conductor in an external field develops [induced surface charges] that exactly cancel the external field in the conductor's interior, a phenomenon called [electrostatic shielding].

## 4.6 The Faraday Cage

Q: Why does a hollow conductor shield its interior from external electric fields (the Faraday cage)?
A: Induced charges arrange themselves on the conductor's outer surface to cancel the external field inside the conducting material. The interior cavity, surrounded entirely by conductor at a single potential, satisfies Laplace's equation with constant boundary conditions — and its unique solution is $V = \text{const}$, giving $\mathbf{E} = 0$ throughout the cavity.

Q: Why does a Faraday cage NOT shield against charges placed INSIDE the cavity?
A: The shielding is asymmetric: induced charges on the inner surface of the cavity reflect any interior charges, and charges on the outer surface reflect exterior charges. An interior source still produces a field in the cavity and can even induce an equal-and-opposite charge on the conductor's outer surface — so a compass inside can detect charges placed inside, but not those placed outside.

## 4.7 The Method of Images

Q: What is the method of images for electrostatic problems?
A: A technique that replaces a complicated boundary-value problem with a simpler one in free space containing fictitious "image" charges. The images are chosen so that together with the real charges, they reproduce the required potential on the original boundary. By the uniqueness theorem, the resulting field is identical to the true field in the physical region.

C: The method of images solves for the field of a point charge near a [grounded conductor] by placing fictitious charges in the non-physical region to reproduce the [boundary conditions].

Q: For a point charge $+q$ at distance $d$ above an infinite grounded conducting plane, what is the image and what is the resulting field in the upper half-space?
A: Image: a charge $-q$ at distance $d$ BELOW the plane. The resulting field in the upper half-space is identical to the field of a dipole-like pair. The potential vanishes on the plane (halfway between equal and opposite charges), satisfying the grounded-plane condition, and uniqueness guarantees this matches the real problem.

Q: Why does the method of images work only in the PHYSICAL region, not in the image region?
A: Because the image charges don't actually exist — placing a real charge in the image region would be a different problem entirely. The method gives the correct $V$ and $\mathbf{E}$ only in the region where the original problem was posed. The field in the non-physical region is whatever happens inside the conductor (zero for a grounded conductor).

## 4.8 Capacitance

C: [Capacitance] is the ratio $C = Q/V$, measuring how much charge must be placed on a pair of conductors to produce a given potential difference between them.

Q: Why is the capacitance a purely geometric property of the conductor arrangement, independent of the applied charge or voltage?
A: In a linear electrostatic problem, doubling the charge on each conductor doubles the potential everywhere — both $Q$ and $V$ scale together. Their ratio depends only on the shapes and positions of the conductors, not on how much charge you put on them.

C: Capacitance is a [geometric] quantity: it depends only on the shape and configuration of the conductors, not on the charge or voltage applied.

Q: What is the capacitance of a parallel-plate capacitor with plate area $A$ separated by distance $d$?
A: $C = \varepsilon_0 A/d$. From $E = \sigma/\varepsilon_0 = Q/(\varepsilon_0 A)$ and $V = Ed = Qd/(\varepsilon_0 A)$, the ratio $Q/V$ gives $\varepsilon_0 A/d$. Larger plates store more charge per volt; larger gaps reduce $C$ because the potential difference for a given charge becomes larger.

C: Parallel-plate capacitor with plate area $A$ and separation $d$: $C = [\varepsilon_0 A/d]$.

## 4.9 Energy Stored in a Capacitor

Q: Why is the energy stored in a capacitor $U = \frac{1}{2}CV^2 = \frac{Q^2}{2C}$, not simply $QV$?
A: Charging the capacitor builds up $V$ gradually: at intermediate charge $q$, the potential is $q/C$ and the differential work to add $dq$ more is $(q/C)\,dq$. Integrating from 0 to $Q$ gives $\frac{1}{2}Q^2/C = \frac{1}{2}CV^2$. The factor of $\frac{1}{2}$ is the average potential during charging, not the final value.

C: The energy stored in a capacitor can be written as $U = [\tfrac{1}{2}CV^2] = \tfrac{Q^2}{2C} = \tfrac{1}{2}QV$ — all three forms are equivalent.

## 4.10 Capacitors in Series and Parallel

Q: Why do capacitors in PARALLEL add directly ($C_{\text{tot}} = C_1 + C_2$), while capacitors in SERIES add reciprocally ($1/C_{\text{tot}} = 1/C_1 + 1/C_2$)?
A: In parallel, both capacitors share the same voltage $V$, so the total charge is $Q_1 + Q_2 = (C_1 + C_2)V$ — capacitances add. In series, the same charge $Q$ sits on both (conservation of charge on the middle wire), but the voltages add: $V = V_1 + V_2 = Q(1/C_1 + 1/C_2)$ — inverse capacitances add.

C: Capacitors in parallel: $C_{\text{tot}} = [C_1 + C_2]$. Capacitors in series: $1/C_{\text{tot}} = [1/C_1 + 1/C_2]$.

## 4.11 Capacitance of a Spherical Capacitor — P:/S:

P: A spherical capacitor consists of two concentric conducting shells: an inner shell of radius $a$ at potential $V_a$ and an outer shell of radius $b > a$ at potential $V_b = 0$ (grounded). The inner shell carries charge $+Q$. Find the capacitance $C$ and the energy stored in the capacitor.

S:
**IDENTIFY**: Spherical geometry — symmetry gives a trivial Gauss's law application. Then compute $V$ by integration and $C = Q/V$.

**PLAN**:
- Use Gauss's law on a sphere of radius $r$ with $a < r < b$ to find $E(r)$ between the shells.
- Integrate $-E\,dr$ from $r = b$ to $r = a$ to find the potential difference.
- Take the ratio $C = Q/V$.
- Compute the energy via $U = \frac{1}{2}Q^2/C$ as a cross-check.

**EXECUTE**:
1. Field between the shells (Gaussian sphere of radius $r$ encloses $+Q$):
$$E(r) = \frac{Q}{4\pi\varepsilon_0 r^2},\quad a < r < b.$$
2. Potential difference: $V_a - V_b = -\int_b^a E\,dr = \int_a^b \frac{Q}{4\pi\varepsilon_0 r^2}\,dr = \frac{Q}{4\pi\varepsilon_0}\left(\frac{1}{a} - \frac{1}{b}\right)$.
3. With $V_b = 0$, we have $V = V_a = \frac{Q}{4\pi\varepsilon_0}\cdot\frac{b - a}{ab}$.
4. Capacitance: $C = Q/V = 4\pi\varepsilon_0\cdot\frac{ab}{b - a}$.
5. Energy: $U = \frac{1}{2}\frac{Q^2}{C} = \frac{Q^2(b - a)}{8\pi\varepsilon_0 ab}$.

**EVALUATE**:
- Limit $b \to \infty$: $C \to 4\pi\varepsilon_0 a$. This is the capacitance of an isolated sphere of radius $a$ with the "other plate" at infinity — a good consistency check.
- Limit $b \to a$ (thin shell gap): $C \to 4\pi\varepsilon_0 ab/(b - a) \to \infty$. As the shells get close, the parallel-plate-like approximation kicks in: $C \approx \varepsilon_0 A/(b - a)$ with $A \approx 4\pi a^2$, matching $C \to 4\pi\varepsilon_0 a^2/(b - a)$. ✓
- Units: $[\varepsilon_0 \cdot \text{length}] = \text{F}$. ✓
- The result $C = 4\pi\varepsilon_0\,ab/(b - a)$ can be memorized as "parallel-plate-like times a geometric correction," and is used to estimate the capacitance of coaxial spheres in vacuum-tube design and Van de Graaff generators.
