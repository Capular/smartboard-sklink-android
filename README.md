# SchoolX Smartboard Public Releases

This repository is the public update feed for SchoolX Smartboard PC.

## Purpose

- Host Velopack release artifacts (`*.nupkg`, setup exe, release manifests)
- Provide update metadata consumed by installed Smartboard clients
- Keep installer/update distribution public without exposing private source code

## Repositories

- Private source code: https://github.com/Capular/smartboard-schoolx-pc
- Public releases/feed: https://github.com/Capular/smartboard-schoolx-pc-public

## Notes

- New app versions are built from the private source repository and published here via CI release workflow.
- Smartboard clients check this repository feed before app startup.

