# Allen Matrix Professional Dashboard V2.1

Static read-only publication of the Allen Matrix Professional Dashboard V2.1.

- Main entry: `index.html` (V2.1)
- V2.1 dashboard: `professional_allen_dashboard_v21.html`
- V2 alias: `professional_allen_dashboard_v2.html`
- V1 alias/current: `professional_allen_dashboard_v1.html`
- Explainable dashboard: `explainable_allen_dashboard.html`
- Per-asset sheets: `explainable_sheets/`
- V2.1 audit: `dashboard_v21_per_asset_visual_audit.csv`
- V2.1 visual errors: `dashboard_v21_visual_errors_by_asset.csv`
- V2.1 validation: `dashboard_v21_visual_sanity_validation.csv`

V2.1 adds per-asset chart scale sanity, NOT_AVAILABLE visual mode, OPERATIVE_VIEW/FULL_VIEW, and protection against out-of-scale levels flattening charts such as SI / Plata.

Policy preserved from generated dashboard:

- `shadow_only = true`
- `dashboard_calculates_signals = false`
- `dashboard_modifies_data = false`
- `production_signals_modified = false`
- `production_weights_modified = false`
- `automatic_trading = false`
- `classic_predictor_replaced = false`
- `neural_promotion = false`

This repository contains static HTML only. It does not call external APIs, does not fetch market data, and does not place or modify trades.
