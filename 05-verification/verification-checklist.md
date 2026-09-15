# Verification Checklist

## Personal Verification Protocol

Before accepting an AI-assisted UX output, I will:

1. **Identify the claims:** Separate facts, assumptions, recommendations, and generated examples.
2. **Trace the source:** Confirm every project-specific fact against the supplied scenario or approved documentation.
3. **Flag missing information:** Replace invented owners, dates, policies, results, and research findings with `[Not Specified]` or an explicit assumption.
4. **Test safety and privacy:** Check whether the output exposes personal data, protected ownership evidence, or an unsafe shortcut.
5. **Check user-state accuracy:** Ensure interface language matches the actual system state, especially "possible," "under review," and "confirmed."
6. **Check inclusion and clarity:** Review language, accessibility assumptions, tone, and potential stereotypes.
7. **Confirm decision ownership:** Verify that AI advice does not replace an authorized human decision.
8. **Document the outcome:** Record what was checked, what changed, and who approved the final version.

## Applied Verification Example

### Output reviewed

The first AI-generated possible-match notification from the writing workflow:

> Great news! We found your lost bag. Verify your identity now to claim it.

### Verification record

| Check | Finding | Decision or correction |
|---|---|---|
| Claims | "We found your lost bag" converts a similarity signal into a confirmed fact. | Changed to "possible match." |
| Source trace | No source confirms that the item belongs to Noura. | Removed the ownership claim. |
| Missing information | Identity-verification policy and release steps are not provided. | Avoided describing an unconfirmed identity process. |
| Privacy | The message itself reveals no item detail, but the next screen could. | Added a requirement not to show protected details. |
| User-state accuracy | The actual state is "potential match awaiting ownership answers and employee review." | Rewrote the status and next step. |
| Inclusion and clarity | "Claim it" is abrupt and may imply immediate release. | Replaced with a calm explanation. |
| Decision ownership | The original copy suggests successful self-service verification. | Added airport employee review. |
| Documentation | Changes and reasoning are recorded here and in Section 02. | Approved for conceptual prototype. |

## Verified Final Output

### Possible match found

> We found a report with details similar to your lost item. Answer a few private questions so an airport employee can review the match.

## Verification Result

The original output failed factual-accuracy, state-accuracy, and accountability checks. After revision, the message correctly communicates uncertainty, preserves human review, and gives the user a clear next action without revealing sensitive details.

## Evidence Limitation

This verification confirms consistency with the conceptual project documentation only. It does not verify real airport policy, legal compliance, technical security, or production accessibility.

