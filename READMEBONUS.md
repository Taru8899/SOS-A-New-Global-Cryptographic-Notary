

SOS Monetary System — Hybrid Time- & Gas-Backed Model

I. System Overview

The SOS system consists of two layers of monetary stability:

Stage 1 — ETH Gas-Cost Production Floor

Raw SOS requires ETH to mint.

Imposes economic friction, preventing free inflation.


Stage 2 — Time-Minted Raw Base

Raw SOS grows deterministically over time.

Provides a predictable, immutable monetary base.


Wrapped SOS Layer

Represents tradable tokens backed by Raw SOS.

Maximum issuance capped by reserve ratio: CR ≥ 5.

Includes dynamic bonus issuance tied to reserve health.


Key Rules:

No buybacks or burn incentives.

Hard reserve constraint: CR ≥ 5.

Deterministic issuance ensures long-term stability.




II. Bonus Mint Strategy

Principle: Bonus minting cannot weaken reserve ratio (CR).

Bonus is issued only from excess reserve capacity:

CR(t) = R(t) / W(t)
E(t) = R(t) - 5 * W(t)

Maximum bonus per mint:

B_max = E(t)/5 - ΔW


Dynamic Bonus Curve:

BonusRate = k * (CR - 5)/5

CR = 5 → Bonus = 0

CR > 5 → Bonus increases proportionally

Smooth continuous function, no fixed tiers


Outcome:

Avoids paradoxical incentives (committing less does not give higher bonus).

Strengthens Wrapped SOS by tying expansion to actual reserve capacity.

Self-correcting: CR oscillates naturally between 5–6.




III. Equilibrium Price Model for Wrapped SOS

Backing Density:

D = R / W

Ensures each Wrapped SOS is supported by ≥5 units of Raw SOS.


Reserve Premium Model:

θ = 1 - W / (R/5)
P_w ∝ 1 / (1 - θ)

Scarcity of Wrapped increases its price as reserve utilization approaches limit.

Linear Raw growth → predictable maximum Wrapped supply → lower volatility.


Long-Term Behavior:

Stable appreciation.

Mean-reverting bands prevent runaway inflation.



IV. Game Theory of Rational Minters

Player Types:

1. Early Minters


2. Late Minters


3. Passive Holders



Incentives:

Bonus tied to global CR only.

Rational strategy: mint when CR high, wait when CR tight.


Nash Equilibrium:

Natural oscillation around CR ≈ 5–6.

No advantage in panic exit → no bank-run dynamics.




V. Monetary Policy Function (Whitepaper Section)

5.1 Base Issuance

R(t) = R_0 + α * t

Deterministic time-based Raw SOS issuance.


5.2 Credit Layer Constraint

CR(t) = R(t) / W(t) ≥ 5

Ensures minimum 500% reserve for Wrapped SOS.


5.3 Expansion Valve — Bonus Mechanism

Bonus allowed only when CR > 5.

Maximum issuance:


W_new ≤ R(t) / 5

5.4 Stability Layers

1. Production Floor: ETH cost per mint.


2. Structural Reserve: deterministic time base.



5.5 Risk Bound

Leverage L(t) = W(t)/R(t) ≤ 0.2

Guarantees systemic solvency for all time.



VI. 50-Year Macro Simulation (Conceptual)

Raw base grows monotonically.

Wrapped SOS capped at 20% of Raw.

CR oscillates between 5 and 8.

Bonus activates during high CR.

System converges to cyclical steady state.


Extreme Scenarios:

ETH crash → Stage 2 intact.

Bull mania → CR constraint prevents runaway.

Demand collapse → CR rises automatically.


Observation:

Over 50 years, risk remains bounded, leverage capped, reserves grow asymptotically.


VII. Conceptual Insights

Not a stablecoin — a time-indexed, reserve-constrained monetary constitution.

Structurally anti-fragile:

Time increases safety

Usage increases value

CR constraint prevents collapse


System mimics central-bank style policies entirely on-chain:

Dynamic bonus → interest-rate style expansion

CR floor → reserve requirement

ETH friction → production cost floor


Bonus is fully endogenous, not market-dependent.

Maximum systemic leverage permanently bounded → mathematically provable stability.
