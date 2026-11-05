<!-- markdownlint-disable -->

# Hardening Report: matrix-org--pr-details-action/v1.3

> This file was generated automatically by the hardening agent.

**Policy SHA:** `d636be7e43ef829af6e853da6b3c7566db9f72fe`

**Test Policy SHA:** `843adf9e4b8f85d0c08b27b9d0b09dd094b54702`

**Harden Agent Version:** `2`

Action **matrix-org--pr-details-action/v1.3** was hardened automatically. 1 finding(s) were identified and resolved across 1 iteration(s).

## Findings Fixed

### unpinned-uses (severity: high)

action.yml uses an unpinned action reference: `uses: actions/github-script@v6`. Pin it to a full 40-character commit SHA.

Locations:

- `action.yml:29`

## Iteration Notes

### Iteration 1

**Fixes applied:** unpinned-uses

**Notes:**

Pinned actions/github-script@v6 to d7906e4ad0b1822421a7e6a35d5ca353c962f410 # v6 in action.yml. Inputs already pass through env, so no other changes were needed.

