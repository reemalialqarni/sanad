# Responsible AI Use

## 1. Accuracy

AI-generated flows, copy, classifications, and recommendations are treated as drafts. Status language must reflect the real conceptual state: a similarity signal is a **possible match**, not confirmation that an item was found or belongs to a traveler.

## 2. Accountability

The trainee is responsible for the final portfolio. In the proposed service, authorized airport employees remain responsible for reviewing evidence and approving item release. An AI score cannot be used as the sole basis for ownership or handover.

## 3. Confidentiality

No real passenger, airport, or organizational information is included. Protected ownership evidence, such as hidden contents or unique marks, must not be exposed in public results, match previews, notifications, or screenshots.

## 4. Privacy

The service should collect only information needed to report, match, verify, and recover an item. General descriptors must be separated from private evidence. Production design would require approved retention, access, deletion, consent, and audit rules; these are `[Not Specified]` in this concept.

## 5. Bias

Ownership confidence must not depend on nationality, language, age, appearance, name, travel class, or device type. The provisional persona must not be treated as representative of every traveler. Arabic and English support is a design requirement, while broader language needs require research.

## 6. Human Oversight

AI may structure descriptions, flag missing fields, and rank possible matches. Humans define policy, review exceptions, decide whether evidence is sufficient, approve release, and handle appeals or disputed cases.

## Information Classification

| Information | Classification | Handling rule |
|---|---|---|
| Published service name and generic description | Green | May appear publicly. |
| General item descriptors such as category and broad color | Green | May support matching, but should still be displayed cautiously. |
| Approximate time and airport area | Amber | Use for matching; restrict unnecessary exposure. |
| Contact email or phone number | Amber | Limit access to authorized service functions and staff. |
| Full name linked to a report | Amber | Do not display to other users. |
| Government ID, passport, or boarding-pass details | Red | Do not place in prompts or public repositories; production handling requires approved secure controls. |
| Hidden contents, serial number, or unique ownership mark | Red | Store as protected proof; never reveal in match previews. |
| Employee-only match notes or AI confidence indicators | Red | Restrict to authorized review and audit. |

## Prompt Safety Checklist

- Use synthetic or anonymized examples only.
- Remove names, contact details, document numbers, and identifiers.
- Do not upload found-item photographs containing personal documents.
- Ask AI to mark uncertainty and missing information.
- Review for invented policy, research, deadlines, and outcomes.
- Keep AI-generated match suggestions provisional.
- Record human decisions and material corrections.

## Production Safeguards Required

- Access control and role separation.
- Encryption and secure evidence storage.
- Defined retention and deletion rules.
- Audit logs for employee access and release decisions.
- Rate limits and abuse monitoring.
- A dispute and escalation process.
- Security, legal, privacy, and accessibility review.
- Testing with real travelers and airport employees.

These safeguards are requirements for future validation, not claims about an implemented system.

