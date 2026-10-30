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
