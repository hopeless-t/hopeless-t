# Research Method

My public research repositories use a deliberately bounded workflow.

```text
Question
  ↓
Contract / hypothesis
  ↓
Measurement design
  ↓
Experiment
  ↓
Observation
  ↓
Acceptance / falsification
  ↓
Evidence
  ↓
Next bounded question
```

The point is not to force every project into one methodology. The point is to keep plans, executions, observations, and conclusions from collapsing into one another.

## What this means in practice

### Define the claim before the result

Experiments should have an explicit question, observable, and acceptance or falsification condition before a result is interpreted.

### Separate observation from intervention

A project should first establish what the current system does before introducing a mechanism that claims to improve it.

### Preserve negative findings

If a proposed mechanism does not produce the expected effect, that outcome remains part of the evidence.

### Use independent verification where possible

A completed program run is not automatically a successful experiment, deployment, or external action.

## Example: Finite RAM Lab

[Finite RAM Lab](https://github.com/hopeless-t/finite-ram-lab) studies memory pressure, residency, and future-demand mismatch.

The project has repeatedly moved from observation to controlled hypothesis testing rather than assuming that a proposed hint or intervention is beneficial. Negative and confirmatory results remain in the repository and constrain the next experiment.

This is the pattern I want from systems research:

```text
observe
  ↓
characterize
  ↓
reproduce
  ↓
form a narrow hypothesis
  ↓
intervene
  ↓
compare
```

## Example: ChatGPT Conversation Refresh PoC

[ChatGPT Conversation Refresh PoC](https://github.com/hopeless-t/chatgpt-refresh-poc) applies a similar discipline to product engineering.

```text
user-visible symptom
  ↓
behavior contract
  ↓
forbidden effects
  ↓
acceptance criteria
  ↓
minimal executable PoC
```

The implementation does not attempt to reverse-engineer private application internals. It models the intended semantics and makes them testable.

## Research boundary

I prefer narrow, reproducible claims over broad conclusions that outgrow the evidence.

Where a project is exploratory, its README should say so. Where a result is only a reference, qualification, or bounded experiment, it should not be promoted into a production claim without additional evidence.
