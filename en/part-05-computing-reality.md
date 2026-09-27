# Part V — Computing Reality

# Opening words of Part 5

Part IV concluded that verification of WRRA requires separation of calibration data and sealed forecast data.Part 5 applies the principles to real finite calculations.

Convert a single positive continuous spectrum into a finite Jacobi matrix and read the Euclidean resolvent and real-time amplitude from the same visible port.On top of that, localization metric and syndrome recovery are added as separate factors to form the minimum restorable rendering benchmark.[Refer to Appendix D ‘Euclidean-Lorentz signatures’]

This calculation is not the completion of the entire microscopic universe.It is the purpose of this section to record separately what has been accurately calculated, what has been observed in finite samples, what has been preserved by construction, and what is still open.

# Chapter 36 From Declarative Architecture to Computable Model

So far, WRRA has organized the conditions necessary for the implementation and restoration of reality into a declarative interface.However, no actual calculation occurs with just the three words SOURCE, RENDERER and PHENOTYPE.At least one Hilbert space, self-involved Hamiltonian, observation port, and restoration channel must be configured in a finite form.

The goal of Part 5 is not to replicate the entire universe in a computer.The positive continuous spectrum is approximated with a finite Jacobi matrix, the Euclidean resolvent and real-time survival amplitude are calculated on it, and a minimum existence benchmark is created that attaches restoration dynamics to a separate localization/syndrome layer.

*H_N = H_Jacobi ⊗ H_loc ⊗ H_syn* (5.1)

This benchmark is factorized.Spectral simulation, localization metric and recovery channel are set to different tensor factors.Therefore, each condition can be passed explicitly, but it is not claimed that these three elements arose spontaneously from a single microscopic interaction.

The central calculation paper is Finite-Jacobi Compatibility Benchmark for WRRA v1.2, published on August 27, 2026.The public version of Version 1.2 was given DOI 10.5281/zenodo.22126918, and the time-uniform WRRA paper 10.5281/zenodo.22126125 is supplemented as a numerical benchmark.

The success criteria for calculations are also limited.Positive weights, real nodes, self-adjoint finite Hamiltonian, rank-one visible port, convergence of finite Euclidean window, explicit recovery gap and bounded syndrome entropy must exist together.

*Benchmark = spectral simulation + metric corridor + recovery ledger* (5.2)

The meaning of this construct is not ‘proving that the universe is a simulation.’This is the first constructive evidence that some of the declared conditions of WRRA can be realized simultaneously within a single finite accounting ledger without contradicting each other.

## Related research

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [<u>10.5281/zenodo.22126918</u>](https://doi.org/10.5281/zenodo.22126918)

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22126125</u>](https://doi.org/10.5281/zenodo.22126125)

# Chapter 37 Converting a continuous spectrum to a finite Jacobi matrix

The starting point is the positive generalized-Laguerre spectral density above the threshold s₀.If α is greater than −1, the density can be normalized, and in this study, s₀=1, Λ²=1 and α=1/2 were used.The weight of the continuum is positive and the overall integral is 1.

*ρ(s) = \[(s−s₀)^α e^(−(s−s₀)/Λ²)\]/\[Γ(α+1)Λ^(2α+2)\] Θ(s−s₀)* (5.3)

If you use the variable x=(s−s₀)/Λ², the measure will be in the form x^αe^(−x)/Γ(α+1).The ternary equation of the generalized Laguerre polynomial orthogonal to this measure determines the real symmetric Jacobi matrix.

The diagonal component of the N×N Jacobi matrix is ​​s₀+Λ²(2n+α+1), and the adjacent off-diagonal component is Λ²√((n+1)(n+1+α)).Since the matrix is ​​real symmetric, the eigenvalues ​​are real and unitary finite-time evolution is precisely defined.

*(J_N)\_(nn)=s₀+Λ²(2n+α+1), (J_N)\_(n,n+1)=Λ²√((n+1)(n+1+α))* (5.4)

If the first basis vector e₀ is selected as the visible port, the weight of each eigenvalue s_j becomes the square of the first component w_j according to the spectral theorem.Therefore, w_j is not negative and the sum is 1, and one rank-one collective port reads N hidden spectral nodes.

This structure does not declare the continuum as N independent physical particles.The goal is a Gaussian quadrature and finite state-space realization of the spectral measure.N is not the natural number of particles, but an approximate order.

The strongest point of Jacobi's construct is that positivity and self-contingency are not obtained by post hoc testing.Since it follows structurally from the measure and recurrence, it avoids the risk of arbitrarily fitting complex poles or negative spectral weights.

## Related research

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [<u>10.5281/zenodo.22126918</u>](https://doi.org/10.5281/zenodo.22126918)

# Chapter 38 How one visible port reads the continuum

The Euclidean response of a continuous spectral target is read as a Stieltjes transform.When Q² is greater than 0, G_E(Q²) is the integral of spectral density divided by Q²+s.In the finite Jacobi model, the same quantity becomes the diagonal matrix element of the resolvent for e₀.

*G_E(Q²)=∫ ρ(s)/(Q²+s) ds* (5.5)

If we diagonalize the matrix, the finite response is the sum of w_j/(Q²+s_j).This expression shows that the quadrature nodes and weights are not a simple list of numbers, but come from a single self-involving Hamiltonian and visible vector.

The real-time amplitude is also owned by the same data.The continuous goal is A(t)=e^(−it)(1+it)^(−3/2), and the finite model is A_N(t)=Σ_jw_je^(−is_jt).Do not fit the Euclidean response and real-time amplitude with different parameters.

*A(t)=e^(−it)(1+it)^(−3/2), A_N(t)=Σ_j w_j e^(−is_jt)* (5.6)

One port reading all nodes means that information is compressed to rank one, not that the entire material space is one dimension.The state dimension of the hidden Jacobi chain is N, and only visible coupling is achieved through e₀.

This common-owner structure is in line with WRRA's minimal computation intuition.Rather than attaching separate sensors and separate transmitters to each component of the continuum, one collective boundary coordinate carries common spectral content.

However, this visible port is not yet a standard model particle with charge, spin, and flavor.It is a minimal interface to read the spectrum without loss, and the joint realization of physical quantum numbers remains a larger embedding problem.

## Related research

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [<u>10.5281/zenodo.22126918</u>](https://doi.org/10.5281/zenodo.22126918)

# Chapter 39 How accurate is it in the Euclidean window?

The first test of the finite model was done in the Euclidean window of Q²∈\[0,10\].We increased the Jacobi order to N=2,4,8,16,32 and compared the maximum relative error of the exact Stieltjes transform and the finite resolvent.

*δ_N = max\_(Q²∈\[0,10\]) \|G\_(N,E)−G_E\|/\|G_E\|* (5.7)

The errors were, in order, 4.089×10^(−2), 4.746×10^(−3), 1.858×10^(−4), 1.623×10^(−6), and 1.763×10^(−9).At N=32, it goes down to a few parts per billion within the specified window.

The observed fit equation log δ_N≈−0.55N−3.31 summarizes the fast convergence in this finite sample.However, this is not a proven asymptotic theorem, but an empirical fit from N=2 to 32.The same slope is not guaranteed for different windows and different α.

*log δ_N ≈ −0.55N − 3.31 \[empirical\]* (5.8)

The numerical consistency of node and recurrence was also confirmed.The difference between eigenvalues ​​and quadrature nodes ranged from approximately 2.2×10^(−16) to 5.7×10^(−14) depending on the degree.This is consistent with the stability of the double-precision calculation used.

The reason why Euclidean convergence is fast is because the Stieltjes kernel is smooth outside the positive real axis and is advantageous for quadrature.This success should not be directly translated into the accuracy of Lorentzian long-term dynamics.

Therefore, the correct verdict in this chapter is fixed-window PASS.For a specified spectral density and Euclidean window, the finite Jacobi resolvent converges quickly, but completion for all scales and all complex regions is open.

## Related research

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [<u>10.5281/zenodo.22126918</u>](https://doi.org/10.5281/zenodo.22126918)

# Chapter 40 Real-time tracking window and returning waves

The amplitude A(t) of the continuous spectrum decreases with phase mixing.However, since the finite Jacobi system is a finite sum of discrete eigenvalues, it cannot permanently reproduce complete irreversible decay.After a sufficiently long period of time, recurrence and revival appear.

In the calculation, the time until the relative error between continuous amplitude and finite amplitude exceeds 1% was defined as T_1%.For N=2,4,8,16,32, 0.43857, 0.96863, 1.69659, 2.67806, and 4.02408 were obtained, respectively.

*T\_(1%) = sup{T : relative error ≤ 0.01 on \[0,T\]}* (5.9)

The empirical fit for this data is T_1%≈0.84√N−0.72.Even if the order is quadrupled, the reliability time tends to roughly double.This equation is also not an asymptotic theorem, but a summary of the five-order benchmark used.

*T\_(1%) ≈ 0.84√N − 0.72 \[empirical\]* (5.10)

The long-term average survival plateau decreased to 0.700, 0.450, 0.3236, 0.2318, and 0.1650.As N increases, the average size of visible bounces decreases, but this does not result in permanent continuum damping at finite N.

This result makes the boundary between simulation and realization clear.Finite closed systems can mimic continuous response very accurately in a defined time window, but they do not possess infinite time irreversibilities and thermal arrows.

Therefore, adopting N as a physical cutoff requires a tracking window longer than the observation time, experimental invisibility of revival, or combination with the real environment.Otherwise, the model remains a finite-window simulator.

## Related research

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [<u>10.5281/zenodo.22126918</u>](https://doi.org/10.5281/zenodo.22126918)

# Chapter 41: What does the recovery cycle restore?

The restoration conditions of WRRA v1.2 cannot be tested using spectrum simulation alone.For this purpose, the entire space is expanded by the tensor product of the Jacobi spectral factor, localization factor, and syndrome qubit.

The selected recovery generator is an amplitude-damping Lindblad operator.The syndrome excitation is lowered to the ground state at σ\_-, the lateral component of the density matrix is ​​attenuated at a rate of κ/2, and the population defect is attenuated at a rate of κ.

*L_rec(ρ)=κ\[σ₋ρσ₊−½{σ₊σ₋,ρ}\]* (5.11)

The corrective gap in the syndrome-transverse sector is Δ_corr,N=κ/2.This value does not depend on the Jacobi order N and recovery order.This is the exact-in-construction gap obtained because the recovery factor is separated from the spectral chain.However, since the unitary recurrence of the Jacobi sector remains, this does not mean that the entire Liouvillian is mixing.

*Δ\_(corr,N)=κ/2 \[syndrome-transverse sector\]* (5.12)

This restoration does not reverse the normal temporal evolution of the spectral amplitude.The intended unitary evolution of the Jacobi sector is maintained while eliminating errors in the syndrome factor.It follows the WRRA principle that restoration does not undo all changes.

However, factorization is a strong assumption.In an actual micro renderer, there may be interaction between spectral, localization and syndrome sectors, and the combination may reduce uniform gap or create new leakage.

Therefore, what passes here is the existence of a recovery channel and accurate gap calculation.Simulation error and recovery error have not yet been controlled for a long time with a single coupled inequality.

## Related research

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [<u>10.5281/zenodo.22126918</u>](https://doi.org/10.5281/zenodo.22126918)

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22126125</u>](https://doi.org/10.5281/zenodo.22126125)

# Chapter 42 Metric corridor and space conservation

Even if there is a restorable state, if the localization metric collapses, it cannot be said that the same space has been maintained.The benchmark places the common reference metric g_ref directly on the localization factor and sets g_N=g_ref for all N.

*c_N g_ref ≤ g_N ≤ C_N g_ref* (5.13)

In this selection, the uniform ellipticity constant c_N=C_N=1 and the condition number is also 1.Therefore, even if the order increases, the metric rank and length scale for each direction are accurately maintained.

*g_N=g_ref, c_N=C_N=1, cond(g_N)=1* (5.14)

This result is not a numerical discovery, but an exact statement by construction.Because the metric corridor is in the tensor factor independent of the spectral approximation, it is automatically preserved.

At the same time, it is clear why this does not explain the origin of three-dimensional space.This is because the standard metric and dimension were entered.The benchmark showed that it could preserve a given space, but did not calculate the process in which the three directions spontaneously opened in SOURCE.

In a stronger model, g_N should not be fixed but made a function of the spectral state and recovery current.Then it is necessary to test whether uniform ellipticity and common characteristic cone are maintained under the actual dynamics.

The current judgment is metric preservation PASS, dynamical geometry origin OPEN.These two sentences must be written together to avoid mistaking the entered space for the predicted space.

## Related research

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [<u>10.5281/zenodo.22126918</u>](https://doi.org/10.5281/zenodo.22126918)

**Recoverable Rendering and Metric Faithfulness in the Wonsik Reality-Renderer Architecture** [<u>10.5281/zenodo.22125506</u>](https://doi.org/10.5281/zenodo.22125506)

# Chapter 43 syndrome entropy and cost of restoration

Restoration does not become free just because it is logically possible.If the syndrome bit is excited with probability p, the Shannon entropy to be processed in one cycle is −p ln p−(1−p)ln(1−p).

*ΔS_rec=−p ln p−(1−p)ln(1−p)* (5.15)

At p=0.01 of the benchmark, ΔS_rec,N=0.0560015 nat/step.This value is independent of N and is finite.It is a bounded ledger obtained because the syndrome factor is fixed to one qubit.

Applying the Landauer lower bound, the minimum heat cost is Q_min=0.0560015 k_BT per step.This is not the actual device or space heat output, but the ideal lower limit required to irreversibly erase the selected syndrome record.

*Q_min=k_BT ΔS_rec=0.0560015 k_BT at p=0.01* (5.16)

To calculate the actual cost, cycle time, bath temperature, coupling efficiency, error production rate and backreaction are needed.Because these values ​​are not available, the cosmological heat budget has not yet been calculated.

Also, the fact that entropy is bounded is different from the fact that long-term total cost is bounded.If the cost per cycle is positive, the cumulative cost of an infinite cycle continues to increase without resource supply and release channels.

Therefore, what the benchmark has closed is a cycle of syndrome entropy ledger.How long the universe performs this restoration and what reservoir it uses are the next steps.

## Related research

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [<u>10.5281/zenodo.22126918</u>](https://doi.org/10.5281/zenodo.22126918)

# Chapter 44 Calculated, combined, not yet calculated

Part 5 is comprised of positive finite-Jacobi realization, real nodes and weights, self-adjoint Hamiltonian, rank-one visible port, and Euclidean/real-time response from the same owner.

What was confirmed numerically was the fixed Euclidean window error from N=2 to 32, 1% real-time tracking window, survival plateau, and node consistency.The fitting formula for error and tracking window is an empirical relationship and is not promoted to an asymptotic theorem.

Closed by exact-in-construction is the N-uniform syndrome-transverse corrective gap of the selected factorized recovery, the metric corridor of the fixed localization factor, and the bounded entropy per cycle of the selected syndrome qubit.The entire Liouvillian mixing was not closed.

What is open is the coupled long-time bound of simulation error and recovery cycle, the origin of dynamical three-dimensional geometry, Lorentzian microcausality, interacting gauge-covariant completion and empirical prediction of the Standard Model, real thermal reservoir, gravitational backreaction and all-scale completion.

Therefore, the final proposition is not ‘the complete universe renderer has been calculated’.‘WRRA's spectrum approximation, localization preservation, restoration gap, and entropy ledger can be realized simultaneously in one finite factorized benchmark.’

*Result₀ = minimal factorized compatibility benchmark* (5.17)

Subsequent research revealed actual coupling between the separate factors.The first off-diagonal localization–carrier combination showed a finite order corridor in the selected gapless benchmark, but the acceptance region and positivity boundary varied depending on the Jacobi order.This is not a no-go for all gapless couplings, but rather a failure of the off-diagonal architecture tested.

*H_coupled = H_Jacobi + H_loc + V_loc-carrier* (5.18)

Nearest-neighbor gauge-covariant derivative coupling restored finite-order positivity and satisfied exact identity for the rank-one compressed response.However, as the principal kinetic coefficient varied depending on the carrier, different characteristic cones were created.The success of positive and compressed responses alone did not lead to the preservation of a common spatiotemporal phenotype.

*positivity corridor = corridor(N, coupling)* (5.19)

In this failure, the conditional selection rule remains.Under the base-class assumption that the physical principal symbol is Hermitian, strongly hyperbolic, and has constant multiplicity and diagonalizability, WRRA-compatible carrier dependence should not split the relative principal causal cone.

*P_principal(ξ; carrier) split ⇒ multiple characteristic cones* (5.20)

In the surviving finite-Jacobi class, the universal kinetic geometry is maintained in common, and the differences between carrier and background are entered into a lower-order gauge-covariant phenotype operator.Representation-preserving scalar dressings are allowed, but the chiral mass and Yukawa require a separate Higgs-owned gauge intertwiner over the doubled chiral representation space.

*∂P_principal/∂carrier = 0, carrier dependence ∈ L_lower* (5.21)

Therefore, the current advance is a finite-order local quadratic runtime PASS.Factorization has been partially unlocked for the first time, but continuum domain convergence, Lorentzian microcausality, interacting BRST closure, Standard-Model completion and empirical prediction are still open.

*Status = finite-order local quadratic runtime PASS* (5.22)

## Closed by the first generation inventory audit

The tensor-product carrier of 6369 modes and 15 internal components can contain the first generation standard model inventory without loss.When substituting the known standard model expression and hypercharge, the perturbative anomaly and SU(2) global anomaly conditions also pass accurately.Therefore, the acceptability and anomaly compatibility of representation inventory are no longer vague OPEN items.

SM15 compatibility = capacity PASS ⊕ anomaly EXACT ⊕ mass availability PASS (5.23)

However, this result does not unconditionally prove “why 15” upstream, nor does it mean that 6369 zeta modes created the standard model charge.The mass mode is an availability audit, not a prediction, because it selects the grid point closest to the observed value.The actual interacting operators, W± transitions, Higgs intertwiner, generational replication, CKM·PMNS mixing and pole residues are still OPEN.

Therefore, the current exact position is up to “there is room for the standard model and it does not conflict with known first generation data.”We have not yet reached the stage of “deriving the standard model from scratch and predicting the new mass.”

## Related research

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [<u>10.5281/zenodo.22126918</u>](https://doi.org/10.5281/zenodo.22126918)

**Local Covariant Nonfactorized Rendering in WRRA** [<u>10.5281/zenodo.22127549</u>](https://doi.org/10.5281/zenodo.22127549)

# Conclusion of Part 5 Calculations have begun, but the universe is still open

This benchmark showed that some of WRRA's declarative conditions can coexist in an actual finite quantum model.Positive Jacobi spectrum, fixed-window convergence, rank-one visible port, recovery gap, metric corridor and syndrome entropy are placed in one computational ledger.

At the same time, the recurrence of finite closed systems, the input localization metric and the factorized recovery make the limits clear.This does not yet compute permanent continuum damping, the generation of three-dimensional geometry, or the actual thermodynamics of our universe.

A subsequent nonfactorized study actually turned on factor coupling and tested both pathways.The simple off-diagonal combination was eliminated due to the order-dependent corridor, and the gauge-covariant derivative combination passed finite order positivity and compressed response but split the common causal cone.

The current surviving direction is local quadratic runtime, which preserves the common principal kinetic geometry while placing material-specific differences in the lower-order gauge-covariant phenotype operator.Now the next bosses are continuum convergence, Lorentzian microcausality, interacting BRST closure, and real particle/observation data.

**Part 6**

**Open Universe**

What we learned and what the next person will follow
