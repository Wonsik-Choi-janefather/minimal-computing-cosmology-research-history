# Part III — Reality Renderer Architecture

# Opening words of Part 3

Part 3 fixes the intuition formed earlier as the minimum specification of WRRA and examines how that specification can be implemented in the language of existing physics.At the center is the renderer path independence paper published on August 27, 2026, v1.1, which repairs this with restorability and metric faithfulness, and v1.2, which deals with time uniformity stability of repeated rendering.

The point of this section is not to declare a particular five-dimensional model to be the ultimate reality of the universe.The 5-dimensional parent is one of the possible renderers, and the Einstein gravity is also a conditional low-energy branch selected under explicit additional assumptions.

For WRRA to survive, it must go beyond beautiful interpretation and show observational equivalence of different implementation paths, anomaly-free constraint closure, and prediction for uninput data.Part 3 records the currently closed structure and the boundaries of the next verification.

# Chapter 18 What does WRRA try to explain?

Wonsik Reality-Renderer Architecture, or WRRA, does not assume that any underlying source is exactly the same as the reality we observe.The source may have more degrees of freedom, continuums, and potential relationships, and the observable 3+1 dimensional reality is the result of their joint realization into one local, coherent form.

In this view, reality is not a copy of the source but a phenotype.Just as the same genetic information in biology appears as specific traits depending on the expression process and environment, physical sources also appear as objects with mass, charge, spin, and position after passing the renderer's rules and boundary conditions.The purpose of the analogy is not to forcefully translate biology into physics, but to separate the layers of implementation between the source and the observed results.

The minimum structure of WRRA is three layers: SOURCE, RENDERER, and PHENOTYPE.SOURCE provides possible degrees of freedom and potential states, RENDERER applies acceptance relations and locality, symmetry, transfer, and recording conditions, and PHENOTYPE is revealed as an observable physical reality.

*P = R(S; RELATION, BOUNDARY, θ)* (3.1)

RELATION and BOUNDARY are included in RENDERER.RELATION determines what can be combined and preserved, and BOUNDARY is the interface where the results interact with other systems and remain as recordable differences.The dimensional filter and common forwarder are candidate modules for the renderer and are not identical to the entire WRRA.

Therefore, WRRA does not require the ontology that ‘the universe is a computer simulation’.Without assuming an external computer or programmer, we can ask about a structure that is implemented as an observational reality with limited source possibilities.Minimum computation is an operating principle where the renderer avoids duplication and reuses common relationships.

What WRRA has currently frozen is a minimum specification, not a single final action.Candidate physical implementations are tested to ensure that they meet this specification, and if a particular 5D model or Bessel carrier fails, the entire architecture does not automatically collapse.Conversely, just because one candidate works does not mean that the entire WRRA can be proven.

*WRRA = {S, R, P;compatibility, locality, recordability}* (3.2)

## Related public research

**Wonsik Reality-Renderer Architecture v1.0** [<u>10.5281/zenodo.22122349</u>](https://doi.org/10.5281/zenodo.22122349)

# Chapter 19 Co-realized physical objects

Let's consider one electron.We can measure the mass of an electron in one experiment, its charge in another, and its spin in another.However, electrons in nature do not possess these properties separately as unrelated labels.All properties are jointly attributed to the same event and the same propagation history.

WRRA calls this joint attribution the joint phenotype.A physical object is not simply a list of eigenvalues ​​of mass operators, gauge expressions, Lorentz expressions, and local positions in one line.They must be compatible and persist under the same local observation algebra and the same translation operation.

*P_joint = (m, q, s, x) │ (A_local, T_a)* (3.3)

Stable particles can appear as poles on the real axis, and charged particles such as electrons can appear as infraparticle thresholds instead of strictly single particle poles due to soft photon clouds.Unstable particles are described analytically as extended resonance poles, and proton-like composites are realized as gauge-invariant composite states.The renderer must distinguish between these different spectral ownerships.

*stable pole ⊕ infraparticle threshold ⊕ resonance ⊕ composite* (3.4)

Without this distinction, errors arise such as misreading the resonance width while saying that mass has been created, equating the gauge-dependent field with a physical particle, or treating the mass of a composite as if it were a fundamental field parameter.WRRA's ledger first asks which spectral sector each observation belongs to.

Co-realization also includes location issues.If the charge and mass of an object are defined at different space-time locations, it cannot become a detectable particle.All properties must move and react together at the same translation history and local interaction point.

This is why a renderer is not just a classifier.The filter can decide whether to pass or not, but the renderer must bind the passed degrees of freedom into a single physical identity and preserve it over time.

## Related public research

**Wonsik Reality-Renderer Architecture v1.0** [<u>10.5281/zenodo.22122349</u>](https://doi.org/10.5281/zenodo.22122349)

# Chapter 20 Visible Interface and Hidden Continuum

WRRA v1.0 divides between visible reality and hidden sources with a self-adjoint block architecture.The visible sector is the interface we read as particles and fields, while the hidden sector may include broader continuums or degrees of freedom that have not yet been directly observed.

If we divide the entire Hamiltonian into blocks of visible space and hidden space, the effective dynamics of the visible sector are not the result of simply deleting the hidden sector.Through resolvent, the hidden part returns to self-energy and spectral density.This structure provides a standard way to preserve the self-involvement of the entire operator while preserving the effects of open systems.

*H = \[\[H_vis, V\], \[V†, H_hid\]\]* (3.5)

*G_vis(z) = \[z − H_vis − V(z−H_hid)⁻¹V†\]⁻¹* (3.6)

The important point is that it is not assumed that the hidden continuum is dark matter or another universe.It is the mathematical ownership of degrees of freedom outside the visible interface of the renderer implementation.Actual physical interpretations must be verified separately using pole, threshold, scattering data, and cosmological observations.

Bessel common carriers are one candidate for this hidden continuum.This is an illustration of a single compressed spectral channel carrying several internal directions in common and emitting valid states of matter at the boundaries.The name Bessel comes not from an external program but from a specific differential equation and its spectral structure.

However, it should not be assumed that exact Bessel transport remains the same in all sectors.Scalar stabilization, gauge interactions, defects and boundary conditions can modify the spectrum.Therefore, it is necessary to distinguish between the correct Bessel core, the deformed sector, and the low-energy matching area.

The advantage of this block structure is that it localizes failure.If the UV behavior of a particular hidden continuum fails, the implementation can be discarded, but there is no need to discard WRRA's higher-level question of separating the source and visible phenotypes.

## Related public research

**Quantum Realization Hierarchy of the Bessel Common Carrier** [<u>10.5281/zenodo.22121400</u>](https://doi.org/10.5281/zenodo.22121400)

# Chapter 21 Quantum Realization Has Multiple Layers

There is not one path to quantum realization of the Bessel common carrier.Research genealogy distinguished three levels.The first is a finite Jacobi runtime, the second is a single generalized-field spectral runtime, and the third is a warped defect-holographic parent.[Refer to Appendix D ‘Jacobean Matrix’]

*Jacobi runtime → spectral field → warped defect parent* (3.7)

A finite Jacobi runtime approximates a continuous spectrum with a finite matrix and discrete states.It is the most conservative, computable, and local quantum runtime.It is good to numerically fit the response of poles and residues and limited energy windows, but it does not preserve the exact infinite continuum.

A single generalized field preserves the continuum compressed within a single non-local or pseudodifferential spectral symbol.Although it is possible to express the target two-point function without introducing an infinite number of independent charged fields, closure of the interaction subgraph, gauge completion, and renormalization are separate thresholds.

Warped defect parents are one step more geometric.Higher-order local fields produce Bessel-type spectra at boundaries or defects.Although it may give rise to claims of bulk causality and positive spectral compression, this does not mean that it is a fundamental dimension of nature.

Even though the three runtimes reproduce the same amount of two-point spectral target in a limited matching window, they are not physically the same theory.The Hilbert space in which the number of fields, locality, gauge completion, ultraviolet ray cost and unitarity are defined is different.

*G₁(E) ≈ G₂(E) on E∈W ⇏ Theory₁ = Theory₂* (3.8)

Therefore, the statement that ‘the quantum realization stage is over’ must be said on a layer-by-layer basis.Two-point representation, interaction consistency, one-loop relative closure, all-loop completion, and standard model embedding are different thresholds.The current study has closed some layers, but has not completed the entire quantum gravity.

## Related public research

**Conditional One-Loop Relative BRST Closure of the Single-Field Bessel Spectral Carrier** [<u>10.5281/zenodo.22121047</u>](https://doi.org/10.5281/zenodo.22121047)

**Quantum Realization Hierarchy of the Bessel Common Carrier** [<u>10.5281/zenodo.22121400</u>](https://doi.org/10.5281/zenodo.22121400)

# Chapter 22 A Possible Local Standard-Model Parent

In the quantum realization genealogy, the 5-dimensional Einstein–scalar parent was presented as the first explicit local implementation chassis of WRRA.It is a structure that stabilizes the finite warped interval with a scalar boundary condition and places a Bessel radial core and a chiral standard model zero mode on it.

*ds² = e^(−2A(y))η_μνdx^μdx^ν + dy²* (3.9)

The advantage of this model is that length, gap, chirality, and transmission can be treated together in one local field theory framework.A finite Kaluza–Klein gap separates the low-energy visible sector from the heavy mode, and the generation-universal transport is structured in a way that preserves the observed Yukawa·CKM·PMNS data.

However, ‘preserve’ and ‘predict’ are different.Inserting the observed Yukawa and mixed data as matching input and maintaining it at low energy is a test of feasibility of implementation.The figure was not derived from geometry alone.

*O_low(μ) = Match_μ\[O_parent;θ_obs\]* (3.10)

Additionally, low-energy theories should not be defined by simple Kaluza–Klein cuts.Gauge-covariant matching and threshold correction are required, and the scalar-deformed sector and exact Bessel sector must be separated.Stability, anomaly inflow, flavor counterterm, BRST and cutoff corridor conditions must also be met.

Therefore, the exact status of the 5-dimensional parent is a possible local implementation chassis.It is not the final body of WRRA, nor is it a structure necessarily used by nature, nor is it a fundamental theory that is valid at all scales.

This limitation is not only a weakness.The fact that one of the possible renderers was actually built in an existing field theory language means that the architecture does not remain pure metaphor.Now the deeper question is, what conditions are necessary for different implementation paths to yield the same observational reality?

## Related public research

**A Stabilized Local Standard-Model Parent for the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22123134</u>](https://doi.org/10.5281/zenodo.22123134)

# Chapter 23 Renderer path independence

Let's say we have two rendering paths that start from the same physical boundary and end up at the same boundary.Even if the intermediate slice and gauge selection and decomposition order are different, the final observation content should not change.WRRA calls this renderer path equivalence or path independence.

*R_γ₁(B_f,B_i) ≃\_gauge R_γ₂(B_f,B_i)* (3.11)

This principle does not mean that all intermediate expressions must be literally identical.Differences corresponding to gauge redundancy are allowed, but gauge-invariant observables must match.Therefore, path independence is a condition that separates the overlap of observations and expressions.

When small deformations are applied in different orders, the differences should be closed back to the permitted deformations.If a local slice can be embedded in a non-degenerate space-time geometry, a hypersurface-deformation algebra provides the kinematics of this deformation.

In the canonical representation, these transformations appear as first-class constraints.If the constraint algebra is not closed, different slicing paths create different physical states or leave behind an anomaly.Then the renderer cannot consistently implement the same reality.

*{H\[N\],H\[M\]} = D\[qᵃᵇ(N∂\_bM−M∂\_bN)\]* (3.12)

However, it would be an exaggeration to say that path independence itself directly creates the Einstein equation.It requires the necessary gauge and deformation structures.Which dynamics branch is chosen depends on the canonical variables used, locality, differential order and additional degrees of freedom.

This principle changes WRRA in a verifiable direction.The difference between boundary observables calculated in different renderer paths can be measured, and if constraint anomaly or source-clock leakage remains, the implementation will fail.

## Related public research

**Renderer Path Independence and the Einstein Branch of the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22124886</u>](https://doi.org/10.5281/zenodo.22124886)

# Chapter 24 Restorable renderer and metric faithfulness

When path equivalence is applied to quantum renderers, a new problem arises.General quantum channels are not reversible.Even a fully positive, trace-preserving CPTP map can make two different states more similar, erasing location-distinguishing information and metric rank.

Root fidelity does not decrease under the CPTP map.Therefore, the distance defined by fidelity shrinks, and the information geometry metric derived from a sufficiently smooth state family can also become small in the output.The mere fact that it is a quantum channel does not preserve spatial orientation and localization.

*F(Φρ, Φσ) ≥ F(ρ,σ) ⇒ g_out ≤ g_in* (3.13)

WRRA v1.1 does not solve this problem with the inverse function of the entire renderer.Specifies the code subspace or observable algebra that needs to be physically protected, and requires that a recovery map exist only in that area.Restoration is not about reviving the entire microstate, but about preserving the logical information necessary for visible reality.

*Recovery ∘ Φ = id on A_protected* (3.14)

At this time, three conditions must be distinguished.First, localization rank must be preserved.Second, the output state family must achieve faithful immersion in a common corrected space-time geometry.Third, the protected observable algebra must be restored after recovery, including the intended logical time evolution.

Path equivalence changes to recovered path equivalence.The raw output of two different paths need not be the same.After appropriate recovery of each path, the same intended transition with the same physical content must be obtained in the protected observation log.

*R₁∘Φ_γ₁ ≃ R₂∘Φ_γ₂ on A_protected* (3.15)

Here, invariants and physical transitions should not be confused.Flavor mixing and decay do not preserve the original state.What the renderer must preserve is not the fact that there is no change, but that the allowed sector-changing evolution and its probability, charge, and local records are implemented correctly.For this, Fock space or direct-sum sector may be required.

## Related public research

**Recoverable Rendering and Metric Faithfulness in the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22125506</u>](https://doi.org/10.5281/zenodo.22125506)

# Chapter 25 Maintaining the same reality over time

We cannot immediately conclude that a renderer that is restorable at one point in time will maintain the same reality over time.Even if the quantum channels at each stage can be restored individually, if small errors accumulate repeatedly, the protected observation algebra and local geometry may change after a long time.Snapshot recoverability and long-time stability are different thresholds.

The most direct sufficient condition is that the disturbance size ε_k at each stage can be summed.If the cumulative error up to n steps is controlled by the sum of the errors at each step and the infinite sum is finite, the error can be kept within a time-independent range even after repeated rendering.This is a stronger condition than saying that each step is small.

*‖E_n‖ ≤ Σ\_(k=1)^n ε_k, Σ\_(k=1)^∞ ε_k \< ∞* (3.16)

v1.2 distinguishes three sufficient mechanisms for time-uniform restoration.There is a summable disturbance in which the sum of the disturbances is finite, a noiseless observable algebra in which the protected observable algebra is exactly preserved, and a contractive recovery in which the state after recovery is contracted to the attractor code manifold.The three mechanisms can replace each other or be used together.

In shrinkage reconstruction, the current error is reduced to less than λ times at each step and a new disturbance ε_k is added.If λ, which is above 0 but below 1, remains independent of time, past errors are exponentially forgotten, and under limited new perturbations, the state stays around the code manifold.However, it should not be a restoration that stops the intended logical time development.

*d\_(k+1) ≤ λd_k + ε_k, 0 ≤ λ \< 1* (3.17)

The fact that the metric rank at one point in time is 3 does not guarantee a continuous three-dimensional space.Uniform ellipticity is required, where the effective metrics at all points in time are uniformly limited above and below a common reference metric.Additionally, quantum Fisher or Bures metric, which can vary from probe to probe, should not be directly equated with shared space-time geometry.The characteristic cones of bosons and fermions must also be compatible with the same corrected causal structure.

*c g\_\* ≤ g_k ≤ C g\_\* for all k* (3.18)

Reality is not something that is restored separately for each local area and then simply put together.The recovery defined in the overlapping regions U and V must be compatible with the protected observations of the intersection.Without this quasi-local compatibility, each local observation, even if normal, is not stitched into a single global reality.The stability of geometric and quantum states also feeds back to each other and must be controlled together.

*R_U│\_(U∩V) ≃ R_V│\_(U∩V)* (3.19)

Restoration also follows a thermodynamic ledger.The cost of reading the syndrome, erasing information, and leaving feedback in geometry and matter should not be hidden.The conclusion of this chapter is the conditional theorem that a time-uniform WRRA interface is sufficient under these conditions.This is not a declaration that the derivation of the microscopic renderer or the actual implementation of the entire time in the universe has been completed.

*L_thermo = S_syndrome + C_erasure + B_backreaction* (3.20)

## Related public research

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22126125</u>](https://doi.org/10.5281/zenodo.22126125)

The WRRA Information Provision Ledger 10.5281/zenodo.22139233

# Chapter 26: How is the Einstein branch selected?

Even if renderer path independence requires consistency of hypersurface deformation, the possible gravitational dynamics are not fixed to one without additional assumptions.To obtain the Einstein branch, a Hojman–Kuchař–Teitelboim type condition must be specified.

The key assumptions are a local metric canonical variable, standard spatial-diffeomorphism action, reversibility, absence of additional gravitational canonical fields, at most quadratic dependence on momentum, and no more than two spatial derivatives.

Under this condition, if the Hamiltonian constraint and momentum constraint implement hypersurface-deformation algebra as first-class, Einstein dynamics of general relativity is selected as the conditional low-energy branch.The cosmological constant term may be allowed and its specific value is a separate vacuum and observation matter.

*Recovered path equivalence + HKT assumptions ⇒ Einstein branch* (3.21)

Therefore, the correct direction of logic is not ‘path independence ⇒ Einstein equation.’‘Path equivalence ⇒ consistent deformation/gauge structure’, and ‘the structure + HKT type assumption ⇒ Einstein branch’.

*G_μν + Λg_μν = 8πG T_μν* (3.22)

Other branches are possible by allowing additional scalar, higher derivative, nonlocal variable or other canonical content.This does not mean that WRRA denies Einstein gravity, but rather makes the scope and selection assumptions of Einstein gravity clear.

The position of the 5-dimensional parent is organized in the same way.It is a chiral/spectral dilation candidate for the matter renderer, not the ultimate SOURCE.The low-energy gravity of our universe may follow the Einstein branch, but the underlying structure of the renderer may be broader.

## Related public research

**Renderer Path Independence and the Einstein Branch of the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22124886</u>](https://doi.org/10.5281/zenodo.22124886)

**Recoverable Rendering and Metric Faithfulness in the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22125506</u>](https://doi.org/10.5281/zenodo.22125506)

# Chapter 27: Time, Geometry, Big Bang, and Open Verification

In WRRA, time does not need to be given by an external absolute clock.Time can be defined by changes in relationships between states and the correlation of the clock subsystem.However, if traces of the source clock leak non-universally into visible observations, the equivalence principle and path independence may be broken.

*T_rel = T(clock correlations)* (3.23)

Geometry can also be partially reconstructed not only from a pre-placed background but also from the distinguishability between states.Although it is possible to construct effective metrics from fidelity or information distance, it does not automatically guarantee Lorentzian spacetime and Einstein dynamics.Signature, locality and constraint closure must be checked separately.

The physical degrees of freedom of gravity must also be counted after removing the constraint.You cannot count only the number of components of a 3-dimensional space metric and call it graviton degree of freedom.After removing the first-class constraint and gauge orbit, two propagation degrees of freedom remain for each point in the 3+1-dimensional Einstein branch.

*N_phys = ½(12 − 2×4 − 0) = 2* (3.24)

The big bang can potentially be interpreted as the renderer's initial boundary or rank-opening transition.However, this is currently an open hypothesis.To equate the autonomous opening of the Bessel common carrier with the cosmological Big Bang, primordial spectrum, scale invariance, non-Gaussianity, reheating and standard cosmological data must be passed together.

The next verification does not end with tuning to match the numbers.Calibration data and post-verification data must be separated, and values ​​not entered among pole·residue·threshold·gauge observable·flavor data·gravitational wave and cosmology data must be predicted.

*Prediction = Output(test data not used in calibration)* (3.25)

WRRA's open possibilities are not an empty space to avoid failure.Anomaly-free quantum constraint closure, physical state space, observable equivalence between renderers, source-clock leakage bound, and independent low-energy prediction are the specific next bosses.While maintaining the principle that our universe is a possible realization, candidates to explain that realization must compete in the face of observation.

## Related public research

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22126125</u>](https://doi.org/10.5281/zenodo.22126125)

# Part 3 Boundaries and next research

What is fixed in Part 3 is the minimal structure of WRRA and one conditional Einstein branch.In a general quantum renderer, recovered path equivalence on a protected observation algebra is required, not raw path identity, and recovery possibility at one point in time is not enough.Time-uniform disturbance control, uniform ellipticity of common geometry, and quasi-local recovery of overlapping regions are required.These conditions require consistency of gauge and deformation, but they alone do not prove the uniqueness of Einstein's equations.

The 5-dimensional Einstein–scalar parent and Bessel carrier are possible local implementations.Numerical derivation of Standard Model parameters, all-loop quantum completion, and identification of physical state space and cosmological Big Bang are still open.

The goal in the next step is not to adjust more parameters, but to freeze the calibration set, estimate held-out observables, and test whether different renderer runtimes reproduce the same observables.

**Part 4**

**How our universe is tested**

From calibration to prediction
