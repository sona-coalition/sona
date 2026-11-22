# Sona working practices

**English** | [Español](./README.es.md)

*How an organisation manages activity on its sonas, stated in the vocabulary of [Sona](../README.md). Independent of any tool or implementation — for one realisation, see the coalition's GitHub work standard; the correspondence lives in the mapping document.*

*Terminology (sona#8, 2026-11-17): the concepts are now **activity** (formerly "work"), **agent** (formerly "entity"), and **jichi** (computational agent). This document's title and path keep the older word for now — renaming them is a separate decision, because other repositories link here.*

## Organisations and activity

An **organisation** is a collection of agents. Being a collection, an organisation is itself an agent — and like any agent it has a personal sona (the collection that is wholly its own) and may have further sonas for the projects it is working on. All members of an organisation are curators of its personal sona.

Activity is a change an organisation manages deliberately, and it comes in two kinds:

* **Internal activity** modifies one of the organisation's sonas.
* **External activity** changes something outside them — the wider environment, other sonas, other agents.

A **task** represents an item of internal or external activity.

## The two approvals

These practices exist to guarantee two acts:

1. **Proposal approval.** Before the activity starts, the proposal is reviewed and accepted — by an agent **other than the proposer**.
2. **Activity approval.** Before the result changes the sona (or the external thing), the activity is reviewed and accepted — by an agent **other than the one who did it**.

Everything else is mechanism. An approval given by the proposer is not an approval, only a click.

## Task states and their guards

A task passes through the states `Draft`, `Proposed`, `Accepted`, `Assigned`, `InReview`, `Done`. States are not gates that constrain movement; each state carries a **guard** — what should be true while a task is in it — checked at review. Before changing a task's state, check the guard of the state you are moving it to.

| State | Guard — what should be true while a task is here | Why the state exists |
| --- | --- | --- |
| `Draft` | The task exists but does not yet specify the activity effectively; "done" may still be unclear. | A place to refine ideas without exposing them as planned activity. |
| `Proposed` | The task fully describes the activity, including what "done" means. The proposer requests **proposal approval**. | The queue for the first approval. |
| `Accepted` | Proposal approved by an agent other than the proposer; the approval is recorded. | Approved activity waiting for capacity. |
| `Assigned` | The task has an assigned contributor, who has begun or is about to begin. | Activity in progress. |
| `InReview` | The assignee judges the activity complete and offers evidence. Awaiting **activity approval** by an agent other than the assignee. | The queue for the second approval. |
| `Done` | Activity approved and accepted; the sona (or the external thing) reflects it. | The record of accepted activity. |

Old tasks in `Done` are archived periodically so current views stay clean; tasks that will not be done are archived with the reason recorded. Deletion is reserved for tasks created in error or as tests, and only while in `Draft`.

Decisions the organisation makes collectively are executed by a curator, because only curators hold the power to change the sona. A team review — periodic, or continuous for a small organisation — is where reviews of proposals and of activity happen; what matters is that every approval is real and the record shows where it happened.

## Principles

1. Every contribution is associated with at least one task.
2. A proposal is accepted only after review by an agent other than the proposer.
3. A contribution is accepted only after review by an agent other than the contributor.
4. Tasks are transitory: anything that must persist must not live solely within a task.
5. The state of every task is recorded, and visible to the whole organisation.

An implementation of these practices (for example, the GitHub work standard) derives its own rules from these principles; the mapping document shows the derivation.
