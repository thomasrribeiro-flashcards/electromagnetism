+++
order = 6
subject = "physics"
tags = ["electromagnetism", "current", "ohms-law", "emf", "continuity"]
+++

# Electromagnetism — Currents and Resistance

## 6.1 Electric Current

C: Electric [current] $I$ is the rate at which charge crosses a given cross-section of a conductor: $I = dQ/dt$.

Q: Why does the direction of conventional current oppose the actual direction of electron flow in most circuits?
A: The convention was fixed before the discovery of the electron: Benjamin Franklin guessed that current carriers were positive, so "current flow" was defined as the direction a positive charge would move. Decades later, electrons turned out to be negative and carry the current in most metals — but the convention was too entrenched to change. Conventional current still points from $+$ to $-$ externally.

## 6.2 Current Density

C: The [current density] $\mathbf{J}$ is the current per unit cross-sectional area: $I = \int_S \mathbf{J}\cdot d\mathbf{A}$ through a surface $S$.

Q: Why is current density the natural local quantity, while current $I$ is a derived integral over a surface?
A: Current $I$ depends on the specific surface we integrate over. Current density $\mathbf{J}$ is a property of each point in space — it tells you how much charge per unit time per unit area is flowing through a little patch at that point. Local physical laws (like the continuity equation) are naturally stated in terms of $\mathbf{J}$, not $I$.

Q: How is current density related to the density and drift velocity of charge carriers?
A: $\mathbf{J} = n q \mathbf{v}_d$, where $n$ is the number density of carriers, $q$ is the charge per carrier, and $\mathbf{v}_d$ is the average drift velocity. Even in a copper wire carrying a large current, $\mathbf{v}_d$ is only millimeters per second — but the density $n$ of mobile electrons is so enormous that the product gives a macroscopic current.

C: Current density in terms of carriers: $\mathbf{J} = [n q \mathbf{v}_d]$, where $n$ is the carrier density and $\mathbf{v}_d$ is the average drift velocity.

## 6.3 The Continuity Equation

Q: What does the continuity equation $\partial\rho/\partial t + \nabla\cdot\mathbf{J} = 0$ express, and why must it hold?
A: It is the local statement of charge conservation. The first term is the rate at which charge density changes at a point; the second is the rate at which charge "flows out" of that point. Their sum vanishes because charge cannot be created or destroyed: if $\rho$ decreases, the difference must have flowed out, and vice versa.

C: Charge conservation in local form (the continuity equation): $\partial\rho/\partial t + \nabla\cdot\mathbf{J} = [0]$.

Q: Why does the continuity equation imply that in a steady state ($\partial\rho/\partial t = 0$), the current density is divergence-free?
A: Setting $\partial\rho/\partial t = 0$ gives $\nabla\cdot\mathbf{J} = 0$. Physically: in a steady state, whatever current flows into a tiny volume must flow back out, with no accumulation. This is Kirchhoff's current law at the level of a single point — the sum of currents at a node is zero.

## 6.4 Ohm's Law (Microscopic)

Q: What is the microscopic form of Ohm's law?
A: $\mathbf{J} = \sigma\mathbf{E}$, where $\sigma$ (here the conductivity, not surface charge) relates local current density to local electric field. The reciprocal $\rho = 1/\sigma$ is the resistivity. The law expresses a linear response: weak fields produce proportional currents, with a coefficient that depends on the material.

C: Microscopic Ohm's law: $\mathbf{J} = \lbrack \sigma\mathbf{E}\rbrack $, where $\sigma$ is the [conductivity] of the material.

Q: Why is Ohm's law a MATERIAL property rather than a fundamental law of nature?
A: Because it describes how electrons interact with a lattice: they accelerate in the field but scatter off defects and phonons, reaching a steady drift velocity proportional to $\mathbf{E}$. For weak fields and typical materials, this balance gives linearity — but it breaks down for strong fields (hot-electron effects) and fails entirely for superconductors, semiconductors, and plasmas. Maxwell's equations remain valid in all these cases.

## 6.5 Ohm's Law (Macroscopic)

Q: Why is the macroscopic form $V = IR$ a direct consequence of the microscopic $\mathbf{J} = \sigma\mathbf{E}$?
A: For a uniform wire of length $L$ and cross-section $A$, integrate $\mathbf{J} = \sigma\mathbf{E}$ along the wire: $I = JA$ and $V = EL$, giving $V = IL/(\sigma A) = IR$ with $R = L/(\sigma A)$. Geometry and material properties combine into a single scalar $R$ — the resistance.

C: Resistance of a uniform wire: $R = [L/(\sigma A)]$, where $L$ is the length, $A$ is the cross-sectional area, and $\sigma$ is the conductivity.

Q: Why is resistance EXTENSIVE in length but INVERSELY proportional to cross-section?
A: A longer wire gives electrons more lattice to scatter through, so more voltage is needed per unit current. A wider wire provides more parallel channels for current to flow, lowering resistance in direct proportion. These behaviors are entirely analogous to hydraulic resistance of a pipe.

## 6.6 Power Dissipation in a Resistor

Q: Why does a current-carrying resistor dissipate energy at rate $P = I^2 R = V^2/R = IV$?
A: The electric field does work on the charge carriers as they drift through the material: $P = \int \mathbf{J}\cdot\mathbf{E}\,dV$. Locally, $\mathbf{J}\cdot\mathbf{E} = \sigma E^2$ is the power density. Integrating over a uniform wire gives $I\cdot V$. In a resistor, this work ultimately goes into heat — the collisions of electrons with the lattice transfer energy from electrical to thermal form.

C: Power dissipated in a resistor (Joule heating): $P = [I^2 R] = V^2/R = IV$.

## 6.7 Electromotive Force

C: An [electromotive force] (EMF) $\mathcal{E}$ is the work done per unit charge by a non-electrostatic source (battery, generator) in driving charges around a circuit.

Q: Why is EMF not actually a "force" despite its name, and why is it measured in volts?
A: EMF is energy per unit charge supplied by a source — it has units of volts, not newtons. The name is historical and misleading. A better description: it's the "push" a source provides to move charges against the electric field that would otherwise equalize potentials, keeping a steady current flowing. Batteries convert chemical energy, generators convert mechanical energy.

Q: Why is the voltage across the terminals of a real battery less than its EMF when current is flowing?
A: Real batteries have internal resistance $r$: the current $I$ flowing through the internal path drops $Ir$ of potential inside the battery. Terminal voltage $V = \mathcal{E} - Ir$ is therefore less than $\mathcal{E}$ whenever $I > 0$. At open circuit ($I = 0$), the terminal voltage equals the EMF exactly.

C: Terminal voltage of a real battery: $V = \lbrack \mathcal{E} - Ir\rbrack $, where $r$ is the [internal resistance] and $I$ is the current drawn.

## 6.8 Kirchhoff's Laws

Q: What does Kirchhoff's current law (KCL) state, and why is it just the continuity equation in disguise?
A: KCL: the sum of currents entering any node in a circuit equals the sum leaving. It follows from the steady-state continuity equation $\nabla\cdot\mathbf{J} = 0$: if charge can't accumulate at a point, the inflow must equal the outflow. Integrating this over a tiny node volume gives KCL.

Q: What does Kirchhoff's voltage law (KVL) state, and why does it hold for circuits?
A: KVL: the sum of voltage drops around any closed loop is zero. It follows from $\nabla\times\mathbf{E} = 0$ (in electrostatic or quasi-static circuits): $\oint\mathbf{E}\cdot d\mathbf{l} = 0$. Stepping around a loop and adding up the potential changes recovers zero. For circuits with time-varying magnetic flux, KVL must be extended with Faraday's law.

C: Kirchhoff's laws: KCL is the [steady-state continuity equation] applied to nodes, and KVL is $\oint\mathbf{E}\cdot d\mathbf{l} = \lbrack 0\rbrack $ applied to loops.

## 6.9 Resistors in Series and Parallel

Q: Why do resistors in SERIES add directly and resistors in PARALLEL add inversely?
A: In series, the same current passes through each resistor, and the voltage drops add: $V = IR_1 + IR_2 = I(R_1 + R_2)$ — so resistances add. In parallel, the same voltage sits across both, and the currents add: $I = V/R_1 + V/R_2 = V(1/R_1 + 1/R_2)$ — so conductances (inverse resistances) add.

C: Resistors in series: $R_{\text{tot}} = [R_1 + R_2]$. Resistors in parallel: $1/R_{\text{tot}} = [1/R_1 + 1/R_2]$.

## 6.10 RC Circuit Discharge — P:/S:

P: A capacitor of capacitance $C$ is initially charged to voltage $V_0$ and then connected at $t = 0$ across a resistor $R$. Find the charge $Q(t)$ on the capacitor and the current $I(t)$ through the resistor as functions of time, and identify the characteristic time constant.

S:
**IDENTIFY**: First-order linear ODE problem. Use Kirchhoff's voltage law around the loop and the relation $I = -dQ/dt$ (with the sign chosen so that a discharging capacitor has positive current in the loop).

**PLAN**:
- Apply KVL around the loop: voltage across the capacitor equals voltage across the resistor.
- Relate $Q$ and $I$ via charge conservation: $I = -dQ/dt$.
- Solve the resulting first-order ODE.
- Extract the time constant from the exponent.

**EXECUTE**:
1. KVL: $V_C = V_R$, i.e., $Q/C = IR$.
2. Conservation: $I = -dQ/dt$ (capacitor losing charge drives positive loop current).
3. Substitute: $Q/C = -R\,dQ/dt$, i.e., $dQ/dt = -Q/(RC)$.
4. Solve: $Q(t) = Q_0 e^{-t/(RC)} = CV_0\,e^{-t/(RC)}$.
5. Current: $I(t) = -dQ/dt = (V_0/R)\,e^{-t/(RC)}$.
6. Time constant: $\tau = RC$.

**EVALUATE**:
- At $t = 0$: $Q = CV_0$ (initial charge) and $I = V_0/R$ (maximum current, limited only by the resistor). ✓
- At $t = \tau = RC$: $Q$ and $I$ have dropped to $1/e \approx 37\%$ of their initial values.
- At $t \gg \tau$: both $Q$ and $I$ decay exponentially to zero — the capacitor has fully discharged.
- Units: $[RC] = \text{ohm} \cdot \text{farad} = (\text{V/A})(\text{C/V}) = \text{C/A} = \text{s}$. ✓
- Energy conservation: initial energy $\frac{1}{2}CV_0^2$ is dissipated entirely in the resistor as heat. Integrating $P = I^2 R$ over $t$ from 0 to $\infty$: $\int_0^\infty (V_0^2/R)e^{-2t/RC}\,dt = V_0^2 RC/(2R) = \frac{1}{2}CV_0^2$. ✓
- Practical significance: $RC$ sets the response time of every first-order electrical filter; a slow oscilloscope probe has a large $RC$ and distorts fast signals, while a fast digital gate has a tiny $RC$ and can switch at GHz frequencies.
