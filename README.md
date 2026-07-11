# App to Production

**I stabilize AI-built apps when the demo works but launch does not.**

I'm Aaron. If you built with Lovable or another AI coding tool and now have a
known Supabase, Stripe, or deployment blocker, I work inside the existing
codebase to produce the smallest test-backed change that addresses the failure
and leaves a clear handoff.

**Best fit:** one reproducible launch blocker, an owned codebase, and a safe
non-production environment.

[Inspect the proof](#production-proof-you-can-run) ·
[Open a redacted fit check][fit-check] ·
[See how I work](#how-i-work)

**Available for fixed-scope contracts and contract or full-time engineering roles.**

> **Portfolio disclosure:** the projects below use synthetic fixtures and are
> reference implementations, not client engagements. Their value is in the
> executable tests, CI runs, source history, and explicit assurance boundaries.

## Does this look like your blocker?

- A signed-in customer can read or change another tenant's data.
- Stripe and application access disagree after duplicate, delayed, or
  out-of-order webhook deliveries.
- Preview works, but production fails because environment contracts, callback
  URLs, API paths, readiness checks, or client bundles have drifted.

Those are the failure classes demonstrated in the repositories below.

## Production proof you can run

| Proof project | Failure addressed | Evidence you can inspect |
| --- | --- | --- |
| [Lovable + Supabase RLS Rescue][rls-proof] | An auth-only policy exposes another tenant's row. | Preserved broken baseline, tenant-scoped read/write migrations, anon/Alice/Bob test matrix, CI, rollback notes. |
| [Billing Webhook + Entitlement Rescue][billing-proof] | Forged, duplicate, delayed, or out-of-order billing events make application access drift. | Signature guard, event-ID idempotency, authoritative reconciliation, dead-letter replay, deterministic tests and CI. |
| [Production Parity Gate][parity-proof] | Preview and production silently diverge. | TypeScript CLI and GitHub Action covering seven modeled drift classes, React/Vite fixture, JSON and Markdown evidence, tests and CI. |

Each repository includes a short reviewer path, executable fixtures, operations
notes, and an explicit statement of what the proof does—and does not—establish.

## How I work

1. Reproduce the exact failure with a deterministic test.
2. Define one observable acceptance condition.
3. Make the narrowest safe code, policy, or configuration change.
4. Exercise the affected path under realistic roles or failure ordering.
5. Leave CI evidence, rollback guidance, residual risks, and a maintainable
   handoff.

I work from the existing application rather than treating every problem as a
blank-slate rebuild.

## Engineering focus

- TypeScript and JavaScript on Node.js
- React and Vite release boundaries
- PostgreSQL and Supabase-style Row Level Security
- Webhook verification, idempotency, reconciliation, and entitlement state
- GitHub Actions, deterministic fixtures, structured evidence, and runbooks

For hiring teams, the repositories show the implementation and review trail:
root cause, source changes, tests, CI, operating limits, and recovery guidance.

## Assurance boundary

A passing local harness is not production certification. Hosted identity,
provider APIs, infrastructure, performance, migrations, and production data
paths still require authorized staging verification for the real application.

## Start with the blocker

If the application already has one known and reproducible launch blocker, open
a [public, redacted project fit check][fit-check].

**GitHub issues are public. Never include passwords, API keys, tokens, private
repository or staging URLs, customer data, personal data, payment data,
proprietary code, or production payloads.**

[rls-proof]: https://github.com/AppToProduction/lovable-supabase-rls-rescue
[billing-proof]: https://github.com/AppToProduction/stripe-entitlements-rescue-reference
[parity-proof]: https://github.com/AppToProduction/production-parity-gate
[fit-check]: https://github.com/AppToProduction/AppToProduction/issues/new?template=project-fit.yml
