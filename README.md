# Court Message Evidence Map

A local evidence map that ingests synthetic SMS/WhatsApp exports, clusters incidents, cites every claim to message IDs, detects coercive-pattern evidence, and emits a lawyer-ready review packet.

![Court Message Evidence Map working dashboard](outputs/project_working.svg)

## Why it exists

people preparing text-message evidence for court need trauma-aware evidence selection, chain-of-custody clarity, and lawyer-reviewable summaries without hallucinated claims.

The project is intentionally built as a local replay harness instead of a slide. It creates fixtures, plants realistic failure modes, produces citation-locked evidence, and turns the result into a dashboard a reviewer can inspect without credentials or hosted services.

## What is inside

- Deterministic fixture generation for the company-specific risk surface.
- Strategy code in `src/court_message_evidence_map/strategy.py` with project-specific scoring and visual evidence.
- Citation-locked reports where every decision claim points to a generated evidence ID.
- Two regenerated visual artifacts: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, benchmark, and test artifacts.

![Court Message Evidence Map evidence map](outputs/evidence_map.svg)

## Signals it measures

- `people coverage`
- `preparing risk`
- `text-message precision`
- `court latency`

## Failure modes it plants

- people drift
- preparing gap
- text-message misroute
- court blindspot

## Run it locally

```bash
uv sync
uv run court-message-evidence-map all
uv run pytest -q
uv run ruff check .
```

## Outputs worth opening

- `outputs/dashboard.html`
- `outputs/project_working.svg`
- `outputs/evidence_map.svg`
- `outputs/operator_brief.md`
- `outputs/decision_report.md`
- `outputs/strategy_model.json`
- `outputs/demo_pack.zip`

## Boundary

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.
