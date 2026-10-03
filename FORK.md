# Why this fork exists

This repository is SHIVAM ITCS's pinned fork of
[CopilotKit/CopilotKit](https://github.com/CopilotKit/CopilotKit).
`NOTICE.md` records the legal provenance — the upstream commit, the upstream
license, and exactly what we changed. This document records the *engineering
rationale*: why the fork exists at all, and what it demonstrates.

## The rationale

CopilotKit is the reference implementation of **agent-native frontends** —
generative UI, shared state between the model and the app, and human-in-the-loop
workflows. That is precisely the layer SHIVAM ITCS builds on top of when we ship
agentic systems into production for clients.

We fork it for one reason: **a stable, debranded reference pin we control.**
Upstream moves fast, and "latest main" is not a defensible answer when a client
asks which version of the frontend stack their deployed copilot is actually
running against. Pinning a known-good commit gives us a fixed point to reason
about, to reproduce against, and to upgrade from deliberately — rather than
being dragged along by a moving target.

## What this fork proves

- **Pinned-source intake.** We can take a large, real open-source monorepo,
  pin it to an exact upstream commit (`e8d096b9`, monorepo v1.74.0), strip build
  artifacts and local environments, and stand up a clean, reproducible tree.
- **Licence and attribution discipline.** MIT terms, upstream copyright, and
  the `Atai Barkai` notice are preserved verbatim. Branding is applied without
  editing upstream source or misrepresenting authorship.
- **A working baseline for the agent-native stack.** The tree is the genuine,
  unmodified upstream — the same code clients would get — which makes it a
  trustworthy starting point for the React/Angular/Vue/React Native copilot
  surfaces we integrate.

## What this fork is NOT

- **Not affiliated with or endorsed by CopilotKit or Atai Barkai.** "SHIVAM
  ITCS" branding here identifies the fork's maintainer, not the upstream project.
- **Not a redistribution product.** This is an internal reference pin, published
  transparently rather than hidden.
- **Not a claim over upstream authorship.** Every line of upstream source remains
  upstream's work under upstream's licence. See `NOTICE.md` and `LICENSE`.

## Upstream

- Repository: https://github.com/CopilotKit/CopilotKit
- Pinned commit: `e8d096b94352` — *chore: release monorepo v1.74.0 (#7460)*
- Committed: 2026-09-25 16:36:39 -0700

---

**SHIVAM ITCS** — 18+ years of .NET Core, Azure and agentic AI systems.
Web: https://shivamitcs.in · Contact: MD@ShivamITConsultancy.com
