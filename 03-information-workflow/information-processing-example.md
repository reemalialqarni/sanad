# Information Processing Workflow

## Purpose

This example demonstrates **summarizing, extracting, synthesizing, restructuring, and prioritizing**. All notes are synthetic and created for training; they are not real research findings or airport records.

## Input - Synthetic Messy Notes

```text
Traveler may notice the loss after boarding or after arriving in another city. Team thinks airport and approximate area should be required, but exact time may be hard to remember. Someone suggested showing photos of found items; privacy concern because another person could copy visible details. Need Arabic and English. Operations wants a case number. We do not know the response-time commitment yet. AI could match color, category, time, location, and description, but it must not release an item. Traveler should know whether the report is submitted, searching, under review, or closed. Maybe pickup and shipping; shipping policy is not confirmed. Security team asked where private proof such as bag contents will be stored. No owner was assigned to confirm the identity-check process. Prototype review is next Thursday. Noura scenario: black small bag left near security, noticed after boarding.
```

## Prompt Used

```text
Act as a senior UX researcher and product discovery facilitator. Transform the supplied notes into a decision-ready brief for Sanad. Separate confirmed scenario details, design hypotheses, constraints, risks, open questions, and action items. Do not invent owners, policies, deadlines, research evidence, or service levels. Mark missing information as [Not Specified]. Prioritize issues by user harm and delivery dependency. End with the three decisions needed before the next prototype review.
```

## AI Output - First Pass

> Sanad should allow travelers to report a lost item remotely and track it with a case number. The flow should support Arabic and English, accept approximate location and time, and use AI to identify possible matches. Sensitive proof should be hidden. Shipping and response times require confirmation.

### First-pass action items

| Action | Owner | Deadline | Priority | Status |
|---|---|---|---|---|
| Define ownership verification | Security team | Next Thursday | High | Open |
| Confirm shipping policy | Operations | Next Thursday | Medium | Open |
| Design bilingual reporting flow | Design team | Next Thursday | High | In progress |

## Human Review of the AI Output

The first pass was useful but introduced three unsupported details:

1. It assigned the ownership-verification task to the security team, although the notes explicitly say no owner was assigned.
2. It treated next Thursday as the deadline for all tasks, while it is only the prototype-review date.
3. It marked design work as "In progress" without evidence.

These fields were corrected to `[Not Specified]`. The notes were also restructured so confirmed scenario details were separated from design hypotheses.

## Final Structured Output

### Executive summary

Sanad addresses the lack of a clear remote journey for travelers who discover a lost item after leaving the airport. The proposed experience should capture approximate loss details, issue a trackable case number, protect private ownership evidence, and communicate case states clearly. AI may propose possible matches using non-sensitive descriptors, while an authorized employee makes the ownership and release decision. Shipping, service-time commitments, evidence storage, and identity-check procedures remain unresolved.

### Findings

| Type | Finding | Priority | Rationale |
|---|---|---|---|
| Scenario fact | Noura notices after boarding that a small black bag was left near security. | High | Defines the primary remote-reporting scenario. |
| User need | The traveler needs confirmation that the report was submitted and can be tracked. | High | Reduces uncertainty after leaving the airport. |
| Design hypothesis | Approximate time and area should be accepted when exact details are unavailable. | High | Requires validation with users and operations. |
| Constraint | Arabic and English must be supported. | High | Essential for the proposed airport context. |
| Privacy risk | Showing full photos or distinguishing details may enable false ownership claims. | Critical | Can expose protected evidence. |
| Governance rule | AI may suggest a match but cannot approve item release. | Critical | Preserves human accountability. |
| Open question | Storage and access rules for private ownership evidence. | Critical | Blocks a safe data model. |
| Open question | Identity and ownership-verification procedure. | Critical | Blocks a trustworthy handover flow. |
| Open question | Shipping availability and policy. | Medium | Affects recovery options after approval. |
| Open question | Response-time commitment. | Medium | Affects user expectations and status copy. |

### Action items

| Action item | Owner | Deadline | Priority | Status |
|---|---|---|---|---|
| Define approved ownership and identity checks | [Not Specified] | [Not Specified] | Critical | Open |
| Define storage, retention, and access rules for private evidence | [Not Specified] | [Not Specified] | Critical | Open |
| Validate which item details may appear in a possible-match notice | [Not Specified] | [Not Specified] | High | Open |
| Design the bilingual report and status flow | UX/Product Designer | Prototype review: next Thursday | High | Planned |
| Confirm whether shipping is supported | [Not Specified] | [Not Specified] | Medium | Open |
| Confirm service-level and response-time language | [Not Specified] | [Not Specified] | Medium | Open |

### Decisions needed before prototype review

1. Which information is a general descriptor and which is protected ownership evidence?
2. What human review is mandatory before a match can be approved?
3. Which recovery option can be represented in the first prototype without implying an unconfirmed policy?

