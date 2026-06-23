# Contributing

Read `architecture.md` **completely** before making any changes. The drift-prevention rules and domain-boundary rules are mandatory. Changes that violate them will not be accepted.

---

## Pre-Change Checklist

Before touching any file:

1. Verify SHA256 content baseline (see `FINAL-CONTINUATION-PACKET.md` §2).
2. Confirm target domain is in scope for the current authorized phase (`FINAL-CONTINUATION-PACKET.md` §10).
3. Check `references-index/routing-table.md` — every new module requires a routing entry.
4. Check `references-index/authority-hierarchy.md` — confirm authority tier for new citations.
5. Review overlap with adjacent domains (see `architecture.md` §Overlap Rules).
6. Apply the Change Impact Statement format before any structural change.

---

## Coverage Standard

All committed doctrine must be one of:

- **Strong** (≥200 lines / ≥8,000 bytes) — production-grade; the required standard for final domains.
- **Draft** — explicitly labeled, phase documented, expansion authorized.
- **Stub** — explicitly labeled, phase documented, expansion scheduled.

Do not commit partial doctrine without labeling it. Do not relabel a stub as strong without meeting the depth standard.

---

## Routing Requirement

Every new module must have:

- A routing row in `references-index/routing-table.md`
- A handler reference in `SKILL.md`

No module without routing will be accepted.

---

## Drift Prevention Rules

- One canonical doctrine file per subdomain. No parallel files for the same doctrine.
- No silent cross-domain duplication. If two modules would share doctrine, define a routing rule and reference.
- No file creation without routing purpose.
- No structural folder changes without a Change Impact Statement.
- No modification of `legacy/archived-flat-modules/` — read-only reference only.

---

## Submitting Issues

Use the issue templates:

- **Doctrine Gap** — missing rule, wrong statute, case mismatch, thin coverage.
- **Routing Failure** — query lands in wrong module or module not reachable.

---

## Submitting Pull Requests

Use the PR template. PRs without completed templates will be returned.

Required in every PR:

- Module changed and reason
- Routing change (if any), with before/after routing rows
- Overlap check result (which adjacent domains checked)
- Depth before / after (bytes and line count)
- SHA256 impact (new content baseline if applicable)
