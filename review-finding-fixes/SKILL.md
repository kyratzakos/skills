---
name: review-finding-fixes
description: >
  Fixes one written code-review finding at a time and updates the review document when that
  finding is done. Use when the user points at a review document, asks to work through review
  findings, or says to hand a finding back when it is unclear or conflicts with the docs.
disable-model-invocation: true
---

# Review finding fixes

Work from a written review. One finding per turn.

## Rules

- Work on one issue at a time.
- Update the review document when that issue is done.
- If something is unclear or does not comply with the docs or what you already know about this system, hand it back instead of changing code blindly.

## Before editing

1. Read the finding the user named. If they did not name one, take the next open finding in the review's existing order. Stop after that one.
2. Read the code the finding cites and the project docs that describe that behavior.
3. Hand the finding back, and do not edit code, when any of these are true:
   - The suggested fix conflicts with a project doc.
   - More than one behavior would satisfy the finding, and the docs do not pick one.
   - Applying it would change a documented money, status, or persistence rule the finding does not explicitly override.
4. Say what the doc requires, what the finding suggests, and the choice you need. Wait.

## After the user chooses

Implement only that finding. Do not start the next one.

If the change replaces behavior a project doc describes, update that doc in the same pass so the next finding is checked against the new rule.

## When the finding is done

Update the review document:

- Mark that finding fixed, with the date and what changed.
- Remove it from any still-open list and from the merge-blocking triage if those sections exist.
- Leave every other finding as it was.

## Hand-back

State the conflict in a few sentences, then the options. Do not include a partial implementation.

Finding: treat every non-`RJCT` status as accepted. Project doc: any status other than `RJCT` is approved, and names a code the finding would reject. Stop. Ask which map to implement. Do not edit the parser or mark the finding fixed.
