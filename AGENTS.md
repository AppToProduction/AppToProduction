# Repository instructions

## Product goal

Present Aaron's narrow Lovable + Supabase launch-rescue offer and route qualified prospects to a safe, public fit-check issue.

## Architecture

This is the special GitHub profile repository for the `VJO-JavaScript` account. `README.md` is the buyer-facing profile. `docs/github-metadata.md` records the recommended account and repository fields.

## Commands

- Setup: none.
- Development preview: render `README.md` with GitHub's Markdown preview.
- Placeholder check: `rg -n "FLAGSHIP_URL|EVIDENCE_URL|INTAKE_URL|TODO|TBD" .`
- Link inventory: `rg -o "https://[^) ]+" README.md docs/github-metadata.md`
- Build: none.

## Environment and secrets

No environment variables, tokens, private URLs, customer data, or credentials belong in this repository. The intake route is a public GitHub issue and must warn users accordingly.

## Deployment target

Public GitHub repository `VJO-JavaScript/VJO-JavaScript`. Publishing or changing public account fields requires Aaron's approval and a signed-out link check.

## Verification checklist

- The flagship repository and every linked document exist publicly.
- The fit-check issue template opens successfully.
- CI is green before the profile claims CI evidence.
- The reference-work disclosure remains above the evidence table.
- No client results, testimonials, or credentials are implied.
- No secrets or private contact details appear in content or Git history.

## Definition of done

The public profile renders cleanly, communicates one narrow outcome, links to working evidence, and routes prospects to a public, privacy-safe fit check.

## High-risk files

- `README.md`: public buyer-facing claims and intake warnings.
- `docs/github-metadata.md`: recommended public account fields.

