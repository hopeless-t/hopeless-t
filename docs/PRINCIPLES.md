# Engineering Principles

These are working engineering principles, not universal laws. They are useful because they make boundaries explicit and testable.

## Evidence != Authority

Evidence can support a decision.

It does not, by itself, grant permission to act.

A verification component should not silently become an authorization component.

## Proposal != Decision

A component may be able to express a proposal without owning the authority to approve or execute it.

Expressibility and executability are different capabilities.

## UNKNOWN stays UNKNOWN

Missing or stale evidence should not be silently upgraded into confidence.

When a required fact has not been established, the system should preserve that uncertainty explicitly.

## Observation before intervention

Before introducing a mechanism intended to improve a system, measure the existing system closely enough to show that the claimed gap is real.

This reduces the risk of “solving” an assumed problem.

## Execution != Verification

The component that performs an action should not be the only component allowed to declare the action successful.

Where practical, expected postconditions should be checked against a fresh observation.

## Negative results are results

A falsified hypothesis narrows the design space.

A result should not disappear because it makes a preferred mechanism less attractive.

## Bounded systems are easier to inspect

Small contracts, narrow tool surfaces, explicit state transitions, deterministic guards, and reproducible receipts make agent-assisted systems easier to debug and review.

## Claims should point to artifacts

A public engineering claim is stronger when another person can follow it to code, tests, experiment records, or other inspectable evidence.
