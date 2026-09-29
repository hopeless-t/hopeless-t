# Projects

This page is a curated index of public work. It intentionally favors projects that are inspectable, reproducible, or useful as concrete engineering evidence.

## Verification & agent systems

### [NazeYatta](https://github.com/hopeless-t/NazeYatta)

**Problem**  
Automation can collapse “not verified” into “probably fine,” or blur the boundary between checking an action and authorizing it.

**Built**  
A small CLI for bounded preflight checks and exact post-action verification, with explicit `UNKNOWN`, `MISSING`, `STALE`, and `VERIFIED` states and reproducible receipts.

**Evidence**  
The repository includes runnable examples, schemas, tests, and package installation instructions.

---

### [ChatGPT Conversation Refresh PoC](https://github.com/hopeless-t/chatgpt-refresh-poc)

**Problem**  
A mobile conversation view can become stale even when newer server-side state exists.

**Built**  
A Swift proof-of-concept that models refresh as read-only reconciliation rather than regeneration, sending, or conversation creation.

**Evidence**  
The repository contains the behavior contract, a SwiftUI example, and acceptance tests covering revision updates, stale-state no-ops, identity mismatch, and preservation of local-only UI state.

## Systems research

### [Finite RAM Lab](https://github.com/hopeless-t/finite-ram-lab)

**Question**  
When physical memory is constrained, how well does observed residency align with future application demand?

**Method**  
Controlled Linux memory-pressure experiments with explicit acceptance criteria, independent validation runs, randomized trials, negative-result recording, and evidence-preserving analysis.

**Current value**  
The project is less about proposing a memory-management mechanism than about measuring when a real information gap exists and how much intervention headroom that gap leaves.

## Experimental research

### [Memory Attention Lab](https://github.com/hopeless-t/memory-attention-lab)

Independent reproducibility and systems research around attention value construction, accelerator residency, offloading, and reconstructable attention state.

### [Topological Spin Lab](https://github.com/hopeless-t/topological-spin-lab)

A small computational-physics lab for reproducing and exploring qualitative topological and spin-dependent electronic behavior on ordinary hardware.

### [Finite Tool Surface Lab](https://github.com/hopeless-t/finite-tool-surface-lab)

A reproducible research lab studying how much tool surface an AI worker should see, separating tool availability, visibility, retrieval quality, selection quality, and end-to-end task success.

## Selection rule

Projects appear here because they provide public, inspectable artifacts. Private work is intentionally not used as primary evidence on this profile.
