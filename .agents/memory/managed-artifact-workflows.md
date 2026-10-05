---
name: Artifact-owned workflows
description: Replit behavior when cleaning up generated artifacts and their managed workflows.
---

Replit-managed artifact workflows cannot be removed with the ordinary workflow-removal operation. Removing the generated artifact in this environment also removed its registered workflow.

**Why:** Artifact service workflows are coupled to registered artifacts rather than configured as standalone processes.

**How to apply:** When cleaning generated starter apps from this project, treat the artifact and its managed workflow as one unit instead of retrying workflow removal.