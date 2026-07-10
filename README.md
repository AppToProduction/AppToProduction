# I fix launch-blocking access-control failures in Lovable + Supabase apps

I'm Aaron. I focus on one narrow outcome: reproduce a Supabase tenant-isolation failure under realistic user roles, make the smallest safe policy change, and leave behind a regression test, CI evidence, and rollback notes.

[Review the broken-to-fixed RLS proof](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue) | [Request a public fit check](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue/issues/new?template=fit-check.yml)

> **Reference-work disclosure:** The linked project uses synthetic tenants and demonstration data. It shows my process and technical approach; it is not client work, and its intentionally vulnerable baseline is never deployed.

## What you can verify

| Evidence | What it shows |
| --- | --- |
| [Baseline finding](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue/blob/main/docs/audit/baseline-findings.md) | The cross-tenant read is reproduced before remediation. |
| [Remediation ledger](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue/blob/main/docs/audit/remediation-ledger.md) | The policy change is narrow, documented, and tied to a test. |
| [Role-accurate CI](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue/actions) | The same attack path is checked automatically without treating a service role as an end user. |
| [Rollback runbook](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue/blob/main/docs/operations/rollback-runbook.md) | The handoff includes recovery steps instead of only a code patch. |
| [Residual risks](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue/blob/main/docs/operations/residual-risks.md) | Untested paths and limits remain explicit. |

## A bounded first engagement

The best fit is an existing Lovable + Supabase app with one known and already reproducible RLS or tenant-isolation blocker. I work staging-first, use least-privilege access, define the acceptance test before changing code, and deliver the fix through a reviewable branch with evidence and rollback notes.

This is not a whole-app security certification, compliance audit, destructive migration, or authorization to probe a production system.

## Request a fit check

[Open a fit-check issue](https://github.com/VJO-JavaScript/lovable-supabase-rls-rescue/issues/new?template=fit-check.yml) with a sanitized description of the broken flow and the outcome you need.

**GitHub issues are public. Do not include passwords, API keys, access tokens, production data, customer information, private repository links, or private app URLs.** Use placeholders for anything sensitive. Repository access is neither requested nor required for the initial fit check.
