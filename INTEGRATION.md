# embedded-tls integration branch

This branch is embedded-tls `main` with changes that upstream has not merged yet. Each tag, named `integration-` and a date, marks one state of the branch. The branch is rebuilt on each new `main`. A project that builds on it must pin a tag or a commit, not the branch.

## Base

embedded-tls `main` at `0557076`, committed to `main` on 2026-11-12.

## Changes on top, in order

| Change | Commits |
|---|---|
| Move to embassy `da5e85fe5`, so that embedded-tls links with embassy-crypto drivers written against current embassy | 1 |

## Using it

embassy-crypto declares `links`, so a build holds one copy of it. Every embassy-crypto crate in the build, such as a driver crate, must name the same embassy commit as this branch: `da5e85fe5d3945d27a0d2066458d0fa3460c8d87`.
