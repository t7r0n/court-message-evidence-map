# Court Message Evidence Map

A local evidence map that ingests synthetic SMS/WhatsApp exports, clusters incidents, cites every claim to message IDs, detects coercive-pattern evidence, and emits a lawyer-ready review packet.

## Why This Exists

people preparing text-message evidence for court need trauma-aware evidence selection, chain-of-custody clarity, and lawyer-reviewable summaries without hallucinated claims.

## What It Builds

- Replays synthetic `people` and `preparing` cases against the project's evidence rules.
- Scores `people_coverage`, `preparing_risk`, and `text-message_precision` so regressions are visible in CSV and JSON.
- Plants `people drift` and `preparing gap` failures as negative controls.
- Writes citation-locked decision claims; unsupported claims fail verification.
- Exports a review dashboard and demo pack for `court-message-evidence-map` without hosted services.

## Local Run

```bash
uv sync
uv run court-message-evidence-map all
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/analysis.json`
- `outputs/scenario_report.csv`
- `outputs/decision_report.md`
- `outputs/evidence_packet.md`
- `outputs/dashboard.html`
- `outputs/demo_pack.zip`

## Sources

- https://www.disputebuddy.co/
- https://www.disputebuddy.co/our-story
- https://www.trustpilot.com/review/disputebuddy.co

## Boundary

This repository uses synthetic fixtures only. It has no credentials, no customer data, no outreach data, and no dependency on a hosted API.
