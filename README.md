[![CI](https://github.com/TodoPR/niche-factory/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/TodoPR/niche-factory/actions/workflows/ci.yml)

# niche-factory

Zero-variable-cost software factory monorepo scaffold.

This repository hosts the automation skeleton for the **Niche Software Factory** project.
It follows a static-first architecture and a CI/CD pipeline that targets **Cloudflare Pages (Free)** with GitHub Actions on public repositories.

## Directory layout
apps/ # App and site workspaces (added later)
packages/ # Shared libraries/components
infra/ # IaC and deployment files (minimal on Cloudflare Pages)

sql
Copy code

## Next steps
- S06: Repo templates (`AGENTS.md`), PR template, CODEOWNERS; branch protection.
- S07: CI skeleton (lint/test/build).
- S08: Security scans (CodeQL + dep audit).

## Governance
Keep this repo **public** so GitHub Actions stay free. See project Governance for details.

## License
MIT — see `LICENSE`.
