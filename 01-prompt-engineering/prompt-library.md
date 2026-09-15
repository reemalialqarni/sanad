# Prompt Library

## Purpose

This library contains seven reusable prompts for the Sanad UX/Product Design workflow. All prompts use either the **C.A.R.E.** framework (Context, Action, Role, Expected output) or **R.C.T.O.** (Role, Context, Task, Output).

## Prompt 1 - Turn Messy Notes into a Product Brief

- **Workplace task:** Information synthesis
- **Framework:** C.A.R.E.
- **When to use:** After an early stakeholder conversation when notes are incomplete and unstructured.

```text
Context: I am exploring Sanad, a conceptual lost-and-found service for airports. The source notes may contain confirmed details, assumptions, unresolved questions, and missing owners.

Action: Separate the notes into confirmed facts, assumptions, user needs, constraints, risks, open questions, decisions required, and action items. Do not add missing information. Mark every missing owner or deadline as [Not Specified].

Role: Act as a senior UX researcher and product discovery facilitator.

Expected output: Produce (1) a five-line executive summary, (2) a structured findings table, and (3) an action-item table with columns for action, owner, deadline, priority, and status. Add a final section titled "Items requiring human confirmation."
```

### Short sample output

> The main service gap is not only item discovery; it is the absence of a visible and trustworthy case journey after the traveler leaves the airport. Ownership evidence must be protected, and any AI-generated match must remain provisional until employee review.

## Prompt 2 - Define the Primary Persona Without Inventing Research

- **Workplace task:** Persona drafting
- **Framework:** R.C.T.O.
- **When to use:** To convert an explicitly fictional scenario into a documented design hypothesis.

```text
Role: Act as a UX researcher who clearly distinguishes evidence from assumptions.

Context: Sanad is a conceptual airport lost-and-found service. The only provided scenario is: Noura Alotaibi, age 32, is a domestic traveler who notices after boarding that she left a small black bag near airport security. She has already left the airport and needs a remote way to report and track the item.

Task: Create a provisional persona for design exploration. Use only the supplied facts. Put any reasonable but unverified design hypotheses in a separate section labeled "Assumptions to validate." Do not invent quotations, research statistics, disabilities, income, or technology preferences.

Output: Provide a concise persona with scenario, goal, needs, pain points, behaviors supported by the scenario, assumptions to validate, and design implications.
```

## Prompt 3 - Build a Privacy-Aware Lost-Item Flow

- **Workplace task:** User-flow design
- **Framework:** C.A.R.E.
- **When to use:** When defining the MVP journey.

```text
Context: Sanad helps an airport traveler report and recover a lost item. The user may have left the airport. General descriptors can support matching, but private ownership evidence must not be shown publicly. AI can suggest possible matches but cannot approve ownership or release an item.

Action: Propose an end-to-end user flow from starting a report to case closure. Include alternative paths for incomplete information, no match, potential match, failed verification, employee review, pickup, and future shipping.

Role: Act as a senior service designer specializing in trust, privacy, and high-stress digital journeys.

Expected output: Return a numbered flow. For each step include user action, system response, sensitive data involved, failure state, and point of human oversight. Keep the MVP within ten primary user steps.
```

## Prompt 4 - Generate Accessible UX Copy

- **Workplace task:** UX writing
- **Framework:** R.C.T.O.
- **When to use:** To draft clear status, error, and confirmation messages.

```text
Role: Act as a bilingual UX writer for a high-stress airport service.

Context: Users may be anxious, in transit, and using the service quickly. Copy must be calm, direct, and honest. Never imply that an item has been found when the system has only identified a possible match.

Task: Draft Arabic and English messages for: report submitted, information missing, no match yet, possible match, verification failed, employee review, ready for pickup, and case closed.

Output: Use a table with state, Arabic title, Arabic body, English title, English body, and primary CTA. Titles must be under six words and body copy under thirty words. Preserve the distinction between "possible match" and "confirmed item."
```

### Short sample output

| State | Title | Body | CTA |
|---|---|---|---|
| Possible match | Possible match found | We found a report with similar details. Answer a few private questions so an employee can review the match. | Continue verification |
| No match | Search still active | No matching item has been confirmed yet. Your report remains active, and we will notify you if its status changes. | View report |

## Prompt 5 - Evaluate Design Concepts with a Decision Matrix

- **Workplace task:** Structured evaluation
- **Framework:** C.A.R.E.
- **When to use:** When comparing alternative interaction concepts.

```text
Context: Three concepts are being considered for reporting a lost item: a conversational assistant, a guided step-by-step form, and a single long form. The experience must work under stress, protect sensitive details, support incomplete recall, and remain accessible.

Action: Evaluate the three concepts using the same criteria: clarity, completion effort, accessibility, privacy control, error prevention, multilingual suitability, and employee handoff. Explain uncertainty instead of inventing evidence.

Role: Act as a product design lead facilitating a concept review.

Expected output: Create an unweighted decision matrix using Low/Medium/High ratings, explain each rating in one sentence, list assumptions requiring usability testing, and provide a provisional recommendation for human review.
```

## Prompt 6 - Create a Usability-Test Script

- **Workplace task:** Research planning
- **Framework:** R.C.T.O.
- **When to use:** Before testing the reporting and verification prototype.

```text
Role: Act as a senior usability researcher.

Context: We need to test a prototype of Sanad's lost-item report and ownership-verification flow. The prototype uses fictional data and does not connect to a real airport. We must avoid leading questions and must not claim that the participant's data will be processed by a live service.

Task: Create a 25-minute moderated usability-test script covering task comprehension, report creation, distinction between general description and private evidence, status understanding, and response to a possible match.

Output: Include introduction and consent language, scenario, five neutral tasks, non-leading follow-up questions, observation fields, success criteria, and closing questions. Clearly label the prototype as conceptual.
```

## Prompt 7 - Audit a Screen Before Handoff

- **Workplace task:** Quality assurance
- **Framework:** C.A.R.E.
- **When to use:** Before design review or developer handoff.

```text
Context: I will provide a screen specification from Sanad. It may include labels, status language, actions, error handling, sensitive fields, and assumptions.

Action: Audit only the supplied specification for clarity, consistency, accessibility, privacy, recoverability, and alignment with the rule that AI suggests matches while employees approve release. Do not claim visual compliance if measurements or screenshots are unavailable.

Role: Act as a UX quality reviewer with experience in accessibility and privacy-sensitive services.

Expected output: Return four sections: verified strengths, issues, missing evidence, and recommended revisions. Assign Critical/High/Medium/Low severity and explain the reason. End with a human sign-off checklist.
```

## Human Review Note

These prompts are reusable starting points, not autonomous instructions. Their outputs must be checked against real project evidence, approved policies, accessibility requirements, and stakeholder decisions before use.

