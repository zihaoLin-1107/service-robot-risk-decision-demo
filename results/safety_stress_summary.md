# Safety Stress Summary

The safety override stress test asks whether hard safety remains protected when the cost model underestimates risk or over-rewards direct handover.

## Tempting Direct-Handover Stress Test

| Variant | Hard Safety Violation | Unsafe Continue | Prevented Unsafe Selection |
|---|---:|---:|---:|
| `no_safety_override` | 1.0 | 1.0 | 0 |
| `full_policy` | 0 | 0.395 | 1.0 |

## Interpretation

Safety override is not mainly an average-performance booster. It is a fail-safe layer that prevents hard-infeasible actions when the cost model is misspecified.

The remaining unsafe continuation under the full policy reflects soft risk and preference calibration limits; it is not a hard safety violation.
