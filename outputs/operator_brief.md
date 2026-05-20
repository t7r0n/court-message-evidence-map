# Operator Brief: Dispute Buddy

Dispute Buddy gets a local, deterministic pressure test around people, preparing, and text-message. The useful part is not the dashboard; it is the repeatable evidence path from fixture to failure to operator action.

## Highest-leverage checks

- people evidence replay -> block release until cited evidence is regenerated (people_coverage, evidence ev_0000).
- court operator packet -> accept only if decision claims cite fixture evidence (preparing_risk, evidence ev_0055).
- text-message regression harness -> open a regression issue with trace and benchmark delta (text-message_precision, evidence ev_0022).
- preparing boundary probe -> route to reviewer with evidence packet (court_latency, evidence ev_0077).

## What makes this useful

The workflow is intentionally local and deterministic. A reviewer can run the same fixture set, inspect the evidence IDs, open the dashboard, and see exactly why a recommendation passed, went to review, or blocked.
