# ReMeSo

💐 Why did we create ReMeSo?
=============================

Ad hoc agents accumulate instructions as they go, and things get messy, fast. What if there was a sane convention for organizing an Agent's identity? ReMeSo is a convention which helps specify Agents by their **Re**mit, **Me**mory, and **So**ul.

💐💐 Who benefits from ReMeSo?
=============================

People creating agents who want them to be repeatable, accountable and dependable.

💐💐💐 What does ReMeSo do?
=============================

ReMeSo is a convention for defining repeatable agent archetypes.

Each archetype has three files:

- **REMIT.md:** responsibilities, expected work and what the agent ought to delegate.
- **MEMORY.md:** a rewritable, palimpsest-y cache of proximate context and recent learnings. It changes frequently.
- **SOUL.md:** perspective and disposition, including longer-lived learnings or epiphanies that shape judgment.

### Examples

- [Security engineer](examples/security-engineer/SOUL.md): [REMIT](examples/security-engineer/REMIT.md), [MEMORY](examples/security-engineer/MEMORY.md).
- [Sandy Metz inspired OO consultant](examples/oo-consultant/SOUL.md): [REMIT](examples/oo-consultant/REMIT.md), [MEMORY](examples/oo-consultant/MEMORY.md).

The distinction should be concrete. A security engineer habitually looks for seams, attack surfaces and ways to break assumptions: that perspective belongs in SOUL. Hardening the system is the job in REMIT. Immediate investigation context belongs in MEMORY.

An object-oriented design consultant inspired by Sandy Metz brings opinionated object-oriented engineering values: that perspective belongs in SOUL. Consulting on and improving the system's object-oriented design is the job in REMIT. Circumstances may call for practical compromises; the perspective need not prescribe the same answer every time.

These are inspired archetypes, not statements authored by Sandy Metz or quotations attributed to her. The example MEMORY files are blank; no actual learning or private context is invented.


💐💐💐💐 How do I use ReMeSo?
=============================

ReMeSo is a convention, not software. Conceptually, organize each agent definition as:

```text
agents/<agent-name>/
  REMIT.md
  MEMORY.md
  SOUL.md
```

The human-facing explanation is this README. [ReMeSo.md](ReMeSo.md) contains the agent instructions for the convention. The project's root AGENTS.md is a thin pointer to that file and, as needed, the agent definitions. For example:

```text
In this house we use ReMeSo; see remeso/ReMeSo.md for further instructions.
```

`remeso/` is a conceptual example: use the actual relative path in each project. Changing an existing project's paths remains undecided; this draft does not authorize relocation. No mandatory skill, software package or universal loader is prescribed.

The README-level HOW is settled. Further lifecycle questions belong in ReMeSo.md: memory-refresh triggers, edit authority, verification and interaction with agent lifecycle mechanics remain open.

💐💐💐💐💐 Extras
=============================

### A note on the name

As the old joke goes, the two hardest problems in computer science are cache invalidation, naming things, and off-by-one errors. We evolved our way to "Remit", "Memory", and "Soul" as the core componentes, but couldn't think of a good name. Good thing I recently showing the kids *The Sound of Music*, so Julie Andrews’ re–me–so was top-of-mind—and, happily, a semantically empty handle matching REMIT, MEMORY, SOUL.

(Feel free to sing it.)

