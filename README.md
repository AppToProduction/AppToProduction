# Aaron — AI app production engineer

I turn fragile AI-built applications into reviewable production changes across
authorization, billing state, and release configuration.

**Open to fixed-scope rescue work and contract or full-time engineering roles.**

[Review selected work](#selected-work) ·
[See the Supabase rescue proof][rls-proof] ·
[Request a public fit check][fit-check]

> **Portfolio disclosure:** the projects below use synthetic fixtures and are
> reference implementations, not client engagements. Their value is in the
> executable tests, CI runs, source history, and explicit assurance boundaries.

## Selected work

| Project | Production problem | Evidence you can inspect |
| --- | --- | --- |
| [Lovable + Supabase RLS Rescue](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue) | An auth-only policy leaked another tenant's row; hardened reads and writes now require membership. | Postgres roles, SQL migrations, anon/Alice/Bob CRUD matrix, baseline-to-v1.1 comparison, CI, rollback notes. |
| [Billing Webhook + Entitlement Rescue](https://github.com/VJO-JavaScript/stripe-entitlements-rescue-reference) | Forged, duplicate, delayed, and out-of-order billing events can drift application access. | TypeScript signature guard, event-ID idempotency, authoritative reconciliation, dead-letter replay, tests and CI. |
| [Production Parity Gate](https://github.com/VJO-JavaScript/production-parity-gate) | Preview and production can silently diverge in environment contracts, callbacks, readiness paths, and client bundles. | TypeScript CLI and GitHub Action, React/Vite fixture, Markdown + JSON evidence, deterministic tests and CI. |

## How I work

1. Reproduce the exact failure with a deterministic test.
2. Define the smallest observable acceptance condition.
3. Make the narrowest safe code, policy, or configuration change.
4. Exercise the same path under realistic roles or failure ordering.
5. Leave CI evidence, rollback guidance, and residual risks for the handoff.

## Technical focus

- TypeScript and JavaScript on Node.js
- React and Vite build boundaries
- PostgreSQL and Supabase-style Row Level Security
- Webhook verification, idempotency, reconciliation, and entitlement state
- GitHub Actions, deterministic fixtures, JSON/Markdown evidence, and runbooks

I do not present a local harness as production certification. Hosted identity,
provider APIs, infrastructure, performance, and production data paths still
need authorized staging verification for the real application.

## Work with me

The best first consulting fit is an existing application with one known and
already reproducible launch blocker. For hiring teams, the repositories above
show the implementation and review trail rather than a technology-logo list.

[Open a public, redacted fit-check issue](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue/issues/new?template=fit-check.yml)
for a non-sensitive scope question.

**GitHub issues are public. Never include passwords, API keys, tokens, private
repository or staging URLs, customer data, personal data, payment data, or
proprietary code.**

[rls-proof]: https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue
[fit-check]: https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue/issues/new?template=fit-check.yml
