# Scope

What belongs in this index, what doesn't, and where the neighbouring ones start.

## In scope

Claude Code tooling — templates, plugins, workspaces, skills — for **mental health work a person
does on their own material**:

- Working through a bounded personal issue in writing
- Organising and tracking an ongoing course of therapy
- Preparing for an appointment with a professional
- Structuring reflection: journals, voice memos, chronologies, patterns over time
- The background context layer that lets scoped workspaces work without repetition

The common test: *does it help a person organise their own experience, in files they keep?*

## Out of scope

| Not here | Where |
| --- | --- |
| Health-access, medication-access and policy work | [AI-Assisted-Policymaking-Index](https://github.com/danielrosehill/AI-Assisted-Policymaking-Index) |
| Physical health tracking, medical records, care logs | Personal-admin repos; not indexed publicly |
| General journaling and life planning with no mental health framing | [Claude-Code-Projects-Index](https://github.com/danielrosehill/Claude-Code-Projects-Index) |
| Other people's mental health AI tools | A `*-Resources` repo, per the [Subindices](https://github.com/danielrosehill/Subindices) convention: `*-Index` repos index my own projects |
| Private repos | Deliberately absent — this index is public |

`Claude-Personal-Planning-Plugin` is a borderline case and is listed because its therapy and
health-wellness variants are the general form of two other entries here. Its diary and
house-search variants are not the reason it's included.

`Claude-Personal-Context-Plugin` is not mental-health-specific — it is a general context layer.
It's here because the therapy workspace template does not work without it, and because the
scoping and sensitivity design in the contract came out of this problem.

## The line this index does not cross

Nothing indexed here diagnoses, assesses, screens, scores or treats. No PHQ-9, no GAD-7, no
severity ratings, no risk assessment, no "this sounds like X".

That is not defensive hedging. A number produced by a tool with no clinical standing, carried
into an appointment, distorts the appointment — it primes a clinician with framing that didn't
come from a clinician, and it is very hard to walk back. Description is genuinely useful and
classification is not ours to do.

Anything that acquires an assessment instrument stops belonging in this index.

## Adding an entry

1. Confirm it is a Claude Code artefact, mine, public, and in scope above.
2. Add it to the right section of `README.md` in the existing table shape.
3. Update **Last Updated**.
4. If it's a new *kind* of thing, say why in the *How they fit together* section — the reason
   somebody would choose it over the neighbours is the useful part, not the description.
