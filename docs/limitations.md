# Current Limitations

This public demo repository presents a PhD application research prototype, not a deployed service robot.

## Scope

- The decision experiments are run in a simplified decision sandbox.
- The Webots/RViz demonstration validates branch mapping, not full online deployment.
- The current robot execution does not include real grasping, object attachment/detachment, or MoveIt-based manipulation.

## Evaluation

- The oracle and risk weights are partly hand-designed.
- The human preference calibration uses 35 direct labels only.
- The labels are preliminary preference calibration, not a formal user study.
- Raw logs, raw labels, and detailed experiment traces are not included in this public repository.

## Learning and Adaptation

- The preference update is rule-based.
- No RL/PPO system has been trained.
- No LLM is used for decision making.
- Continuous belief state estimation is future work.

## Deployment Boundary

The current prototype supports research framing, decision logic evaluation, and branch-mapping validation. It should not be interpreted as a finished elderly-care or home-service deployment.
