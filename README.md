# semicolab-registry

Central submission registry for SemiCoLab IP tiles.

## How submissions work

Submissions are created **automatically** by the precheck workflow in each
tile repository (see [semicolab-precheck](https://github.com/MifralTech/semicolab-precheck)),
right after a real, passing VeriFlow verification run. The submission issue
is opened with data read directly from that run's `results.json` — nothing
here is self-reported by the tile author.

If you need to open a submission manually (e.g. the automated step failed,
or you're submitting from a repo that doesn't use the standard precheck
workflow), use [Issues → New Issue](../../issues/new/choose) and fill in
the form — you'll need your tile repo's `results.json` from a passing run
to complete it.

## Requirements

- Connectivity check: ✅ PASS
- Simulation: ✅ PASS (if a testbench is provided)
- Synthesis: ✅ PASS
- Verified against the `semicolab` interface

## Status

Submissions are reviewed manually. You will be notified via the Issue when
your tile is approved and assigned a Tile ID.
