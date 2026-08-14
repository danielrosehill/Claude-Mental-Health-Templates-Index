# Claude Mental Health Templates Index

[![Master Index](https://img.shields.io/badge/Master_Index-GitHub-blue?style=flat-square&logo=github)](https://github.com/danielrosehill/Github-Master-Index)

[![Index Repo](https://img.shields.io/badge/Type-Index_Repo-purple?style=flat-square)](https://github.com/danielrosehill/Subindices)

[![Claude Code Index](https://img.shields.io/badge/Parent-Claude_Code_Projects_Index-orange?style=flat-square&logo=github)](https://github.com/danielrosehill/Claude-Code-Projects-Index)

[![License](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg?style=flat-square)](https://creativecommons.org/licenses/by/4.0/)

Claude Code templates, plugins and workspaces for **mental health work that a person does on
their own material** — organising what happened, tracking a course of therapy, preparing for an
appointment, and keeping the background context that makes any of it repeatable.

A subindex of the [Claude Code Projects Index](https://github.com/danielrosehill/Claude-Code-Projects-Index).

**None of this is therapy, and none of it is clinical software.** Nothing here diagnoses,
assesses, scores or treats. What these tools do is organise, remember, write down and prepare —
see [SCOPE.md](SCOPE.md) for the boundary and why it is drawn where it is.

**Last Updated:** August 2026

---

## Working the material

Where the actual thinking happens.

| Project | Description | Links |
|---------|-------------|-------|
| **Claude-Therapy-Workspace-Template** | A GitHub template for working through **one bounded issue** — a career situation, one relationship, a bereavement. One workspace, one issue, with an ending. Ten workspace-local skills: capture a session, unpack an incident, build a chronology from raw material, re-read it through other lenses, review what recurs, draft the hard message, and produce a two-page handover for an appointment. `for-therapist/` is the deliverable the rest feeds | [![View Repository](https://img.shields.io/badge/View-Repository-blue?style=flat-square&logo=github)](https://github.com/danielrosehill/Claude-Therapy-Workspace-Template) |

## The context layer

Issue-scoped workspaces only work if you aren't re-explaining your life at the top of each one.

| Project | Description | Links |
|---------|-------------|-------|
| **Claude-Personal-Context-Plugin** | Builds and maintains a persistent background context layer — intake interview, ingestion of material you already have (journals, exports, old notes), gap analysis, scoped retrieval, maintenance and export. Ships the **Portable Context Contract**: entry schema, scopes, sensitivity levels, read/write protocols, backends and an export conformance test. Plain markdown in a store you own; model-managed memory is prohibited by the spec | [![View Repository](https://img.shields.io/badge/View-Repository-blue?style=flat-square&logo=github)](https://github.com/danielrosehill/Claude-Personal-Context-Plugin) |

## Tracking an ongoing course of therapy

The administrative half — you are in therapy, and the tooling keeps the paperwork.

| Project | Description | Links |
|---------|-------------|-------|
| **Therapy-Tracking-Plugin** | Pre- and post-session notes, goal tracking, and turning voice-memo transcripts into structured problem summaries, across an ongoing course of therapy. Data lives outside the plugin so it survives updates; git mode defaults to local-only and the onboarding skill never suggests a public repo | [![View Repository](https://img.shields.io/badge/View-Repository-blue?style=flat-square&logo=github)](https://github.com/danielrosehill/Therapy-Tracking-Plugin) |
| **Claude-Personal-Planning-Plugin** | General personal-planning workspaces — `log-entry` / `set-goal` / `review-progress` primitives across diary, health-wellness, personal-dev and therapy variants. The broad tool the two above are specialisations of | [![View Repository](https://img.shields.io/badge/View-Repository-blue?style=flat-square&logo=github)](https://github.com/danielrosehill/Claude-Personal-Planning-Plugin) |

---

## How they fit together

```text
  Claude-Personal-Context-Plugin          ← who you are. Written once, read by everything.
   store: ~/.claude-user-data/personal-context
                    │  scoped reads
     ┌──────────────┼──────────────┐
     ▼              ▼              ▼
  therapy        therapy        any other
  workspace      workspace      workspace
  (issue A)      (issue B)      implementing the contract
     │
     ▼
  for-therapist/ ─────────────────────►  a real appointment
                                              │
                                              ▼
                                    Therapy-Tracking-Plugin
                                    (the ongoing course, tracked)
```

Choosing between them:

- **Working on one thing?** → therapy workspace template. Bounded, closeable, produces documents.
- **In therapy and want the sessions tracked?** → Therapy-Tracking-Plugin.
- **Want general journaling and goals?** → Personal-Planning-Plugin.
- **Tired of re-explaining yourself?** → Personal-Context-Plugin. Everything else reads it.

## Common thread

| | |
|---|---|
| **Bounded, not general** | A workspace scoped to one issue can state what is out of scope, be reviewed in a sitting, and be closed. General "my mental health" repos accumulate until nobody opens them |
| **Portable context, not vendor memory** | Background context is plain markdown in a store the person owns, read through declared scopes. Every tool here is instructed not to use model-managed memory — it can't be exported, can't be scoped, and dies with the account |
| **Documents are the output** | The conversation is the means. What survives is a session note, a chronology, a thread, a brief — reviewable later, checkable against itself, usable by a professional, and readable when the tool that made it is gone |
| **The bridge, not the destination** | Access to support is rationed by cost, waiting lists, geography and language. The premise is that organised reflection is useful on its own *and* makes the professional hour materially better — so the highest-value output is a person walking into an appointment prepared |
| **Private by default** | Personal material never goes near a public remote. Provisioning scripts check remote visibility and refuse rather than warn |
| **No clinical apparatus** | No screening instruments, no severity scores, no diagnostic language, no assessment dressed up as structure. Describe, don't classify |

## Related, indexed elsewhere

Health-access and policy work is a different subject and lives in
[AI-Assisted-Policymaking-Index](https://github.com/danielrosehill/AI-Assisted-Policymaking-Index) —
including `Israel-ADHD-Medication-Access` and `Claude-ADHD-Research-Workspace`. Those are about
how a system does or doesn't deliver care; these are about doing your own work inside it.

## License

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
