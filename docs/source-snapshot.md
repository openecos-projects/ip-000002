# Source Snapshot

This repository packages the `archinfo` IP as `ip-000002` for catalog review.

The source baseline is the `20250627` tapeout project code. The RTL in this
repository should be treated as a project source snapshot rather than an
automatically synchronized mirror of upstream `main`.

Observed upstream context from the local `new_ip/archinfo` checkout:

- Repository: `https://github.com/oscc-ip/archinfo`
- Branch: `main`
- Commit: `7add3752f8b7bed156a91ff727800aae1b98f608`
- Commit date: `2024-08-01 15:28:25 +0800`
- Commit subject: `feat: add driver and test codes`

The packaged RTL also includes the local common support modules required to
compile and simulate the IP standalone for catalog review.
