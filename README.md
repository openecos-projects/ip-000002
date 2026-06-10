# ip-000002

Display name: APB4 Architecture Info Register Block

UID: ip-000002

Family: archinfo

Category: peripheral

Repository: git@github.com:openecos-projects/apb4-architecture-info-register-block.git

Upstream: https://github.com/oscc-ip/archinfo

Upstream author/maintainer: Beijing Institute of Open Source Chip / OSCC-IP

Current baseline: source snapshot from the `20250627` tapeout project

License: MulanPSL-2.0

Status: candidate, silicon-proven source snapshot

This repository is managed as a child repository of `ip-catalog`.

## Summary

This IP is an APB4-accessible architecture information register block. It
exposes system architecture metadata, tapeout/process identification, and
tapeout date information through three 32-bit APB4 registers.

The local repository contains a source mirror from the `20250627` tapeout
project for catalog evaluation. The current RTL baseline should be treated as
the tapeout project source snapshot rather than an automatically synchronized
upstream checkout.

## Layout

```text
rtl/       SystemVerilog RTL and required local common support modules
tb/        SystemVerilog testbench files
driver/    Minimal C software access example
docs/      Datasheet, test plan, checklist, and provenance notes
reports/   Review, lint, simulation, or synthesis report summaries
```

## Top Level

The integration top module is:

```text
apb4_archinfo
```

The top-level interface is an APB4 slave SystemVerilog interface:

```text
apb4_if.slave apb4
```

## Catalog Mapping

The corresponding catalog record is expected at:

```text
data/ip/peripheral/ip-000002.yaml
```

The local metadata source is:

```text
ip.yaml
```

## Review Notes

- Upstream repository: https://github.com/oscc-ip/archinfo
- Upstream default branch observed locally: `main`
- Current source snapshot comes from the `20250627` tapeout project code.
- IP status is recorded as silicon-proven based on the provided tapeout project provenance.
- The RTL uses local common support modules copied into `rtl/`.
- No local passing simulation, lint, synthesis, coverage, or silicon validation report artifact has been added yet.
