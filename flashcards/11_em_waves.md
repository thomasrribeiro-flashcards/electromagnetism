+++
order = 11
tags = ["electromagnetism", "waves", "poynting", "polarization", "radiation"]
+++

# Electromagnetism — Electromagnetic Waves and Radiation

## 11.1 The Wave Equation from Maxwell's Equations

Q: Why do Maxwell's equations in vacuum (no charges or currents) imply that $\mathbf{E}$ and $\mathbf{B}$ each satisfy a wave equation?
A: Take the curl of Faraday's law: $\nabla\times(\nabla\times\mathbf{E}) = -\partial(\nabla\times\mathbf{B})/\partial t$. Substitute the Ampère–Maxwell law (without sources): $\nabla\times\mathbf{B} = \mu_0\varepsilon_0\partial\mathbf{E}/\partial t$. The vector identity $\nabla\times(\nabla\times\mathbf{E}) = \nabla(\nabla\cdot\mathbf{E}) - \nabla^2\mathbf{E}$ and $\nabla\cdot\mathbf{E} = 0$ in vacuum give $\nabla^2\mathbf{E} = \mu_0\varepsilon_0\partial^2\mathbf{E}/\partial t^2$ — the wave equation. A parallel calculation gives the same equation for $\mathbf{B}$.

C: Electromagnetic wave equation in vacuum: $\nabla^2\mathbf{E} = [\mu_0\varepsilon_0\,\partial^2\mathbf{E}/\partial t^2]$, with $\mathbf{B}$ satisfying the same equation.

Q: Why does the wave speed from the vacuum wave equation turn out to be $c = 1/\sqrt{\mu_0\varepsilon_0}$?
A: Comparing $\nabla^2\mathbf{E} = \mu_0\varepsilon_0\partial^2\mathbf{E}/\partial t^2$ to the general wave equation $\nabla^2\psi = (1/v^2)\partial^2\psi/\partial t^2$, we identify $v^2 = 1/(\mu_0\varepsilon_0)$. Plugging in the known vacuum values gives $c = 3\times 10^8$ m/s — the speed of light. Maxwell noticed this coincidence in 1862 and concluded that light is an electromagnetic wave.

C: The speed of light in vacuum is $c = [1/\sqrt{\mu_0\varepsilon_0}]$, a fundamental constant emerging from purely electromagnetic constants.

## 11.2 Plane Waves

C: A [plane wave] is a solution to the wave equation of the form $f(\mathbf{k}\cdot\mathbf{r} - \omega t)$ — a disturbance that depends only on the coordinate along a single direction $\mathbf{k}$.

Q: What is the general form of a monochromatic plane electromagnetic wave in vacuum?
A: $\mathbf{E}(\mathbf{r}, t) = \mathbf{E}_0\cos(\mathbf{k}\cdot\mathbf{r} - \omega t + \phi)$ with $|\mathbf{k}| = \omega/c$. The direction of $\mathbf{k}$ is the direction of propagation; $\omega$ is the angular frequency; $\mathbf{E}_0$ is the amplitude (polarization vector). An accompanying magnetic field is determined by the Maxwell equations.

Q: Why are electromagnetic plane waves TRANSVERSE, meaning $\mathbf{E}$ and $\mathbf{B}$ are perpendicular to the propagation direction?
A: The vacuum Maxwell equation $\nabla\cdot\mathbf{E} = 0$ applied to a plane wave gives $i\mathbf{k}\cdot\mathbf{E}_0 = 0$, i.e., $\mathbf{E}_0\perp\mathbf{k}$. The same argument for $\nabla\cdot\mathbf{B} = 0$ gives $\mathbf{B}_0\perp\mathbf{k}$. Both field amplitudes are confined to the plane perpendicular to propagation — there is no "longitudinal" component.

C: Electromagnetic plane waves are [transverse]: both $\mathbf{E}$ and $\mathbf{B}$ are perpendicular to the propagation direction $\mathbf{k}$.

## 11.3 Relation Between E and B in a Plane Wave

Q: Why are $\mathbf{E}$ and $\mathbf{B}$ in a plane wave perpendicular to each other, in phase, and related by $B_0 = E_0/c$?
A: Substituting a plane-wave ansatz into Faraday's law gives $\mathbf{k}\times\mathbf{E}_0 = \omega\mathbf{B}_0$, which forces $\mathbf{B}_0$ to be perpendicular to both $\mathbf{k}$ and $\mathbf{E}_0$, with magnitude $B_0 = kE_0/\omega = E_0/c$. Both fields oscillate in phase (same sinusoidal function). The triple $(\mathbf{E}, \mathbf{B}, \mathbf{k})$ forms a right-handed orthogonal system.

C: In a plane electromagnetic wave in vacuum: $\mathbf{E}\perp\mathbf{B}\perp\mathbf{k}$, and the magnitudes obey $B = [E/c]$.

## 11.4 Energy in a Plane Wave

Q: Why do the electric and magnetic energy densities in a plane electromagnetic wave carry equal shares of the total energy?
A: The electric energy density is $u_E = \frac{\varepsilon_0}{2}E^2$, the magnetic is $u_B = B^2/(2\mu_0)$. Using $B = E/c$ and $c^2 = 1/(\mu_0\varepsilon_0)$: $u_B = E^2/(2\mu_0 c^2) = \varepsilon_0 E^2/2 = u_E$. The two are equal at every point and every instant — the total energy density is evenly split between the electric and magnetic field contributions.

C: In a plane EM wave, the electric and magnetic energy densities are equal: $u_E = [u_B] = \varepsilon_0 E^2/2$.

Q: What is the time-averaged Poynting vector for a monochromatic plane wave with peak electric-field amplitude $E_0$?
A: $\langle\mathbf{S}\rangle = (1/(2\mu_0 c))E_0^2\hat{k} = (c\varepsilon_0/2)E_0^2\hat{k}$. The magnitude is the INTENSITY of the wave, i.e., the time-averaged power per unit area. The factor of $1/2$ comes from averaging $\cos^2(\omega t)$ over a period.

C: Time-averaged intensity of a monochromatic plane wave: $I = \langle S\rangle = [c\varepsilon_0 E_0^2/2]$, where $E_0$ is the peak electric field amplitude.

## 11.5 Radiation Pressure

Q: Why does an EM wave hitting a surface exert a pressure equal to $I/c$ (absorbed) or $2I/c$ (perfectly reflected)?
A: The wave carries momentum density $g = S/c^2$, so its momentum flux is $S/c = I/c$ — this is the force per unit area (pressure) delivered to an absorber. For a mirror, the wave reverses direction, doubling the momentum transfer and therefore the pressure. The existence of radiation pressure was first demonstrated by Nichols and Hull in 1901.

C: Radiation pressure on a perfectly absorbing surface is $P = [I/c]$, and on a perfect reflector is $P = 2I/c$.

Q: Why is radiation pressure utterly negligible in everyday life but crucial in astrophysics?
A: $I/c$ is tiny because $c$ is huge: sunlight at Earth's orbit ($I \sim 1400$ W/m²) gives only $\sim 5\,\mu$Pa, dwarfed by mechanical forces. But in stars, the radiation field is enormous and the matter is hot and optically thick: radiation pressure balances gravity in the upper layers of massive stars, drives solar wind, and shapes the inside of nebulae. It also limits the brightness of stars via the Eddington limit.

## 11.6 Polarization

C: The [polarization] of an electromagnetic wave refers to the orientation (and its time behavior) of the electric field vector in the plane perpendicular to propagation.

Q: What distinguishes linear from circular polarization?
A: In linear polarization, $\mathbf{E}$ oscillates along a fixed direction perpendicular to $\mathbf{k}$. In circular polarization, $\mathbf{E}$ has equal-magnitude components along two perpendicular axes with a $90°$ phase difference — the tip of the $\mathbf{E}$ vector traces out a circle as the wave passes. Elliptical polarization is the general case.

Q: Why does superposing two linearly polarized waves with a phase difference of $\pi/2$ produce a circularly polarized wave?
A: If $\mathbf{E}_x = E_0\hat{x}\cos(kz - \omega t)$ and $\mathbf{E}_y = E_0\hat{y}\cos(kz - \omega t + \pi/2) = -E_0\hat{y}\sin(kz - \omega t)$, then as time progresses the total $\mathbf{E}$ vector rotates uniformly in the $xy$-plane with constant magnitude $E_0$. The rotation direction (clockwise or counterclockwise viewed from $+z$) determines right- or left-handed polarization.

## 11.7 Electromagnetic Spectrum

Q: What determines the "type" of electromagnetic wave (radio, visible, X-ray, etc.), and why is it misleading to think of them as different physical phenomena?
A: All electromagnetic waves are the same physical object — solutions to Maxwell's equations traveling at $c$ in vacuum. They differ only in frequency (and hence wavelength $\lambda = c/f$). Radio is $\sim 10^6$ Hz, visible light is $\sim 10^{14}$ Hz, X-rays are $\sim 10^{18}$ Hz. The interactions with matter change dramatically with frequency, but the fields themselves obey identical wave equations.

C: All electromagnetic radiation — from [radio waves] to [gamma rays] — differs only in frequency, not in the underlying physics.

## 11.8 Waves in Matter

Q: How does the EM wave equation change inside a linear medium with permittivity $\varepsilon$ and permeability $\mu$?
A: Replace $\varepsilon_0 \to \varepsilon$ and $\mu_0 \to \mu$. The wave speed becomes $v = 1/\sqrt{\mu\varepsilon} = c/n$, where $n = \sqrt{\mu\varepsilon/(\mu_0\varepsilon_0)}$ is the index of refraction. Most non-magnetic materials have $\mu \approx \mu_0$, so $n \approx \sqrt{\varepsilon_r}$. The wave is slower than in vacuum and its wavelength is shorter by a factor of $n$ at the same frequency.

C: In a linear medium, the speed of electromagnetic waves is $v = [c/n]$, where $n = \sqrt{\varepsilon_r\mu_r}$ is the [index of refraction].

Q: Why does the frequency of an electromagnetic wave stay constant when it crosses from vacuum into a denser medium, while its wavelength decreases?
A: The boundary condition requires continuity of the oscillating fields at the interface — the two sides must "wave in phase" at every moment. Phase matching across the boundary means the temporal oscillation (frequency) is the same on both sides, but the spatial variation (wavelength) adjusts to the new wave speed. $v = f\lambda$ with $f$ fixed gives $\lambda_{\text{med}} = \lambda_0/n$.

## 11.9 Dipole Radiation

Q: Why does an oscillating electric dipole radiate electromagnetic waves, while a static dipole does not?
A: A static dipole has fixed fields and stores energy locally without sending any away. An oscillating dipole has $\partial\mathbf{E}/\partial t \neq 0$, which produces a time-varying magnetic field via the Ampère–Maxwell law, which in turn produces a time-varying electric field via Faraday's law. This self-sustaining coupling lets the fields propagate outward as radiation, carrying energy to infinity.

Q: Why is the angular distribution of dipole radiation proportional to $\sin^2\theta$, peaking perpendicular to the dipole axis and vanishing along it?
A: The far-field radiation comes from the acceleration of the charges along the dipole axis. By relativistic kinematics, an accelerating charge radiates no energy along the direction of its acceleration (where $|\hat{r}\times\mathbf{a}| = 0$) and radiates most strongly perpendicular to the acceleration. For a sinusoidal dipole aligned with $\hat{z}$, the intensity pattern becomes $dP/d\Omega \propto \sin^2\theta$, where $\theta$ is the angle from the dipole axis.

C: Angular distribution of electric-dipole radiation: $dP/d\Omega \propto [\sin^2\theta]$, vanishing along the dipole axis and peaking in the equatorial plane.

Q: Why does the total radiated power of an oscillating dipole scale as $\omega^4$ (the Larmor–Rayleigh law)?
A: Each time derivative of the dipole moment pulls out a factor of $\omega$ from a sinusoidal oscillation, and the radiation field in the far zone is proportional to the second time derivative of the dipole moment. Squaring and time-averaging gives a factor $\omega^4$. This explains why the sky is blue: Rayleigh scattering of sunlight off atmospheric molecules scales as $\omega^4$, favoring short-wavelength blue light over red.

C: Total radiated power of an oscillating dipole scales as $P \propto [\omega^4]$ — the origin of the $\omega^4$ factor in Rayleigh scattering.

## 11.10 Energy Flux of a Plane Wave — P:/S:

P: A monochromatic plane electromagnetic wave in vacuum has peak electric field amplitude $E_0$ and propagates in the $+\hat{z}$ direction with angular frequency $\omega$. Find (a) the magnetic field amplitude, (b) the instantaneous Poynting vector, (c) the time-averaged intensity, and (d) the time-averaged momentum flux per unit area delivered to a perfect absorber.

S:
**IDENTIFY**: Standard plane-wave bookkeeping problem. Use the vacuum relations between $\mathbf{E}$, $\mathbf{B}$, and $\mathbf{S}$, then average over a period.

**PLAN**:
- Write $\mathbf{E}(z, t) = E_0\cos(kz - \omega t)\hat{x}$.
- Use $B = E/c$ and the right-hand rule to get $\mathbf{B}$.
- Compute $\mathbf{S} = (1/\mu_0)\mathbf{E}\times\mathbf{B}$ instantaneously.
- Average over a period ($\langle\cos^2\rangle = 1/2$).
- Convert intensity to momentum flux via $p = S/c$.

**EXECUTE**:
1. Electric field: $\mathbf{E}(z, t) = E_0\cos(kz - \omega t)\,\hat{x}$.
2. Magnetic field: $\mathbf{B} = (E_0/c)\cos(kz - \omega t)\,\hat{y}$ — perpendicular to $\mathbf{E}$, in phase, with magnitude $E_0/c$.
3. Instantaneous Poynting vector:
$$\mathbf{S}(z, t) = \frac{1}{\mu_0}\mathbf{E}\times\mathbf{B} = \frac{E_0^2}{\mu_0 c}\cos^2(kz - \omega t)\,\hat{z}.$$
4. Simplify with $1/(\mu_0 c) = c\varepsilon_0$:
$$\mathbf{S}(z, t) = c\varepsilon_0 E_0^2\cos^2(kz - \omega t)\,\hat{z}.$$
5. Time average: $\langle\cos^2\rangle = 1/2$, so
$$\langle\mathbf{S}\rangle = \frac{c\varepsilon_0 E_0^2}{2}\hat{z}.$$
6. Momentum flux per unit area on a perfect absorber: $P_{\text{rad}} = \langle S\rangle/c = \varepsilon_0 E_0^2/2$.

**EVALUATE**:
- Intensity direction $+\hat{z}$: the energy flows in the propagation direction, as expected.
- Factor-of-$\frac{1}{2}$ from time averaging is the standard "peak to RMS squared" conversion for a sinusoid.
- For a perfect REFLECTOR, the pressure is twice this: $2\varepsilon_0 E_0^2/2 = \varepsilon_0 E_0^2$, because the wave reverses direction and delivers momentum both on arrival and on departure.
- Units: $[\varepsilon_0 E_0^2] = (\text{F/m})(\text{V/m})^2 = \text{V·C/m}^3 = \text{J/m}^3$, which (divided by $c$) gives pressure = Pa. ✓
- Numerical scale: for sunlight at Earth's orbit, $I \approx 1400$ W/m² gives $E_0 \approx 1000$ V/m and radiation pressure $\approx 5\,\mu$Pa — small but measurable, and the working principle of solar sails.
- Connection to quantum mechanics: each photon of frequency $\omega$ carries energy $\hbar\omega$ and momentum $\hbar k = \hbar\omega/c$. The classical result $P = I/c$ is exactly what you get by multiplying the photon flux by the momentum per photon.
