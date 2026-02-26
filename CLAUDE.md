# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is the documentation site for Seam AI, an AI-native account-based marketing (ABM) platform. It is built with [Mintlify](https://mintlify.com/) and deployed automatically when changes are pushed to `main`.

## Local Preview

To preview the docs locally, install the Mintlify CLI and run:

```bash
npm install -g mintlify
mintlify dev
```

There are no other build, lint, or test commands — this is a pure content repository.

## Architecture

- **`docs.json`** — Central configuration: navigation structure, theme, branding, navbar links. All pages must be registered here to appear in the sidebar.
- **`openapi.json`** — OpenAPI 3.1.0 spec for the Seam AI enrichment API (`/v1/chat/completions` with the `researcher` model).
- **`onboarding/`** — Linear getting-started flow: Setup → Configure → Orchestrate.
- **`guides/`** — Deep-dive reference docs organized by feature area (Data, Intelligence, Agents, Management).
- **`connections/`** — Integration setup guides, one file per integration (23 total).
- **`assets/`** — Logos, favicon, and images referenced in content.

## Key Conventions

- All content files use `.mdx` extension (MDX, not plain Markdown).
- When adding a new page, register it in `docs.json` under the appropriate tab/group, using the file path without the `.mdx` extension.
- Navigation order in `docs.json` controls the sidebar order exactly.
- Connection pages use `icon` fields (Mintlify icon names) on groups in `docs.json`.
- The primary brand color is `#4c810a` (Seam green).

## Seam AI Concepts (for accurate documentation)

- **Fit Score** — AI-generated A/B/C/D grade for accounts based on ICP criteria.
- **Intent Signals** — Buying signals from 1st-party (web pixel) and 3rd-party (Bombora) sources.
- **Audiences** — Dynamic account segments combining fit + intent.
- **Plays** — Automated multi-channel workflows triggered by audience/signal conditions.
- **Routing** — Queue management that assigns accounts to SDRs based on rules.
- **Credits** — Seam's consumption unit for AI enrichment operations.
