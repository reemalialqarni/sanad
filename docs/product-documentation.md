# Sanad Product Documentation

## Document Status

- **Type:** Conceptual MVP documentation
- **Domain:** Airport lost and found
- **Evidence level:** Synthetic training scenario; not validated production research
- **Decision owner:** Human product and operational stakeholders

## Primary User

Noura Alotaibi is a fictional 32-year-old domestic traveler. After boarding, she realizes that she may have left a small black bag near airport security. She cannot return to the area and needs to report and track the loss remotely.

### User goal

Submit a credible report quickly, know that it reached the responsible service, follow its status, and recover the item without exposing sensitive information.

### Needs supported by the scenario

- Remote report submission.
- Acceptance of approximate time and location.
- A reference number and visible status.
- Clear next steps.
- Protection of ownership evidence.
- A route for recovery after leaving the airport.

### Assumptions to validate

- Travelers prefer a guided form over phone contact.
- Approximate time and area provide useful matching signals.
- Users understand the difference between a possible and confirmed match.
- Pickup and shipping are the relevant recovery options.

## Actors

| Actor | Responsibility |
|---|---|
| Traveler | Submits and tracks a report; provides private ownership evidence. |
| Finder | Hands the item to an authorized airport channel; direct traveler contact is outside MVP. |
| Lost-and-found employee | Registers found items, reviews possible matches, verifies evidence, and approves or rejects release. |
| AI-assisted matching service | Structures descriptions and ranks possible matches; does not decide ownership. |

## Core Lost-Item Flow

1. Traveler starts a lost-item report.
2. Traveler identifies airport, approximate area, date, and time.
3. Traveler adds general item descriptors.
4. Traveler separately provides protected ownership evidence.
5. Traveler reviews privacy guidance and submits.
6. System issues a reference number and "Search active" status.
7. Matching service identifies a possible match.
8. Traveler receives a notification without protected found-item details.
9. Traveler answers private ownership questions.
10. Employee reviews evidence and approves, rejects, or requests more information.
11. Approved traveler receives available recovery options.
12. Employee confirms handover and closes the case.

## Report States

| State | Meaning | User-facing requirement |
|---|---|---|
| Draft | Report is incomplete and not submitted. | Explain missing fields and preserve progress where possible. |
| Submitted | Report was received. | Show reference number and next step. |
| Search active | No confirmed match exists. | Avoid implying failure; explain that monitoring continues. |
| Possible match | Similarity was detected. | State uncertainty and request protected verification. |
| Awaiting employee review | User submitted answers. | Explain that a person is reviewing the case. |
| More information needed | Evidence is insufficient. | Explain what can be added without revealing the expected answer. |
| Approved | Employee accepted the ownership claim. | Show only approved recovery options. |
| Rejected | Evidence did not support the claim. | Provide an escalation or correction route subject to policy. |
| Ready for recovery | Item is approved and prepared for handover. | State location, requirements, and timing only when confirmed. |
| Closed | Item was recovered or case was closed. | Show reason and support route when applicable. |

## AI-Supported Functions

- Extract category, color, material, time, and location from free text.
- Ask for clarification when critical information is missing.
- Rank possible matches using permitted descriptors.
- Support employee review with an explainable comparison summary.

## Prohibited Autonomous Decisions

- Confirming that an item belongs to a traveler.
- Rejecting a claim without an approved human-review path.
- Releasing an item.
- Revealing another person's identity or contact data.
- Displaying protected ownership evidence.
- Creating policy, service-level promises, or legal requirements.

## Conceptual Data Separation

| Data group | Examples | Visibility |
|---|---|---|
| General descriptors | Category, broad color, material | Matching service and limited user display |
| Context signals | Airport, approximate area, date, time | Matching service and authorized staff |
| Protected evidence | Hidden contents, serial number, unique damage | Authorized verification only |
| Personal contact | Name, email, phone | Authorized service communication only |
| Decision record | Employee decision, reason, handover record | Authorized staff and audit function |

## Accessibility and Content Principles

- Support Arabic and English layouts.
- Use plain language and one primary action per state.
- Do not rely on color alone to communicate status.
- Provide labels and text alternatives for meaningful images.
- Keep error messages specific and recoverable.
- Preserve user input after correctable errors.
- Use uncertainty language consistently.

No claim of accessibility compliance is made without a measured interface audit and user testing.

## Conceptual Success Measures

- Report completion rate.
- Percentage of reports requiring clarification.
- Time from submission to first meaningful status update.
- Rate of verified matches.
- Incorrect-release incidents.
- User comprehension of "possible match" versus "confirmed."
- Employee time required per reviewed case.
- User-reported confidence in privacy and status clarity.

Targets are intentionally not invented; they require baseline evidence and stakeholder approval.

## Open Decisions

- Approved verification and identity requirements.
- Data retention and deletion periods.
- Employee roles and access permissions.
- Service-level commitments.
- Shipping eligibility and payment responsibility.
- Dispute, appeal, and fraud-handling procedures.
- Integration with airport and airline systems.

