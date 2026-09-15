# Sanad UX Case Study

## Summary

Sanad explores how an airport lost-and-found service could become a clear, trackable, and privacy-aware digital journey. The case study focuses on a traveler who discovers a loss after leaving the relevant airport area and must continue remotely.

## The Problem

Losing an item in an airport creates more than a search problem. The traveler may not know which organization owns the process, what details are needed, whether the report was received, or how ownership will be verified. A service that reveals too much about found items can also enable fraudulent claims.

## Design Question

> How might we enable a traveler to report, track, and prove ownership of a lost item after leaving the airport, while protecting personal information and sensitive item details?

## Provisional Persona

### Noura Alotaibi

- **Age:** 32
- **Context:** Domestic traveler who notices after boarding that a small black bag may have been left near airport security.
- **Goal:** Submit a report remotely and understand what happens next.
- **Primary need:** Confidence that the case reached the right service and can be tracked.
- **Main concern:** Another person may use visible item details to make a false claim.

Noura is a fictional design hypothesis, not a research participant.

## Current-State Journey Hypothesis

| Stage | User action | Likely experience | Design opportunity |
|---|---|---|---|
| Realize loss | Tries to remember where the item was left. | Stress and incomplete recall. | Accept approximate context and guide memory. |
| Find help | Searches for the responsible contact. | Unclear ownership across airport, airline, and security. | Provide one entry point and route internally. |
| Report | Repeats the description through different channels. | Effort, inconsistency, and no structured record. | Create one structured report with a reference number. |
| Wait | Calls or checks repeatedly. | No visible status or expectation. | Provide meaningful states and notifications. |
| Prove ownership | Describes private details to different people. | Privacy risk and uncertainty. | Capture protected evidence separately. |
| Recover | May need to return without confirmation. | Time and travel cost. | Confirm approval before presenting recovery options. |

This journey is a hypothesis and requires real research.

## Key Design Principles

1. **One visible journey:** A single case reference connects reporting, matching, review, and recovery.
2. **Reveal less, verify more:** Match previews disclose minimal information; private evidence supports employee review.
3. **Uncertainty must be explicit:** "Possible match" is never presented as "item found."
4. **Human release decision:** AI supports comparison; an authorized employee approves handover.
5. **Recovery from errors:** Users can correct approximate details and respond when evidence is insufficient.
6. **Design for stress:** Short steps, clear status, preserved input, and direct language reduce cognitive load.

## Proposed Experience

### Report

The traveler provides approximate context, general descriptors, and protected proof in separate steps. The review screen explains which details support matching and which remain hidden.

### Track

A reference number and status timeline replace repeated calls. Each state explains what has happened, what has not happened, and the next expected action.

### Match

The system compares permitted descriptors and identifies possible matches. The traveler does not see full found-item details or finder information.

### Verify

The traveler answers questions derived from protected evidence. An airport employee reviews the comparison and decides whether more information is needed.

### Recover

Only after approval does the service show confirmed recovery options. Handover and closure remain recorded human actions.

## Example UX Copy

**Possible match found**

> We found a report with details similar to your lost item. Answer a few private questions so an airport employee can review the match.

**Search still active**

> No matching item has been confirmed yet. Your report remains active, and we will notify you if its status changes.

## Responsible AI Position

Generative AI was used to structure prompts, draft copy, reorganize synthetic notes, and check for gaps. It was not used to create fake research evidence or make an ownership decision. Every output in this portfolio was reviewed against the supplied scenario, and unsupported details were removed or labeled `[Not Specified]`.

## Limitations

- No real passengers or airport employees were interviewed.
- No production airport policy was supplied.
- No live matching model was implemented or evaluated.
- No legal, security, or accessibility certification was conducted.
- Metrics have no targets because no baseline data exists.

## Next Steps

1. Conduct research with travelers and lost-and-found employees.
2. Map actual airport, airline, security, and vendor responsibilities.
3. Validate data classification and verification policy.
4. Prototype the bilingual reporting and review flows.
5. Test comprehension, accessibility, and false-claim resistance.
6. Define measurable targets only after baseline evidence is available.

