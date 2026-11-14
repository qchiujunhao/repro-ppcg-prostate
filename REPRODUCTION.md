# Reproduction attempt: "Evolutionary trajectory and momentum shape prostate cancer outcomes" (PPCG)

Deposit: Zenodo 10.5281/zenodo.22706046 (ppcg-evolution.zip, 1.4 MB), downloaded 2026-11-14.

## Outcome: not reproducible from the public deposit

Nothing was run, because nothing in the deposit can be run as published:

1. **No figure source data.** `scripts/reproduce_figures.R` regenerates every panel from
   `figures_data/*_source_data.{tsv,rds}`. The deposit contains no `figures_data/` directory;
   `data/` holds only `data/ext/cytoBand_hg19.txt` (32 KB). The README points reviewers to a
   private figshare link for the source data. That link is not part of the deposit and was not used.
2. **Patient-level data are access-controlled** (PPCG, Hartwig, HEROIC via EGA), so the analysis
   scripts under `scripts/0*_*/` cannot run either.
3. **The pinned environment is Linux-only.** `envs/ppevo.yaml` pins `linux-64` conda builds
   (R 4.2.2 plus Bioconductor); it cannot be created on macOS as written.
4. **Two companion code releases live on GitFront**, outside the archive.

What the deposit does deliver: the complete code, a panel-to-script table, and an exact package list.
A reader with the figshare files and a Linux machine could follow steps 1, 3 and 4 of the README.

No whatran record exists for this directory because no command produced a result.
