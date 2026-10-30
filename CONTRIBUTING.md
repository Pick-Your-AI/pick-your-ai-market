# Contributing market research

Follow the [organization contribution rules](https://github.com/Pick-Your-AI/.github/blob/main/CONTRIBUTING.md), this guide and the current issue/Project instructions.

## Before starting

1. Search this repository, [Project #2](https://github.com/orgs/Pick-Your-AI/projects/2) and the [existing Research market program](https://github.com/Pick-Your-AI/pick-your-ai-research/issues/47) for overlapping work. Record a short prior-work note.
2. Keep existing work in its original issue and repository unless a transfer has been explicitly agreed. Do not duplicate issues to populate the new repository.
3. Confirm scope with the current assignee. Preserve Project statuses, priorities, workstreams and dependency relationships; this repository does not redefine Project #2's fields.

## Prepare a submission

- Use a focused branch and pull request. Explain the research question, method, evidence, limitations, decision requested and any affected consumer.
- Prefer primary sources. Record access dates and version, region, currency and units where relevant. Separate vendor claims, published measurements, independent measurements and estimates.
- Keep incomplete findings as notes. Do not fabricate required fields or promote synthetic examples into real evidence.
- Keep credentials, personal/customer content, raw datasets, model weights and large evidence downloads out of Git. Use source links and evidence manifests for external artifacts.
- Technical schemas and pricebooks remain governed by the Research repository. Propose contract changes through [Research #40](https://github.com/Pick-Your-AI/pick-your-ai-research/issues/40); do not copy and independently modify the frozen v1 contract here.
- Research does not authorize customer outreach, paid services, scraping beyond permitted access, deployment or spending.

## Review and validation

Before requesting review, run `git diff --check`, inspect Markdown rendering, verify local links and check that source citations support the stated claims. Report exactly what was checked and any access or evidence limitations. There is no research-validation program or CI workflow installed in this initial documentation-only repository.

Request independent review under the organization rules. Link related work with `Refs`; use `Closes` only after the issue's acceptance criteria and receiving handoffs are actually complete. Creating a document, merging a PR or closing an issue does not establish measured product capabilities.

## Routing decisions

For an unresolved decision, first read the existing issue, its assignees, relevant
decision record and related pull requests. Preserve accepted ownership and local
review, evidence, security and release requirements. Routing identifies a contact;
it does not grant access, appoint an owner, authorize publication or waive a gate.

Use the canonical [escalation guide](https://github.com/Pick-Your-AI/.github/blob/main/docs/governance/ESCALATION.md) and
[versioned routing policy](https://github.com/Pick-Your-AI/.github/blob/main/governance/escalation-policy.json). These links depend on the organization
governance change merging; until then, use its reviewed checkout and describe the
route as provisional. Do not claim the central tooling is installed or active.

The order is repository team → repository maintainer → repository lead maintainer
→ applicable parent teams → CompleteDotTech. Record a disposition at each level,
including unresolved, vacant, pending-acceptance or inaccessible roles; membership,
team-management status and repository permissions do not establish accepted
operational ownership. Keep owner placeholders for the final fallback. Do not
silently skip an unresolved role or treat a proposed mapping as accepted.

An operator with read access must refresh the private snapshot before resolving:

```sh
python /path/to/org-checkout/governance/router.py refresh --policy /path/to/org-checkout/governance/escalation-policy.json --snapshot /private/path/routing-snapshot.json --status /private/path/routing-status.json
python /path/to/org-checkout/governance/router.py resolve --policy /path/to/org-checkout/governance/escalation-policy.json --snapshot /private/path/routing-snapshot.json --repo Pick-Your-AI/pick-your-ai-market --max-age-seconds 86400 --status /private/path/routing-status.json
```

Here `86400` is an **operator-selected example**, not an approved default. Select
an appropriate explicit maximum age; a proposed policy value does not supply one.
Check that refresh succeeded. If refresh fails, stop recipient selection and
report the failure; the last successful snapshot is retained for diagnosis, not
as a current route. Report stale or incomplete coverage explicitly. Keep snapshots,
raw API responses, rosters and private
identities outside public Git and public issues. Share only the necessary public
team destination and a sanitized decision summary.

When escalation is needed, include the decision needed, current responsible role,
prior disposition and proposed next recipient. Reuse information already in the
issue or PR; routine contributions need no full escalation history. Send nothing
and change no assignment automatically. Keep sensitive information out of public
issues. This routing guidance establishes no new or verified private intake.
Follow any separately verified repository security policy; without a verified
private destination, do not submit confidential material.
