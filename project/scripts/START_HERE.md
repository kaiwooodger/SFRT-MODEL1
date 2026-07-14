# Start Here

This directory contains the main reproducibility entry points for the PMB revision package.

Use this short path:

1. Read `SCRIPT_MAP.md`.
2. Run `bash project/scripts/reproduce_manuscript.sh --mode public`.
3. Inspect:
   - `project/public_results/`
   - `figures/manuscript_clean/`
   - `manuscript/SFRT_Submission.pdf`

## Two execution modes

- `public`
  - Validates the bundled manuscript-facing result tables and frozen headline numbers.
  - Does not require TOPAS.

- `full`
  - Uses the top-level wrappers to call the preserved full implementation.
  - Requires TOPAS and Geant4.

## Provenance note

The original implementation scripts are preserved in `project/scripts/internal_legacy/`.
They retain their historical names so the scientific workflow remains runnable, but the
top-level entry points and manuscript-facing results use descriptive naming.
