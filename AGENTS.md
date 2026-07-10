# Repository instructions

## Product goal

Present Aaron as an AI app production engineer for both hiring teams and
fixed-scope rescue clients. Route non-sensitive Supabase questions to a safe,
public fit-check issue while keeping every portfolio claim evidence-backed.

## Architecture

This is the special GitHub profile repository for the `VJO-JavaScript` account.
`README.md` is the public hiring/client profile, `assets/` contains editable
brand sources, and `docs/github-metadata.md` records the approved account,
identity, and pin strategy.

## Commands

- Setup: none.
- Development preview: render `README.md` with GitHub's Markdown preview.
- Placeholder check: `rg -n "FLAGSHIP_URL|EVIDENCE_URL|INTAKE_URL|TODO|TBD" .`
- Link inventory: `rg -o "https://[^) ]+" README.md docs/github-metadata.md`
- Build: none.

## Environment and secrets

No environment variables, tokens, private URLs, customer data, or credentials
belong in this repository. The intake route is a public GitHub issue and must
warn users accordingly.

## Deployment target

Public GitHub repository `VJO-JavaScript/VJO-JavaScript`. Publishing or changing
public account fields requires Aaron's approval and a signed-out link check.

## Verification checklist

- All three selected-work repositories and every linked document exist publicly.
- The fit-check issue template opens successfully.
- CI is green before the profile claims CI evidence.
- The reference-work disclosure remains above the evidence table.
- No client results, testimonials, or credentials are implied.
- No secrets or private contact details appear in content or Git history.

## Definition of done

The public profile renders cleanly, shows three distinct production-engineering
proofs, communicates honest assurance boundaries, and routes non-sensitive
questions to a public, privacy-safe fit check.

## High-risk files

- `README.md`: public buyer-facing claims and intake warnings.
- `docs/github-metadata.md`: recommended public account fields.
