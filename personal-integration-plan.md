# Personal AI Integration Plan

## Goal

Use generative AI as a structured design assistant while keeping evidence, privacy decisions, prioritization, and final approval under human control.

## Task 1 - Organize Discovery Notes

- **Recurring task:** Turn stakeholder notes, workshop outputs, or interview notes into structured themes and action items.
- **Expected benefit:** Reduce manual sorting time and make missing decisions visible earlier.
- **Preferred prompt/workflow:** Input -> C.A.R.E. prompt -> AI synthesis -> source comparison -> human correction -> final brief.
- **Main risk or verification requirement:** The model may invent an owner, deadline, consensus, or research theme. Every statement must be traced to the source; unknowns are marked `[Not Specified]`.
- **Frequency:** After every discovery meeting or research session.
- **Success looks like:** The final brief contains no unsupported facts, separates evidence from assumptions, and can be reviewed quickly by stakeholders.

## Task 2 - Draft and Refine UX Copy

- **Recurring task:** Produce first drafts of status messages, instructions, confirmations, empty states, and errors.
- **Expected benefit:** Generate consistent alternatives quickly and adapt tone for stressful user situations.
- **Preferred prompt/workflow:** State definition -> R.C.T.O. prompt -> draft variants -> fact and state verification -> accessibility and tone review -> human sign-off.
- **Main risk or verification requirement:** Copy may overpromise, hide uncertainty, use an incorrect system state, or describe an unsupported policy. Check every claim and action against the approved flow.
- **Frequency:** During each prototype iteration and before handoff.
- **Success looks like:** Users can understand what happened, what has not yet happened, and what they should do next without misleading reassurance.

## Task 3 - Review Flows and Prototype Specifications

- **Recurring task:** Check a proposed flow for missing states, privacy exposure, inconsistent decisions, and weak recovery paths.
- **Expected benefit:** Expand review coverage and reveal questions before stakeholder or developer handoff.
- **Preferred prompt/workflow:** Provide the approved scope and screen specification -> structured audit prompt -> severity list -> human validation -> tracked revisions.
- **Main risk or verification requirement:** AI may claim compliance without sufficient visual, policy, or technical evidence. Treat all findings as review prompts, not proof of compliance.
- **Frequency:** At the end of each design phase and before handoff.
- **Success looks like:** Critical states and dependencies are documented, high-risk gaps are resolved or escalated, and the final decision log identifies the human approver.

## 30-Day Adoption Plan

| Period | Action | Evidence of progress |
|---|---|---|
| Week 1 | Save the three approved prompt templates and use them on synthetic practice material. | Three reviewed outputs with corrections recorded. |
| Week 2 | Apply the writing workflow to five interface states. | Draft, verification, refinement, and sign-off shown for each. |
| Week 3 | Use the audit workflow on one complete prototype journey. | Severity log and revised flow. |
| Week 4 | Review quality, time saved, recurring errors, and unsafe suggestions. | Short retrospective and updated prompt versions. |

## Personal Rule

> AI accelerates preparation and review; it does not create evidence, approve risk, or own the final design decision.

