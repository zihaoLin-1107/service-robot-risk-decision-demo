# Case A: Webots/RViz Branch Mapping Demo

## Context

```text
user_state = requesting_water
event_state = none
risk_state = near_user_block
selected_action = cautious_handover
```

## What Appears in the Video

- Terminal output showing the selected action and branch mapping log.
- RViz visualization showing path, marker, target information, and branch validation.
- Webots scene showing the mobile manipulator executing the mapped service branch.

## What It Validates

- A high-level `selected_action` can be mapped to a robot execution branch.
- `cautious_handover` can be represented as a safer branch rather than a direct handover.
- The bridge can map service actions to navigation goals, arm pose sequences, waits, retreats, markers, and logs.

## What It Does Not Validate

- It is not full online deployment.
- It is not real grasping.
- It is not MoveIt manipulation.
- It is not a formal user study.
- It does not prove robust real-world safety.

## Video Link

TODO
