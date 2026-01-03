# Versioned Snapshots & Reproducible Outputs
**Generated:** 2026-01-03

## Goal
Ensure that figures/tables do not change mid-semester and that you can reproduce any semester’s materials.

## Recommended Strategy
1. **Semester release tags** in GitHub:
   - Example: `v2026-spring`, `v2026-fall`
2. Store generated assets under a dated snapshot folder:
   - `snapshots/2026-01-03/figures/`
   - `snapshots/2026-01-03/data/`
3. Keep notebooks as the “compiler,” and commit outputs for students.

## Minimal Workflow
- Run instructor notebooks
- Copy outputs:
  - `figures/slide_ready/` → `snapshots/2026-01-03/figures/`
  - `data/*.csv` and `data/assets_manifest.json` → `snapshots/2026-01-03/data/`
- Tag a GitHub release for the semester

## Optional: Checksums
Create checksums so you can verify no file drift:
- `sha256sum snapshots/2026-01-03/figures/* > snapshots/2026-01-03/FIGURES_SHA256.txt`
- `sha256sum snapshots/2026-01-03/data/* > snapshots/2026-01-03/DATA_SHA256.txt`
