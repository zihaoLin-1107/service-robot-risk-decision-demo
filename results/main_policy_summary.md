# Main Policy Summary

The main decision-sandbox comparison evaluates three policies over the factorized service context.

| Policy | Action Correct | Unsafe Continue | Avg. Total Cost |
|---|---:|---:|---:|
| `fixed_policy` | 0.5515 | 0.1636 | 55.39 |
| `rule_based_policy` | 0.8061 | 0 | 26.65 |
| `risk_sensitive_policy` | 0.9818 | 0 | 18.57 |

## Interpretation

The fixed policy is a negative baseline because it tends to prioritize direct service completion. The rule-based policy handles simple labels but does not compare candidate actions through risk cost. The risk-sensitive policy chooses among service actions using context, risk cost, and hard safety constraints.

These are summary-level sandbox results, not real-world deployment results.
