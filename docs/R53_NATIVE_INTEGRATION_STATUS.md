# SEMITS Health V524 R5.3 — Native Integration

Status: local development package built and tested; **GitHub source upload is not yet complete**.

## Main-window integration
- Original V524 application at `/platform/` is the default entry point.
- R5 Product Search, Food Diary, Activity Log, Live Dashboard and illustrative Meal Planner are native sidebar pages rendered into the original V524 `#main` element (not an iframe).
- R5 food/activity data uses existing local Python API and SQLite data.
- Original V524 browser profiles and medical records are NOT migrated or merged with R5 SQLite.

## Local verification
- 32 automated tests passed on 2026-11-17.
- Windows device end-to-end testing still pending.
- No private SQLite database included in the release ZIP.

## Source layout target
- `platform/` original V524 UI with native R5 sections
- `app.py` local Python backend
- `integration/` planning bridge
- `tests/` regression and native integration tests
- `reference_sql/` non-running PostgreSQL references

Do not merge this branch into main until the complete R5.3 source is uploaded, the Windows user test is complete, and storage boundaries are reviewed.
