# Ticket / Spec template (Jira KAN)

Copy this into the **Jira ticket description** when creating work for the docs repo. The ticket is the single source of truth — no spec, no build. Add a **flowchart in a Jira comment** when the change touches multi-step flows or navigation.

**Label:** `repo-docs-pro` (required)

---

## User Story

Add the details of this issue from the user's POV.

---

## Acceptance Criteria

Include at least one **failure-case** scenario, not only the happy path.

1. **GIVEN** …
   **WHEN** …
   **THEN** …

2. **GIVEN** … (failure / edge case)
   **WHEN** …
   **THEN** …

---

## Tech Details

- Pages / MDX files affected
- `docs.json` navigation changes
- OpenAPI or code-sample updates
- Links to related aggregator/provider PRs if API docs change

---

## Money-safety

- Touches settlement / balances / order routing documentation in a way that could mislead integrators? **Yes / No**
- If **Yes**: second human reviewer required before prod; call out invariants and failure cases explicitly in the docs.
- Docs-only wording/clarity with no protocol impact: usually **No**.

---

## Notes / Assumptions

- Assumptions that must stay true for this change to remain correct.

---

## Open Questions

- …

---

## Bug tickets (shorter variant)

For **Bug** issue type, use at minimum:

**Describe the bug** — what is wrong (broken link, outdated API field, wrong example).

**To reproduce** — URL or steps.

**Expected** — what readers should see.

**Environment** — staging vs production docs, page path.

**Acceptance criteria** — **GIVEN / WHEN / THEN** for the fix, including one regression check.
