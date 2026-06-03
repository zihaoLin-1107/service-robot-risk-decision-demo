# Public Research Claims

This public repository supports the following preliminary claims at the demo-prototype level.

## Claim 1: Factorized Context Modeling Clarifies the Decision Problem

The project models service context as `user_state + event_state + risk_state` rather than using a flat scenario label.

What can be claimed:

- The factorized formulation separates user intent, external disturbance, and environmental risk.
- It makes branch selection easier to inspect and explain.

What cannot be claimed:

- It is not yet a learned continuous belief model.
- It has not been validated in a formal human-subject study.

## Claim 2: Risk-Sensitive Policy Outperforms Fixed and Rule-Based Baselines in the Sandbox

Summary evidence:

- `fixed_policy`: action_correct = 0.5515, unsafe_continue = 0.1636, avg_total_cost = 55.39.
- `rule_based_policy`: action_correct = 0.8061, unsafe_continue = 0, avg_total_cost = 26.65.
- `risk_sensitive_policy`: action_correct = 0.9818, unsafe_continue = 0, avg_total_cost = 18.57.

What can be claimed:

- In the synthetic decision sandbox, the risk-sensitive policy performs better than fixed and simple rule-based baselines.

What cannot be claimed:

- This does not prove real-world deployment performance.

## Claim 3: Hard Safety Override Is a Fail-Safe

Summary evidence from a tempting direct-handover stress test:

- Without safety override: hard_safety_violation = 1.0, unsafe_continue = 1.0.
- With full policy: hard_safety_violation = 0, prevented_unsafe_selection = 1.0.

What can be claimed:

- Safety override prevents hard-infeasible choices under cost/reward misspecification.

What cannot be claimed:

- Safety override does not solve all soft social risk or all unsafe continuation risk.

## Claim 4: Human Preference Labels Motivate Service-Oriented Cautious Behavior

35 direct labels preferred:

- `cautious_handover`: 11.
- `place_nearby`: 10.
- `safe_wait`: 9.
- `direct_handover`: 0.
- `abort_or_retreat`: 0.

What can be claimed:

- Preliminary labels suggest service completion should not be defined only as direct handover.

What cannot be claimed:

- This is not a formal user study and does not establish population-level preference.
