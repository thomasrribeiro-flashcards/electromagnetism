+++
order = 5
tags = ["electromagnetism", "dielectrics", "polarization", "displacement-field", "bound-charge"]
+++

# Electromagnetism — Dielectrics

## 5.1 What a Dielectric Is

C: A [dielectric] is an insulating material in which charges cannot move freely through the bulk but can shift slightly within atoms or molecules in response to an applied electric field.

Q: Why does a dielectric respond to an external field even though its charges cannot flow freely?
A: At the atomic level, each atom has a positive nucleus and a cloud of electrons. An external field pushes these in opposite directions, slightly displacing the electron cloud relative to the nucleus and creating an atomic-scale dipole. Polar molecules (like water) additionally rotate to align their permanent dipole moments with the field. No bulk current flows, but the internal charge distribution changes.

## 5.2 Polarization

C: The [polarization] $\mathbf{P}$ of a dielectric is the dipole moment per unit volume.

Q: Why is polarization a useful macroscopic description of a medium containing vastly more atomic dipoles than we could track individually?
A: At length scales much larger than an atom, the detailed arrangement of atomic dipoles averages out. What matters macroscopically is the LOCAL average dipole density $\mathbf{P}$, which is a smooth vector field that varies over laboratory length scales. This is the same philosophy as treating mass density $\rho$ instead of individual atomic masses.

C: For a linear dielectric, the polarization is proportional to the local field: $\mathbf{P} = [\varepsilon_0\chi_e\mathbf{E}]$, where $\chi_e$ is the [electric susceptibility] of the material.

## 5.3 Bound Charges

Q: Why does a polarized dielectric develop surface and volume "bound" charge densities even though no free charges have entered or left the material?
A: At a surface where $\mathbf{P}$ terminates, the positive ends of atomic dipoles stick out on one face and the negative ends on the opposite face, creating surface charge densities $\sigma_b = \mathbf{P}\cdot\hat{n}$. In the bulk, if $\mathbf{P}$ is non-uniform, neighboring dipoles don't fully cancel — giving a volume bound density $\rho_b = -\nabla\cdot\mathbf{P}$. These are real charges (physically present in the material), but they are constrained: unlike free charges, they cannot flow.

C: Bound surface charge density: $\sigma_b = [\mathbf{P}\cdot\hat{n}]$, with $\hat{n}$ the outward normal at the dielectric surface.

C: Bound volume charge density: $\rho_b = [-\nabla\cdot\mathbf{P}]$, nonzero only when the polarization varies in space.

Q: Why is the minus sign in $\rho_b = -\nabla\cdot\mathbf{P}$ physically necessary?
A: If polarization "flows out" of a region ($\nabla\cdot\mathbf{P} > 0$), it is pointing away from that region, and the positive ends of the dipoles leave while the negative ends remain — so the region is LEFT with negative charge. Outgoing polarization corresponds to incoming negative bound charge, hence the minus sign.

## 5.4 The Displacement Field

C: The electric [displacement field] is defined by $\mathbf{D} = \varepsilon_0\mathbf{E} + \mathbf{P}$.

Q: Why is the displacement field a more convenient object than $\mathbf{E}$ inside a dielectric?
A: Gauss's law for $\mathbf{D}$ involves only the FREE charge density: $\nabla\cdot\mathbf{D} = \rho_f$. It ignores the bound charges — which are implicitly accounted for in $\mathbf{P}$. For problems where only the free charges are known (e.g., a capacitor with a dielectric slab), the $\mathbf{D}$-field version of Gauss's law can be solved directly without first computing the bound charges.

C: Gauss's law for the displacement field: $\nabla\cdot\mathbf{D} = [\rho_f]$, where $\rho_f$ is the [free charge density] only.

Q: Why is $\mathbf{D}$ sometimes said to be "a bookkeeping device" rather than a fundamental field?
A: Because the fundamental Maxwell-equations quantity is $\mathbf{E}$ — it is what a test charge feels. The displacement field $\mathbf{D}$ is a combination $\varepsilon_0\mathbf{E} + \mathbf{P}$ that happens to satisfy a simpler form of Gauss's law by absorbing the bound charges. It is extremely useful but carries no additional physical content beyond $\mathbf{E}$ and $\mathbf{P}$.

## 5.5 Linear Dielectrics and Permittivity

Q: What characterizes a linear dielectric, and how does $\mathbf{D}$ simplify in that case?
A: In a linear dielectric, $\mathbf{P} = \varepsilon_0\chi_e\mathbf{E}$, so $\mathbf{D} = \varepsilon_0(1 + \chi_e)\mathbf{E} = \varepsilon\mathbf{E}$, where $\varepsilon = \varepsilon_0(1 + \chi_e)$ is the PERMITTIVITY. The ratio $\varepsilon_r = \varepsilon/\varepsilon_0 = 1 + \chi_e$ is the dimensionless relative permittivity (dielectric constant). Inside a linear dielectric, $\mathbf{D}$ is simply a scalar multiple of $\mathbf{E}$.

C: In a linear dielectric: $\mathbf{D} = [\varepsilon\mathbf{E}]$, where $\varepsilon = \varepsilon_0(1 + \chi_e)$ is the [permittivity] of the medium.

C: The dimensionless [relative permittivity] (dielectric constant) is $\varepsilon_r = \varepsilon/\varepsilon_0$, equal to $1 + \chi_e$.

Q: Why does a dielectric with $\varepsilon_r > 1$ reduce the electric field of a given set of free charges compared to vacuum?
A: The dielectric's polarization produces bound charges whose field opposes the field of the free charges. The net interior field is therefore smaller than it would be in vacuum. Quantitatively, $\mathbf{E}_{\text{inside}} = \mathbf{E}_{\text{vacuum}}/\varepsilon_r$ for simple geometries where the dielectric fills the relevant region. The reduction factor $\varepsilon_r$ is why dielectrics increase capacitance.

## 5.6 Capacitance with a Dielectric

Q: Why does filling a capacitor with a linear dielectric of relative permittivity $\varepsilon_r$ multiply its capacitance by $\varepsilon_r$?
A: At fixed free charge $Q$, the dielectric's bound charges partially neutralize the field, reducing $E$ and hence the voltage $V = Ed$ by a factor $\varepsilon_r$. Since $C = Q/V$, the capacitance INCREASES by the same factor $\varepsilon_r$. Physically, the dielectric lets you store more charge at a given voltage before the field is strong enough to cause breakdown.

C: Inserting a linear dielectric with relative permittivity $\varepsilon_r$ into a capacitor multiplies its capacitance by $[\varepsilon_r]$.

Q: Why does a dielectric get PULLED INTO the gap of a charged capacitor, even though no external force is applied?
A: The field stores energy, and pulling the dielectric in reduces the energy at fixed $Q$ (or increases it at fixed $V$, but the battery does the extra work). In either case, the energy-minimization principle at fixed boundary condition favors the configuration with the dielectric inserted, so the system exerts a force that draws the slab inward. At the microscopic level, the fringing field at the capacitor edge polarizes the slab and attracts it.

## 5.7 Boundary Conditions at Dielectric Interfaces

Q: Why is the normal component of $\mathbf{D}$ continuous across a boundary between two dielectrics (in the absence of free surface charge)?
A: Applying Gauss's law for $\mathbf{D}$ to a pillbox straddling the boundary: the enclosed free charge is zero (no free surface charge), so the flux of $\mathbf{D}$ in equals the flux out — meaning the normal component is continuous. If free charge sits on the boundary, $D_{\perp}$ jumps by that amount.

C: At a dielectric interface with no free surface charge, the [normal component of $\mathbf{D}$] is continuous; if free surface charge $\sigma_f$ is present, $D_{\perp}$ jumps by $\sigma_f$.

Q: Why is the tangential component of $\mathbf{E}$ continuous across any interface, regardless of whether a surface charge is present?
A: Because $\nabla\times\mathbf{E} = 0$ in electrostatics, $\oint\mathbf{E}\cdot d\mathbf{l} = 0$ around any loop. Taking a tiny rectangular loop straddling the surface, the two long sides give tangential-component contributions; shrinking the loop to zero width makes the short sides negligible, so the tangential components on either side must be equal.

C: At any dielectric interface, the [tangential component of $\mathbf{E}$] is continuous — a consequence of $\nabla\times\mathbf{E} = 0$.

## 5.8 Energy in a Dielectric

Q: Why does the energy density inside a linear dielectric take the form $u = \frac{1}{2}\mathbf{D}\cdot\mathbf{E} = \frac{1}{2}\varepsilon E^2$, rather than the vacuum expression $\frac{1}{2}\varepsilon_0 E^2$?
A: The $\varepsilon_0$ gets replaced by $\varepsilon$ because the dielectric polarization stores additional energy — assembling the free charges requires working against both the vacuum field and the bound-charge field of the dielectric. The extra "polarization energy" is exactly what the replacement $\varepsilon_0 \to \varepsilon$ captures.

C: The electrostatic energy density inside a linear dielectric is $u = [\tfrac{1}{2}\mathbf{D}\cdot\mathbf{E}]$, reducing to $u = \tfrac{1}{2}\varepsilon E^2$ in a linear medium.

## 5.9 Polarization Inside Uniform Dielectric Sphere — P:/S:

P: A uniform linear dielectric sphere of radius $R$ and relative permittivity $\varepsilon_r$ is placed in an external uniform electric field $\mathbf{E}_0 = E_0\,\hat{z}$ (very far away from the sphere). Find the polarization $\mathbf{P}$ inside the sphere, assuming the classic result that the interior field becomes $\mathbf{E}_{\text{in}} = 3E_0/(\varepsilon_r + 2)\,\hat{z}$ (which you may quote from the Legendre-polynomial solution of Laplace's equation).

S:
**IDENTIFY**: Given the interior field, read off $\mathbf{P}$ from the linear constitutive relation and show it is uniform — a central result for spherical dielectric bodies.

**PLAN**:
- Start from $\mathbf{P} = \varepsilon_0\chi_e\mathbf{E}_{\text{in}}$, where $\chi_e = \varepsilon_r - 1$.
- Substitute the interior field from the problem statement.
- Simplify and comment on the physical implications.

**EXECUTE**:
1. Susceptibility: $\chi_e = \varepsilon_r - 1$.
2. Interior field (given): $\mathbf{E}_{\text{in}} = \frac{3 E_0}{\varepsilon_r + 2}\,\hat{z}$.
3. Polarization: $\mathbf{P} = \varepsilon_0(\varepsilon_r - 1)\mathbf{E}_{\text{in}} = \varepsilon_0(\varepsilon_r - 1)\cdot\frac{3E_0}{\varepsilon_r + 2}\,\hat{z}$.
4. Simplify: $\mathbf{P} = \frac{3\varepsilon_0(\varepsilon_r - 1)}{\varepsilon_r + 2}E_0\,\hat{z}$.
5. This is UNIFORM inside the sphere (independent of position), pointing along the external field.

**EVALUATE**:
- The polarization is constant throughout the sphere. This matches the key fact that a uniformly polarized sphere produces a uniform interior field $-\mathbf{P}/(3\varepsilon_0)$ — the consistent self-solution.
- Limit $\varepsilon_r \to 1$ (no dielectric): $\mathbf{P} \to 0$. ✓
- Limit $\varepsilon_r \to \infty$ (conductor limit): $\mathbf{P} \to 3\varepsilon_0 E_0\hat{z}$, finite. The interior field goes to zero, consistent with conductor behavior.
- The surface bound charge is $\sigma_b = \mathbf{P}\cdot\hat{n} = P\cos\theta$, a standard $\cos\theta$ distribution that produces a pure dipole field outside the sphere.
- This "Clausius–Mossotti-like" structure appears in the theory of the index of refraction: a dilute collection of polarizable spheres has relative permittivity such that $(\varepsilon_r - 1)/(\varepsilon_r + 2) \propto$ number density, giving the Clausius–Mossotti relation.
- Practically, this result underlies capacitor-filling design, the dielectric constant of water ($\varepsilon_r \approx 80$), and the scattering of light by droplets in clouds.
