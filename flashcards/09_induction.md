+++
order = 9
subject = "Physics"
tags = ["electromagnetism", "induction", "faraday", "lenz", "inductance"]
+++

# Electromagnetism — Electromagnetic Induction

## 9.1 Why Induction Matters

Q: What new physics does Faraday's law of induction introduce that static electromagnetism cannot explain?
A: It shows that a changing magnetic field produces an electric field — even in a region with no charges. This breaks the strict separation between electric and magnetic phenomena that held in electrostatics and magnetostatics, coupling the two fields together. Without this coupling, electromagnetic waves and radiation would not exist.

## 9.2 Magnetic Flux

C: [Magnetic flux] through a surface is the surface integral of the magnetic field: $\Phi_B = \int_S \mathbf{B}\cdot d\mathbf{A}$.

Q: Why is magnetic flux independent of the CHOICE of surface (as long as the surface is bounded by the same loop)?
A: Because $\nabla\cdot\mathbf{B} = 0$: the divergence-free magnetic field has the same flux through any two surfaces sharing the same boundary. Any discrepancy would correspond to "magnetic charge" inside the closed volume between them, which doesn't exist. This is why we speak of "flux through a loop" without specifying which surface.

## 9.3 Faraday's Law

Q: What does Faraday's law state?
A: The electromotive force around a closed loop equals the negative time rate of change of magnetic flux through the loop: $\mathcal{E} = -d\Phi_B/dt$. In differential form, $\nabla\times\mathbf{E} = -\partial\mathbf{B}/\partial t$ — a time-varying magnetic field is a source of rotational electric field. Unlike electrostatic $\mathbf{E}$, the induced electric field does not come from static charges and can have nonzero circulation.

C: Faraday's law: $\mathcal{E} = [-d\Phi_B/dt]$, or in differential form $\nabla\times\mathbf{E} = -\partial\mathbf{B}/\partial t$.

Q: Why can the induced electric field have a nonzero curl, even though the electrostatic $\mathbf{E}$ does not?
A: The "induced" electric field is a fundamentally different object than the electrostatic field. The electrostatic field comes from charges and has zero curl. The induced field comes from $\partial\mathbf{B}/\partial t$ and has nonzero curl. In general, the total $\mathbf{E}$ is the sum of both contributions and has a curl equal to $-\partial\mathbf{B}/\partial t$.

## 9.4 Lenz's Law

Q: What does Lenz's law state, and what does the minus sign in Faraday's law physically represent?
A: The induced current (and the associated induced field) opposes the change in flux that created it. If the flux through a loop is increasing, the induced current flows in a direction that creates a flux opposing the increase. The minus sign in $\mathcal{E} = -d\Phi_B/dt$ is the mathematical expression of Lenz's law — it's what enforces energy conservation.

C: Lenz's law: the induced current flows so as to [oppose the change] in magnetic flux that caused it.

Q: Why must Lenz's law hold in order for energy to be conserved?
A: If the induced current AIDED the flux change, it would amplify the original disturbance, which would in turn induce even larger currents, and so on — a runaway that extracts energy from nothing. Lenz's law saves energy conservation: inducing a current requires doing work against the magnetic force, and the energy comes from the source that drives the flux change.

## 9.5 Motional EMF

Q: Why does moving a conducting rod through a magnetic field generate an EMF, even with no time-varying external field?
A: The mobile charges in the rod feel a Lorentz force $q\mathbf{v}\times\mathbf{B}$ as the rod moves, pushing them along the rod. This force effectively acts like a battery: it drives charges around the circuit. The "motional EMF" is $\int(\mathbf{v}\times\mathbf{B})\cdot d\mathbf{l}$ along the moving conductor — different from but mathematically consistent with the induced-field interpretation.

C: Motional EMF across a rod of length $L$ moving with velocity $v$ perpendicular to $\mathbf{B}$: $\mathcal{E} = [BLv]$.

Q: Why do motional EMF and the flux-rule interpretation of Faraday's law give the same answer, even though they sound like different mechanisms?
A: They're the same law viewed from different reference frames. In the lab frame, a moving rod has Lorentz force on its charges. In the rod's frame, the magnetic field appears to change with time, and Faraday induction applies. Both calculations give the same answer because $\Phi_B$ through the circuit changes at the same rate regardless of whose frame you use.

## 9.6 Self-Inductance

C: [Self-inductance] $L$ of a circuit is the proportionality constant between the magnetic flux through the circuit and the current producing it: $\Phi_B = LI$.

Q: Why does a current change in a circuit generate an EMF that opposes the change, via its own self-inductance?
A: When $I$ changes, the flux $\Phi = LI$ changes in proportion. Faraday's law gives $\mathcal{E} = -L\,dI/dt$ — a "back-EMF" that opposes the change in current by Lenz's law. The coefficient $L$ depends only on the geometry of the circuit. This is why inductors resist changes in current the way capacitors resist changes in voltage.

C: Back-EMF of a self-inductor: $\mathcal{E} = [-L\,dI/dt]$, where $L$ is the self-inductance.

Q: What is the self-inductance of a long ideal solenoid of length $\ell$ with $N$ turns and cross-sectional area $A$?
A: $L = \mu_0 N^2 A/\ell$. The field inside is $\mu_0 n I$ with $n = N/\ell$; the flux per turn is $BA = \mu_0 NIA/\ell$; total flux linkage is $N$ times that, giving $\Phi = \mu_0 N^2 I A/\ell = LI$. Inductance grows with the SQUARE of the number of turns — each turn contributes to both producing the field AND intercepting it.

C: Self-inductance of a long ideal solenoid: $L = [\mu_0 N^2 A/\ell]$, with $N$ turns, area $A$, length $\ell$.

## 9.7 Mutual Inductance

Q: What is mutual inductance between two circuits?
A: A coefficient $M_{12}$ relating the flux through circuit 1 to the current in circuit 2: $\Phi_1 = M_{12} I_2$. By Faraday's law, this means a changing current in circuit 2 induces an EMF $-M_{12}\,dI_2/dt$ in circuit 1. Remarkably, $M_{12} = M_{21}$ — a symmetry derived from the structure of Ampère's law.

C: Mutual inductance symmetry: $M_{12} = [M_{21}]$ — the flux in circuit 1 per unit current in circuit 2 equals the flux in circuit 2 per unit current in circuit 1.

Q: Why is the equality $M_{12} = M_{21}$ surprising at first, and why is it actually a consequence of energy conservation?
A: The two coefficients involve completely different integrals (fluxes through different loops from different currents), so nothing obvious guarantees they agree. Equality follows because both can be written as $\oint\oint d\mathbf{l}_1\cdot d\mathbf{l}_2/|\mathbf{r}_1 - \mathbf{r}_2|$ (Neumann formula), which is manifestly symmetric. Physically, it also follows from requiring that the energy stored be a well-defined state function independent of charging order.

## 9.8 Energy Stored in an Inductor

Q: Why is the energy stored in an inductor $U = \frac{1}{2}LI^2$?
A: Establishing a current $I$ against the back-EMF requires work. At intermediate current $i$, the back-EMF is $L\,di/dt$, and the power delivered is $iL\,di/dt$. Integrating from 0 to $I$ gives $\frac{1}{2}LI^2$. Like capacitor energy $\frac{1}{2}CV^2$, the $\frac{1}{2}$ comes from averaging over the charging process.

C: Energy stored in an inductor: $U = [\tfrac{1}{2}LI^2]$, with the factor $\frac{1}{2}$ reflecting integration over the charging process.

Q: Why can the energy stored in a magnetic field be written as $U = \frac{1}{2\mu_0}\int B^2\,d^3r$, parallel to the electrostatic expression?
A: Starting from $U = \frac{1}{2}LI^2$ for an inductor, expressing $L$ as a flux/current ratio, and using $\oint\mathbf{B}\cdot d\mathbf{l} = \mu_0 I$, one can rewrite the energy as an integral over field energy density $u_B = B^2/(2\mu_0)$. The magnetic field carries energy in the same way the electric field does — this becomes crucial for electromagnetic waves.

C: Magnetic energy density in vacuum: $u_B = [B^2/(2\mu_0)]$, analogous to the electric energy density $u_E = \varepsilon_0 E^2/2$.

## 9.9 LR Circuit

Q: Why does connecting an inductor $L$ in series with a resistor $R$ and a battery $\mathcal{E}$ produce a current that rises exponentially rather than instantaneously?
A: Kirchhoff's loop rule with a back-EMF gives $\mathcal{E} = IR + L\,dI/dt$. Solving this first-order ODE with initial condition $I(0) = 0$ yields $I(t) = (\mathcal{E}/R)(1 - e^{-t/\tau})$ with $\tau = L/R$. The inductor resists the sudden jump to the steady-state current $\mathcal{E}/R$, ramping up smoothly over a time $\sim\tau$.

C: Time constant of an LR circuit: $\tau = [L/R]$, setting the exponential approach to steady-state current.

Q: What happens to the current when the battery in an LR circuit is suddenly replaced by a short?
A: The inductor's stored energy $\frac{1}{2}LI^2$ must go somewhere. It continues to drive current through the resistor as the field collapses. The current decays exponentially: $I(t) = I_0\,e^{-t/\tau}$ with the same $\tau = L/R$. All the stored magnetic energy is eventually dissipated as heat in the resistor.

## 9.9a Pattern Recognition: Induction Problems

Q: A problem describes a fixed loop in a time-varying $\mathbf{B}$. What technique?
A: Faraday's law: $\mathcal{E} = -d\Phi/dt$ with $\Phi = BA$ — only $B$ changes.

Q: A problem describes a moving conductor in a static $\mathbf{B}$. What technique?
A: Motional EMF: $\mathcal{E} = \int (\mathbf{v}\times\mathbf{B})\cdot d\mathbf{l}$, or equivalently $-d\Phi/dt$ with $\Phi$ changing through area.

Q: A problem mentions current in an LR circuit "after switch closed." What technique?
A: $I(t) = (\mathcal{E}/R)(1 - e^{-t/\tau})$ with $\tau = L/R$.

Q: A problem says "find direction of induced current" without numbers. What technique?
A: Lenz's law: induced current opposes the change in flux. Sketch flux direction, ask "is it growing or shrinking?", pick current direction that fights it.

## 9.10 Betatron Oscillation — P:/S:

P: A circular loop of wire of radius $a$ and resistance $R$ is placed in a uniform time-dependent magnetic field $\mathbf{B}(t) = B_0\sin(\omega t)\,\hat{z}$, perpendicular to the loop. Find the induced EMF, the induced current, and the instantaneous power dissipated as a function of time. What is the time-averaged power dissipation?

S:
**IDENTIFY**: Direct Faraday's-law problem with a time-varying $\mathbf{B}$ and a fixed loop — the flux changes in time due to the field, not the geometry.

**PLAN**:
- Compute the flux through the loop as a function of time.
- Differentiate to get the EMF.
- Use Ohm's law to get the current.
- Compute instantaneous and averaged power.

**EXECUTE**:
1. Area vector: $\mathbf{A} = \pi a^2\,\hat{z}$.
2. Flux: $\Phi_B(t) = \mathbf{B}\cdot\mathbf{A} = B_0\pi a^2\sin(\omega t)$.
3. EMF: $\mathcal{E}(t) = -d\Phi_B/dt = -B_0\pi a^2\omega\cos(\omega t)$.
4. Current: $I(t) = \mathcal{E}/R = -\frac{B_0\pi a^2\omega}{R}\cos(\omega t)$.
5. Instantaneous power dissipated in the resistance: $P(t) = I^2(t)R = \frac{B_0^2\pi^2 a^4\omega^2}{R}\cos^2(\omega t)$.
6. Time-averaged power: $\langle P\rangle = \frac{B_0^2\pi^2 a^4\omega^2}{2R}$ (using $\langle\cos^2\rangle = 1/2$).

**EVALUATE**:
- The EMF and current are $90°$ out of phase with the applied field, because differentiation of a sinusoid gives a cosine.
- The induced current is largest when the field is passing through zero (fastest rate of change) and zero when the field is at its peak.
- The average power scales as $\omega^2$: faster-changing fields drive larger currents and dissipate more energy, even with the same amplitude $B_0$.
- Limit $\omega \to 0$ (quasi-static field): average power $\to 0$, as expected — no changing flux, no induced current.
- The dissipated energy comes from the external agent driving the magnetic field, not from the loop itself. Lenz's law ensures the induced current's magnetic moment opposes the field change, so work must be done against it.
- Practical realization: this is the working principle of an AC power meter, an induction cooktop, and the eddy-current brake on a roller coaster.
