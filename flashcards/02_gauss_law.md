+++
order = 2
subject = "physics"
tags = ["electromagnetism", "gauss-law", "flux", "divergence", "symmetry"]
+++

# Electromagnetism — Gauss's Law

## 2.1 Electric Flux

Q: What is electric flux through a surface, and why is it the natural quantity for formulating Gauss's law?
A: Electric flux $\Phi_E$ through a surface $S$ is the surface integral of the electric field: $\Phi_E = \int_S \mathbf{E}\cdot d\mathbf{A}$. It counts the net "flow" of field lines through the surface. Flux is natural because it captures the geometric content of the inverse-square law — field lines from a point charge give the same flux through any enclosing surface, regardless of shape.

C: Electric flux through a surface: $\Phi_E = [\int_S \mathbf{E}\cdot d\mathbf{A}]$, where $d\mathbf{A}$ is the outward-pointing area element.

Q: Why does the flux from a point charge through any closed surface enclosing it equal $q/\varepsilon_0$, independent of the shape of the surface?
A: The field lines from a point charge fan out radially, and the flux through a sphere centered on the charge is easily computed: $(q/(4\pi\varepsilon_0 r^2))(4\pi r^2) = q/\varepsilon_0$. For a non-spherical surface, the $r^2$ area factor and the $1/r^2$ field factor still cancel — the total count of field lines crossing out is the same, and only the enclosed charge matters.

## 2.2 Gauss's Law in Integral Form

C: Gauss's law (integral form): $\oint_S \mathbf{E}\cdot d\mathbf{A} = [Q_{\text{enc}}/\varepsilon_0]$, where $Q_{\text{enc}}$ is the total charge enclosed by the closed surface $S$.

Q: Why does Gauss's law depend only on enclosed charge and not on external charges, even though external charges produce fields at the surface?
A: External charges contribute field lines that enter and exit the closed surface — they add zero to the net flux. Only field lines that terminate inside (on enclosed charges) contribute a net flux. The external contribution is irrelevant because every line that goes in also comes out.

Q: Why is Gauss's law equivalent to Coulomb's law for point charges, but more general for continuous distributions?
A: Coulomb's law gives $\mathbf{E}$ for a single point charge, and superposition extends it to any distribution. Gauss's law packages the same content in a coordinate-free statement about flux. It is more general because it applies to any region and any distribution without needing to carry out the superposition integral explicitly — and it reveals the divergence structure of the field directly.

## 2.3 Gauss's Law in Differential Form

C: Gauss's law (differential form): $\nabla\cdot\mathbf{E} = [\rho/\varepsilon_0]$, where $\rho$ is the local charge density.

Q: Why does applying the divergence theorem to $\oint_S \mathbf{E}\cdot d\mathbf{A} = Q_{\text{enc}}/\varepsilon_0$ yield the differential form?
A: The divergence theorem replaces the surface integral with a volume integral: $\oint_S\mathbf{E}\cdot d\mathbf{A} = \int_V \nabla\cdot\mathbf{E}\,dV$. And $Q_{\text{enc}} = \int_V \rho\,dV$. Equating the integrands (because the volume is arbitrary) gives $\nabla\cdot\mathbf{E} = \rho/\varepsilon_0$. The differential form holds point by point.

Q: What does the statement "$\nabla\cdot\mathbf{E} = \rho/\varepsilon_0$" say physically about the structure of the electric field?
A: The divergence at a point measures how much field is "flowing out" of that point. Where positive charge sits ($\rho > 0$), the field has a positive divergence — field lines are born there. Where negative charge sits, field lines die. In empty space, $\rho = 0$ and the field is divergence-free — no field lines created or destroyed.

## 2.3a Reverse-Direction Cards

Q: Given the equation $\nabla\cdot\mathbf{E} = \rho/\varepsilon_0$, what does it physically express?
A: Electric field lines originate at positive charge ($\rho > 0$) and terminate at negative charge ($\rho < 0$); empty space is divergence-free.

Q: Given the equation $\oint_S \mathbf{E}\cdot d\mathbf{A} = Q_{\text{enc}}/\varepsilon_0$, what is its name and what does it state?
A: Gauss's law (integral form) — net electric flux through any closed surface is proportional to the enclosed charge.

Q: When you see the constant $1/\varepsilon_0$ on the right-hand side of a field equation, what does it indicate?
A: A SI-unit-system relation between electric quantities (flux, divergence) and charge sources.

## 2.4 Using Symmetry with Gauss's Law

Q: Why is Gauss's law a powerful calculational tool only when a symmetry picks out the direction of $\mathbf{E}$?
A: Gauss's law gives a single scalar equation (total flux = total enclosed charge). It cannot by itself determine three components of a vector field. But if symmetry forces $\mathbf{E}$ to be, say, radially outward with magnitude depending only on $r$, then the flux integral collapses to $E \times \text{(surface area)}$, and Gauss's law becomes an algebraic equation for $E(r)$.

C: Gauss's law lets you determine $\mathbf{E}$ algebraically whenever a symmetry ([spherical, cylindrical, or planar]) fixes the direction and reduces the field to a scalar function of a [single coordinate].

## 2.5 Field of a Spherically Symmetric Charge

Q: What is the electric field outside a spherically symmetric charge distribution of total charge $Q$?
A: $\mathbf{E} = \frac{1}{4\pi\varepsilon_0}\frac{Q}{r^2}\hat{r}$ — identical to the field of a point charge at the center. Symmetry forces $\mathbf{E}$ to be radial and depend only on $r$, and Gauss's law on a Gaussian sphere of radius $r$ gives $E \cdot 4\pi r^2 = Q/\varepsilon_0$.

C: Outside a spherically symmetric charge distribution, the electric field is [indistinguishable] from the field of a point charge of the same total charge located at the [center].

Q: Why is the electric field inside a uniformly charged insulating ball proportional to $r$, not $1/r^2$?
A: At radius $r < R$ inside the ball, a Gaussian sphere encloses only the charge within $r$: $Q_{\text{enc}} = Q(r/R)^3$. Gauss's law gives $E \cdot 4\pi r^2 = Q r^3/(R^3\varepsilon_0)$, so $E = Qr/(4\pi\varepsilon_0 R^3)$. The field grows linearly from zero at the center to its surface value at $r = R$.

## 2.6 Field of an Infinite Line

Q: Use Gauss's law to find the field at distance $s$ from an infinite line of charge with linear density $\lambda$.
A: Pick a Gaussian cylinder of radius $s$ and length $L$ coaxial with the line. Symmetry: $\mathbf{E}$ is radial and depends only on $s$. Flux through the curved surface is $E\cdot 2\pi s L$; through the ends, it is zero (field is parallel to the end caps). Enclosed charge: $\lambda L$. Result: $E = \lambda/(2\pi\varepsilon_0 s)$.

C: The electric field at perpendicular distance $s$ from an infinite line charge: $\mathbf{E} = [\lambda/(2\pi\varepsilon_0 s)]\,\hat{s}$.

## 2.7 Field of an Infinite Plane

Q: What is the electric field from an infinite plane of surface charge density $\sigma$?
A: $\mathbf{E} = \sigma/(2\varepsilon_0)\,\hat{n}$ on each side, pointing away from the plane (for positive $\sigma$). It is independent of distance — the field does not fall off with distance from an infinite plane, because the added charge at larger radii exactly compensates for the geometric spreading.

C: The field of an infinite plane of uniform surface charge is $E = \lbrack \sigma/(2\varepsilon_0)\rbrack $, [independent of distance] from the plane.

Q: Why does the field of an infinite plane not fall off with distance, unlike the field of a point charge?
A: For a point charge, flux spreads over a sphere of area $4\pi r^2$. For an infinite plane, the "cross-section" available for flux is fixed (the two parallel planes above and below), so spreading doesn't dilute the field. Mathematically, the infinite plane is the $L \to \infty$ limit where the geometry no longer spreads.

## 2.8 Field Discontinuity at a Surface Charge

Q: Why does the electric field jump by $\sigma/\varepsilon_0$ across a surface carrying charge density $\sigma$?
A: Applying Gauss's law to a tiny pillbox straddling the surface: the flux through the top and bottom faces differs by $(E_{\text{above}} - E_{\text{below}})\cdot A$, and the enclosed charge is $\sigma A$. So the normal component of the field jumps by exactly $\sigma/\varepsilon_0$. The tangential component, by contrast, is continuous (shown from the curl of $\mathbf{E}$).

C: Across a surface with charge density $\sigma$, the [normal component] of $\mathbf{E}$ jumps by $\sigma/\varepsilon_0$, while the [tangential component] is continuous.

## 2.9 Inside a Conductor (Preview)

Q: Why is the electric field inside the bulk of a conductor in electrostatic equilibrium exactly zero?
A: If $\mathbf{E}$ were nonzero inside a conductor, the free charges would feel a force and move — violating the assumption of electrostatic equilibrium. Charges redistribute themselves until they cancel any interior field, which happens when excess charge lies only on the surface and arranges itself to shield the interior.

C: In electrostatic equilibrium, the electric field inside a conductor is [zero], and any excess charge resides on the [surface].

## 2.9a Pattern Recognition: When to Use Gauss's Law

Q: A problem describes a spherically symmetric charge distribution and asks for $\mathbf{E}$. What technique?
A: Gauss's law with a spherical Gaussian surface centered on the symmetry point.

Q: A problem describes an infinite line/cylinder of charge. What technique?
A: Gauss's law with a coaxial cylindrical Gaussian surface (flux only through the curved side).

Q: A problem describes an infinite plane or slab of charge. What technique?
A: Gauss's law with a pillbox straddling the plane (flux only through the two faces).

Q: Why is Gauss's law not a useful tool for a finite, asymmetric charge distribution?
A: It gives only one scalar equation; without symmetry it cannot solve for $\mathbf{E}$. Use Coulomb's law / the superposition integral instead.

## 2.10 Field Outside a Charged Sphere — P:/S:

P: A solid insulating sphere of radius $R$ carries a total charge $Q$ distributed uniformly through its volume. Using Gauss's law, find the electric field at every point in space (inside and outside), and show that the two expressions match at the surface.

S:
**IDENTIFY**: Spherically symmetric distribution — Gauss's law on spherical Gaussian surfaces is the standard tool.

**PLAN**:
- Set up a Gaussian sphere of radius $r$, both for $r > R$ and $r < R$.
- Use symmetry to pull $E$ out of the flux integral.
- Compute enclosed charge as a fraction of total, for the interior case.
- Equate flux to $Q_{\text{enc}}/\varepsilon_0$ and solve for $E(r)$.
- Verify continuity at $r = R$.

**EXECUTE**:
1. Symmetry: $\mathbf{E}(\mathbf{r}) = E(r)\,\hat{r}$. Flux through a sphere of radius $r$: $\Phi = 4\pi r^2 E(r)$.
2. **Exterior, $r > R$**: entire charge enclosed, $Q_{\text{enc}} = Q$.
$$4\pi r^2 E = Q/\varepsilon_0 \Rightarrow E_{\text{ext}}(r) = \frac{Q}{4\pi\varepsilon_0 r^2}.$$
3. **Interior, $r < R$**: uniform density $\rho = Q/(\frac{4}{3}\pi R^3)$. Enclosed charge in a sphere of radius $r$:
$$Q_{\text{enc}} = \rho\cdot\frac{4}{3}\pi r^3 = Q\left(\frac{r}{R}\right)^3.$$
4. Gauss's law inside: $4\pi r^2 E = Q r^3/(R^3\varepsilon_0)$.
$$E_{\text{int}}(r) = \frac{Q r}{4\pi\varepsilon_0 R^3}.$$
5. **Continuity check at $r = R$**: $E_{\text{ext}}(R) = Q/(4\pi\varepsilon_0 R^2)$ and $E_{\text{int}}(R) = Q R/(4\pi\varepsilon_0 R^3) = Q/(4\pi\varepsilon_0 R^2)$ — identical.

**EVALUATE**:
- Interior field grows linearly from 0 at the center, exterior field decays as $1/r^2$ — the two smoothly join at the surface with no discontinuity, as expected because volume charge has no surface layer.
- Limits: $r = 0$ gives $E = 0$ (symmetric center feels zero net pull). $r \to \infty$ gives $E \to 0$ (isolated system).
- The field reaches its MAXIMUM at the surface $r = R$, where $E_{\max} = Q/(4\pi\varepsilon_0 R^2)$.
- Same calculation done directly from Coulomb's law would require a nested triple integral — this is the power of symmetry + Gauss.
- Gravity has the identical mathematical structure (inverse square, superposition). The same result gives the gravitational field of a uniform-density planet: linear inside, $1/r^2$ outside — hence free-fall through a uniform Earth would be simple harmonic motion.
