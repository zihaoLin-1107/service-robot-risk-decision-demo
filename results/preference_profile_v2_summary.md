# Preference Profile v2 Summary

The preference calibration step uses 35 direct human labels to refine the service preference profile.

## Label Summary

| Preferred Action | Count |
|---|---:|
| `cautious_handover` | 11 |
| `place_nearby` | 10 |
| `safe_wait` | 9 |
| `direct_handover` | 0 |
| `abort_or_retreat` | 0 |

## Interpretation

The labels do not support an aggressive direct-handover profile. They also do not support unnecessary task abortion. The resulting interpretation is service-oriented but cautious: the robot should try to complete assistance when reasonable, but nearby placement and temporary waiting can be better than forced direct handover.

This is preliminary human preference calibration, not a formal user study.
