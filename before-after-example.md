# Before and After: Improving a Design Prompt

## Workplace Task

Create the first version of Sanad's lost-item reporting flow.

## Before - Weak Prompt

```text
Design an airport lost-and-found app.
```

## Initial Result

The initial response suggested generic screens such as login, home, report item, search, chat, notifications, and profile. It did not define the traveler scenario, protect ownership evidence, distinguish a possible match from a confirmed item, or identify where employee review was required.

## After - C.A.R.E.-Structured Prompt

```text
Context: Sanad is a conceptual airport lost-and-found service. The primary user is a traveler who realizes after boarding that she left a small bag near security and cannot return to the airport. The service must protect personal data and private ownership evidence. AI may rank possible matches, but it cannot confirm ownership or release an item.

Action: Design the MVP user flow from starting a lost-item report to case closure. Include approximate location and time, general description, private proof details, report tracking, no-match state, possible-match notification, ownership questions, employee review, and pickup or future shipping. Include recovery paths for missing information and failed verification.

Role: Act as a senior UX/Product Designer specializing in service design, privacy, and high-stress journeys.

Expected output: Provide no more than ten primary user steps in a table with user action, system response, data sensitivity, error/recovery state, and human decision point. Clearly label assumptions and do not invent airport policy.
```

## Improved Result

| Step | User action | System response | Privacy or recovery control | Human oversight |
|---|---|---|---|---|
| 1 | Start a lost-item report | Explains the process and expected information | No account required before understanding the process | None |
| 2 | Select airport, approximate area, date, and time | Flags missing required information | Approximate values are accepted when memory is uncertain | None |
| 3 | Describe the item | Structures category, color, material, and general features | General descriptors are separated from private proof | None |
| 4 | Add private ownership evidence | Stores hidden details such as contents or unique marks | Evidence is never displayed in potential-match previews | None |
| 5 | Review and submit | Shows exactly what will be submitted | User can edit before submission | None |
| 6 | Track report | Displays reference number and current status | Clear no-match and search-active states | Employee can add a case note |
| 7 | Receive a possible-match notice | States that similarity is not confirmation | No finder identity or full found-item description is shown | None |
| 8 | Answer verification questions | Compares answers with protected evidence | Failed answers can be reviewed or retried according to policy | Employee reviews exceptions |
| 9 | Await employee review | Shows review status and expected next update | AI score is not exposed as proof of ownership | Employee approves or rejects the claim |
| 10 | Arrange recovery and close case | Presents approved recovery options | Release follows verified airport procedure | Employee confirms handover |

## What Improved

1. The scenario became specific enough to produce a coherent journey rather than a generic feature list.
2. Privacy controls were embedded in the flow instead of added at the end.
3. The output separated AI-supported matching from the human decision to release an item.
4. The requested table made gaps, assumptions, failure states, and accountability visible.

## Human Decision

The improved flow is accepted only as an MVP hypothesis. Airport policy, identity checks, service-level expectations, accessibility, and recovery options remain subject to stakeholder validation and real user testing.

