Title:

Bifurcation-Margin Reinforcement Learning: A Validated Stability-Boundary Detector, and Why It Has Not Yet Improved Locomotion Control

Abstract:

This paper makes two contributions of different character. The first is a validated framework: Bifurcation-Margin Reinforcement Learning (BM-RL) estimates, online and without an analytical model, the Floquet multiplier of the closed-loop Poincaré return map as a bifurcation margin m = 1 − |λ|, and constrains actor-critic optimization to keep it away from the flip-bifurcation boundary via Lagrangian dual ascent. This tracks a qualitative failure mode — a stable gait losing stability and turning to chaos — that existing Lyapunov, contraction, and barrier certificates do not, since they certify only local stability. We derive an exact closed-form bifurcation threshold for a hopping-leg testbed and validate the estimator against it, confirming an accurate boundary detector. The second contribution is empirical, and no less valuable for being negative: across four increasingly targeted testbeds — two single-parameter locomotion abstractions, a third where reward is provably independent of a second control axis while the margin is not, and a fourth removing failure penalties entirely — BM-RL shows no significant advantage over an unconstrained baseline in any condition, including two built to favour it. An accurate margin does not imply a useful one: reward maximization already disfavours the bifurcated regime through the reward function shape itself, in every testbed available. We report all four results as obtained and treat this persistent null as the paper's central finding, relocating the open question from whether reward and bifurcation risk can diverge (yes, provably) to whether a dense bifurcation signal is actually exploited once available. We release the estimator, testbeds, and code.

Keywords:

reinforcement learning, bifurcation theory, Floquet multipliers, legged locomotion, nonlinear dynamics, Poincaré maps
