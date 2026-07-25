# Product overview

## The problem

Recreating a working web interface in Figma usually means taking a screenshot and manually rebuilding the design. That loses editable structure, makes long pages expensive to reproduce, and gives no reliable way to know whether the reconstruction is faithful.

## The Atlas approach

Atlas treats a website as a rendered system rather than a flat image:

1. Capture the live browser state.
2. Understand visible structure, text, controls, media, icons, and layout.
3. Generate editable Figma layers.
4. Render the Figma result.
5. Compare it with the browser reference.
6. Accept, diagnose, retry, or withhold the result.

The goal is not to support every website immediately. The goal is to become exceptionally reliable for structured web applications, then expand coverage deliberately.

## Design principles

- Fidelity before blind import.
- Editable structure before screenshot flattening.
- Safe failure before misleading output.
- Small resumable workloads before uncontrolled crawls.
- Figma as the delivery surface, not the long-running job manager.
