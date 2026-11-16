# Agent Instructions

Before starting any task in this repository:

1. Run `make agents/sync`. It writes the shared Plus3 IT instructions for this repository's tardigrade-ci version to `.agents/plus3it/AGENTS.md`.
2. Read `.agents/plus3it/AGENTS.md` and follow it together with this file. If the sync fails, tell the user, and don't guess the conventions.

These rules always apply, even without the shared instructions:

- Don't push, open pull requests, publish releases, or apply infrastructure changes unless the user asks. List those steps for a person in your final report.
- Don't edit files under `.agents/plus3it/`; they are generated and overwritten by the sync.

@.agents/plus3it/AGENTS.md

## Repository-specific

### Purpose

This Terraform module creates one AWS KMS key and one alias for each entry in the `keys` list. The main input is `keys`, a list of objects where `alias` is required and `description`, `deletion_window_in_days`, `policy`, and `enable_key_rotation` are optional; the code defaults are 30 days for deletion and no key rotation. The module outputs `keys`, a map of alias to the KMS key resource.
