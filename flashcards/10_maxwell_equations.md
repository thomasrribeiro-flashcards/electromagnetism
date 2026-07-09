+++
order = 10
subject = "Physics"
tags = ["electromagnetism", "maxwell-equations", "displacement-current", "boundary-conditions"]
+++

# Electromagnetism — Maxwell's Equations

## 10.1 The Inconsistency in Static Ampère's Law

Q: Why does the static Ampère's law $\nabla\times\mathbf{B} = \mu_0\mathbf{J}$ fail for time-varying currents?
A: Taking the divergence of both sides gives $0 = \mu_0\nabla\cdot\mathbf{J}$. But the continuity equation says $\nabla\cdot\mathbf{J} = -\partial\rho/\partial t$, which is nonzero whenever charge densities change. The static form is therefore inconsistent with charge conservation when $\partial\rho/\partial t \neq 0$ — a fatal problem for any time-varying situation, like a charging capacitor.

Q: Why does "the current through a surface bounded by a loop" become ambiguous for a charging capacitor?
A: Consider a loop around the wire leading into a capacitor, and two surfaces bounded by it: one crossing the wire, one passing between the capacitor plates. The wire-crossing surface has current $I$ flowing through it; the plate-crossing surface has zero current — just vacuum. Ampère's law as stated gives two different answers for the same loop, which is impossible.

## 10.2 Maxwell's Displacement Current

Q: What is Maxwell's displacement current, and why does adding it fix Ampère's law?
A: Maxwell added a term $\mu_0\varepsilon_0\partial\mathbf{E}/\partial t$ to the right-hand side of Ampère's law. The "displacement current density" $\mathbf{J}_d = \varepsilon_0\partial\mathbf{E}/\partial t$ is not an actual current — no charges move — but an electric field time derivative. It closes the charging-capacitor loop: the changing $\mathbf{E}$ between the plates plays exactly the role of a current through the gap, making Ampère's law consistent with charge conservation.

C: The displacement current density is $\mathbf{J}_d = [\varepsilon_0\partial\mathbf{E}/\partial t]$, added to the real current in the generalized Ampère–Maxwell law.

Q: Why does adding the displacement current term automatically restore compatibility with the continuity equation?
A: Taking the divergence of $\nabla\times\mathbf{B} = \mu_0(\mathbf{J} + \varepsilon_0\partial\mathbf{E}/\partial t)$ gives $0 = \mu_0\nabla\cdot\mathbf{J} + \mu_0\varepsilon_0\partial(\nabla\cdot\mathbf{E})/\partial t$. Using $\nabla\cdot\mathbf{E} = \rho/\varepsilon_0$, the second term becomes $\mu_0\partial\rho/\partial t$. So $\nabla\cdot\mathbf{J} + \partial\rho/\partial t = 0$ — the continuity equation, automatically satisfied.

## 10.3 The Full Set of Maxwell's Equations

Q: What are the four Maxwell equations in differential form in vacuum?
A:
- Gauss's law: $\nabla\cdot\mathbf{E} = \rho/\varepsilon_0$
- No magnetic monopoles: $\nabla\cdot\mathbf{B} = 0$
- Faraday's law: $\nabla\times\mathbf{E} = -\partial\mathbf{B}/\partial t$
- Ampère–Maxwell law: $\nabla\times\mathbf{B} = \mu_0\mathbf{J} + \mu_0\varepsilon_0\partial\mathbf{E}/\partial t$

Together with the Lorentz force law $\mathbf{F} = q(\mathbf{E} + \mathbf{v}\times\mathbf{B})$, these equations fully specify the classical theory of electromagnetism.

C: Gauss's law in Maxwell's equations: $\nabla\cdot\mathbf{E} = [\rho/\varepsilon_0]$.

C: The no-monopoles law: $\nabla\cdot\mathbf{B} = [0]$, asserting that magnetic field lines have no sources or sinks.

C: Faraday's law in Maxwell's equations: $\nabla\times\mathbf{E} = [-\partial\mathbf{B}/\partial t]$.

C: The Ampère–Maxwell law: $\nabla\times\mathbf{B} = [\mu_0\mathbf{J} + \mu_0\varepsilon_0\partial\mathbf{E}/\partial t]$, including the displacement current.

## 10.4 Integral Form of Maxwell's Equations

Q: What is the integral form of each Maxwell equation, and how does it relate to the differential form?
A:
- $\oint\mathbf{E}\cdot d\mathbf{A} = Q_{\text{enc}}/\varepsilon_0$ (Gauss)
- $\oint\mathbf{B}\cdot d\mathbf{A} = 0$ (no monopoles)
- $\oint\mathbf{E}\cdot d\mathbf{l} = -d\Phi_B/dt$ (Faraday)
- $\oint\mathbf{B}\cdot d\mathbf{l} = \mu_0 I_{\text{enc}} + \mu_0\varepsilon_0\,d\Phi_E/dt$ (Ampère–Maxwell)

Each integral form follows from the differential form by applying the divergence or Stokes theorem and is equivalent for smooth fields.

## 10.5 Two Structural Observations

Q: Why do the curl equations in Maxwell's equations display an asymmetry between electricity and magnetism: Faraday has a minus sign, Ampère–Maxwell does not?
A: The sign difference is Lenz's law in disguise — it's what enforces energy conservation. A changing magnetic field induces an electric field whose induced currents OPPOSE the change; a changing electric field induces a magnetic field that AIDS the change (in the sense that no current-limited back-reaction exists). The minus sign in Faraday's law is the mathematical guarantee that the coupling cannot runaway.

Q: Why does the full set of Maxwell's equations exhibit a striking duality $\mathbf{E}\leftrightarrow c\mathbf{B}$, $\rho \leftrightarrow 0$, $\mathbf{J} \leftrightarrow 0$ in vacuum with no sources?
A: In the vacuum limit, Maxwell's equations are invariant under the exchange $\mathbf{E}\to c\mathbf{B}$ and $\mathbf{B}\to -\mathbf{E}/c$. This "electromagnetic duality" is a clue that electric and magnetic fields are two aspects of a single underlying object — the electromagnetic field tensor of relativity. In the presence of charges, the duality is broken because there are no magnetic charges.

## 10.6 Maxwell's Equations in Matter

Q: How do Maxwell's equations get reformulated inside matter to avoid bookkeeping of bound charges and bound currents?
A: Introduce the auxiliary fields $\mathbf{D} = \varepsilon_0\mathbf{E} + \mathbf{P}$ and $\mathbf{H} = \mathbf{B}/\mu_0 - \mathbf{M}$, where $\mathbf{P}$ is polarization and $\mathbf{M}$ is magnetization. Then the source terms become only the FREE charge and FREE current: $\nabla\cdot\mathbf{D} = \rho_f$ and $\nabla\times\mathbf{H} = \mathbf{J}_f + \partial\mathbf{D}/\partial t$. The homogeneous equations ($\nabla\cdot\mathbf{B} = 0$ and Faraday's law) are unchanged.

C: Maxwell's equations in matter use the auxiliary fields $\mathbf{D} = [\varepsilon_0\mathbf{E} + \mathbf{P}]$ and $\mathbf{H} = [\mathbf{B}/\mu_0 - \mathbf{M}]$ to separate free and bound contributions.

Q: Why are $\mathbf{D}$ and $\mathbf{H}$ mathematically convenient but physically less fundamental than $\mathbf{E}$ and $\mathbf{B}$?
A: Because the Lorentz force law depends on $\mathbf{E}$ and $\mathbf{B}$, not $\mathbf{D}$ and $\mathbf{H}$ — the fields that matter in the force law are $\mathbf{E}$ and $\mathbf{B}$. The auxiliary fields are useful accounting tools for tracking free sources in matter, but they are material-dependent combinations of the fundamental fields with polarization and magnetization.

## 10.7 Boundary Conditions from Maxwell's Equations

Q: What are the four boundary conditions at an interface between two media, derived from the integral forms of Maxwell's equations?
A:
- Normal $\mathbf{D}$ jumps by free surface charge: $D_{\perp,2} - D_{\perp,1} = \sigma_f$
- Normal $\mathbf{B}$ continuous: $B_{\perp,2} = B_{\perp,1}$
- Tangential $\mathbf{E}$ continuous: $\mathbf{E}_{\parallel,1} = \mathbf{E}_{\parallel,2}$
- Tangential $\mathbf{H}$ jumps by free surface current: $\mathbf{H}_{\parallel,2} - \mathbf{H}_{\parallel,1} = \mathbf{K}_f\times\hat{n}$

Each comes from applying Gauss's or Stokes's theorem to a pillbox or narrow loop straddling the interface.

C: Across an interface: the [normal component of $\mathbf{B}$] and the [tangential component of $\mathbf{E}$] are continuous in all cases.

## 10.8 Poynting Vector and Energy Flow

C: The Poynting vector is defined as $\mathbf{S} = (1/\mu_0)\mathbf{E}\times\mathbf{B}$; its units are power per unit area, and it represents the [directional energy flux] of the electromagnetic field.

Q: Why does Poynting's theorem $\partial u/\partial t + \nabla\cdot\mathbf{S} = -\mathbf{J}\cdot\mathbf{E}$ express local energy conservation?
A: The left side is the rate at which field energy at a point either changes in place or flows away; the right side is the rate at which the field does work on charges. If there are no charges, $\mathbf{J}\cdot\mathbf{E} = 0$ and the field energy is conserved locally: whatever leaves one region enters neighboring regions, transported by $\mathbf{S}$. Energy conservation is thus a direct consequence of Maxwell's equations.

C: Poynting's theorem: $\partial u/\partial t + \nabla\cdot\mathbf{S} = [-\mathbf{J}\cdot\mathbf{E}]$, where $u = \varepsilon_0 E^2/2 + B^2/(2\mu_0)$ is the EM energy density.

## 10.9 Momentum in the Electromagnetic Field

Q: Why does the electromagnetic field carry momentum, and what is the momentum density?
A: Maxwell's equations imply that $\mathbf{g} = \mathbf{S}/c^2 = \varepsilon_0\mathbf{E}\times\mathbf{B}$ is a momentum density — the EM field carries linear momentum in addition to energy. This is why light exerts radiation pressure when absorbed or reflected, and it explains the recoil a laser experiences when emitting a photon. Without this momentum, Newton's third law would fail for charges interacting at a distance.

C: Electromagnetic momentum density: $\mathbf{g} = [\varepsilon_0\mathbf{E}\times\mathbf{B}]$, so the field carries momentum as well as energy.

## 10.10 Charging Capacitor as Displacement Current — P:/S:

P: A parallel-plate capacitor with circular plates of radius $R$ is charged at a constant rate $dQ/dt = I$ by a current $I$ flowing into one plate. Ignoring fringe effects, find the magnetic field between the plates as a function of the radial distance $s$ from the axis of the capacitor. Verify consistency with the Ampère–Maxwell law by using a surface that passes between the plates (where no conduction current flows).

S:
**IDENTIFY**: A canonical displacement-current problem. The field between the plates changes with time as charge builds up; the changing $\mathbf{E}$ acts as an effective current source.

**PLAN**:
- Compute the electric field between the plates from Gauss's law.
- Differentiate with respect to time to get $\partial\mathbf{E}/\partial t$.
- Apply the Ampère–Maxwell law to an Amperian circle of radius $s$ inside the gap.
- Solve for $\mathbf{B}(s)$.

**EXECUTE**:
1. Surface charge density on plates (uniformly distributed): $\sigma(t) = Q(t)/(\pi R^2)$.
2. Electric field between the plates (perpendicular to plates): $E(t) = \sigma(t)/\varepsilon_0 = Q(t)/(\varepsilon_0\pi R^2)$.
3. Time derivative: $\partial E/\partial t = (1/(\varepsilon_0\pi R^2))\cdot dQ/dt = I/(\varepsilon_0\pi R^2)$.
4. Displacement current density: $J_d = \varepsilon_0\partial E/\partial t = I/(\pi R^2)$, uniform across the plate area.
5. Amperian circle of radius $s$ between the plates (with $s < R$): the enclosed displacement current is $J_d\cdot\pi s^2 = Is^2/R^2$.
6. Ampère–Maxwell: $\oint\mathbf{B}\cdot d\mathbf{l} = B(s)\cdot 2\pi s = \mu_0\,I_{d,\text{enc}} = \mu_0 I s^2/R^2$.
7. Solve: $B(s) = \mu_0 I s/(2\pi R^2)$ for $s < R$.
8. For $s > R$ (outside the plate radius), the enclosed displacement current is the FULL $I$: $B(s) = \mu_0 I/(2\pi s)$, identical to the field of a long wire carrying current $I$.

**EVALUATE**:
- Inside the plate radius ($s < R$): $B$ grows linearly with $s$ from zero at the axis to $\mu_0 I/(2\pi R)$ at the edge.
- Outside the plate radius ($s > R$): $B$ matches the field of a long wire — continuous with the inside expression at $s = R$. ✓
- Check: using a different surface — a flat disk passing BETWEEN the plates versus one passing through the wire — gives the same $B(s)$ because displacement current exactly replaces the real current where the real current is absent.
- If we had used the naive (static) Ampère's law with a plate-gap surface, we would have concluded $B = 0$ there, contradicting the wire-crossing calculation. The displacement current is necessary for consistency.
- Historically: this paradox is what motivated Maxwell's 1861 extension, and the experimental detection of the resulting electromagnetic waves by Hertz in 1887 established classical electromagnetism in its modern form.
