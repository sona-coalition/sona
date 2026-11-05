# Sona working practices

*How an organisation manages work on its sonas, stated in the vocabulary of [Sona](./README.md). Independent of any tool or implementation — for one realisation, see the coalition's GitHub work standard; the correspondence lives in the mapping document.*

## Organisations and work

An **organisation** is a collection of entities. Being a collection, an organisation is itself an entity — and like any entity it has a personal sona (the collection that is wholly its own) and may have further sonas for the projects it is working on. All members of an organisation are curators of its personal sona.

Work is a change an organisation manages deliberately, and it comes in two kinds:

* **Internal work** modifies one of the organisation's sonas.
* **External work** changes something outside them — the wider environment, other sonas, other entities.

A **task** represents an item of internal or external work.

## The two approvals

These practices exist to guarantee two acts:

1. **Proposal approval.** Before work starts, the proposal is reviewed and accepted — by an entity **other than the proposer**.
2. **Work approval.** Before the result changes the sona (or the external thing), the work is reviewed and accepted — by an entity **other than the one who did it**.

Everything else is mechanism. An approval given by the proposer is not an approval, only a click.

## Task states and their guards

A task passes through the states `Draft`, `Proposed`, `Accepted`, `Assigned`, `InReview`, `Done`. States are not gates that constrain movement; each state carries a **guard** — what should be true while a task is in it — checked at review. Before changing a task's state, check the guard of the state you are moving it to.

| State | Guard — what should be true while a task is here | Why the state exists |
| --- | --- | --- |
| `Draft` | The task exists but does not yet specify the work effectively; "done" may still be unclear. | A place to refine ideas without exposing them as planned work. |
| `Proposed` | The task fully describes the work, including what "done" means. The proposer requests **proposal approval**. | The queue for the first approval. |
| `Accepted` | Proposal approved by an entity other than the proposer; the approval is recorded. | Approved work waiting for capacity. |
| `Assigned` | The task has an assigned contributor, who has begun or is about to begin. | Work in progress. |
| `InReview` | The assignee judges the work complete and offers evidence. Awaiting **work approval** by an entity other than the assignee. | The queue for the second approval. |
| `Done` | Work approved and accepted; the sona (or the external thing) reflects it. | The record of accepted work. |

Old tasks in `Done` are archived periodically so current views stay clean; tasks that will not be done are archived with the reason recorded. Deletion is reserved for tasks created in error or as tests, and only while in `Draft`.

Decisions the organisation makes collectively are executed by a curator, because only curators hold the power to change the sona. A team review — periodic, or continuous for a small organisation — is where reviews of proposals and of work happen; what matters is that every approval is real and the record shows where it happened.

## Principles

1. Every contribution is associated with at least one task.
2. A proposal is accepted only after review by an entity other than the proposer.
3. A contribution is accepted only after review by an entity other than the contributor.
4. Tasks are transitory: anything that must persist must not live solely within a task.
5. The state of every task is recorded, and visible to the whole organisation.

An implementation of these practices (for example, the GitHub work standard) derives its own rules from these principles; the mapping document shows the derivation.
