# Network screening and visualization

Focused workflow for screening weighted interaction edges, calculating connectivity, identifying candidate hubs, and exporting network-ready node/edge tables. The portable runner is dependency-free and uses synthetic data; the original STRING-based R workflow is preserved under `src/legacy/`.

## Quick start

```bash
python workflow.py --input examples/input.csv --config config/workflow.json --output output
python -m unittest discover -s tests -v
```

The run produces audited CSV and SVG artifacts under `output/`. See `docs/STEP_BY_STEP.md` for the input contract and verification checklist.

For biological interpretation, record the interaction source and version, organism, identifier mapping, edge direction, confidence threshold, and background universe. Hub status alone is not evidence of causal importance.
