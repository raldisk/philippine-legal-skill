# ph-legal-skill

> Structured Philippine law reference for Claude — 14 domains, 71 modules, 100-row routing table.

---

## What This Is

A modular Philippine law knowledge base built for orchestration via Claude's system-prompt context. Seventy-one doctrine modules span 14 legal specializations, from foundational civil and commercial law to indigenous peoples' rights under R.A. 8371. Each module carries the governing statute, controlling Supreme Court decisions, procedural rules, and doctrinal exceptions for its domain.

**Core design principle:** Every query routes to a specific module through a 100-entry pre-defined routing table. Domain selection is deterministic and auditable — not left to inference. Legal source attribution stays traceable and domain boundaries stay clean across all specializations.

Entry point: **`SKILL.md`** — load as system prompt or context block.

---

## Domain Coverage

| Domain | Modules | Phase |
|--------|---------|-------|
| `core/` | 12 | Foundation |
| `special-laws/` | 7 | Foundation |
| `civil-law/` | 5 | Phase 9 |
| `commercial-law/` | 5 | Phase 1 |
| `taxation/` | 6 | Phase 2 |
| `property-land-law/` | 4 | Phase 3 |
| `intellectual-property/` | 4 | Phase 4 |
| `environmental-law/` | 5 | Phase 5 |
| `immigration/` | 3 | Phase 6 |
| `adr/` | 4 | Phase 7 |
| `exam-tracks/` | 3 | Phase 8 |
| `negotiable-instruments/` | 4 | Phase 11¹ |
| `legal-ethics/` | 2 | Phase 12 |
| `financial-regulation/` | 1 | Phase 13 |
| `indigenous-peoples/` | 1 | Phase 14 |
| `references-index/` | 3 | Cross-phase |

¹ Byte coverage substantially met (16,260–18,842 bytes per file); prose density yields 104–151 lines. Full reconciliation: `FINAL-CONTINUATION-PACKET.md §3 fn¹`.

---

## Architecture

| File | Role |
|------|------|
| `SKILL.md` | Orchestrator — routing logic, query guardrails, module load order |
| `architecture.md` | Structural rules — domain boundaries, overlap handling |
| `references-index/routing-table.md` | Canonical query-to-module routing (100 rows) |
| `references-index/authority-hierarchy.md` | Source authority and citation hierarchy |
| `FINAL-CONTINUATION-PACKET.md` | Session warm-start; integrity baseline |
| `RELEASE-NOTES-v7.0.md` | Release record — phase history, artifact hash |

---

## Usage

```
1. Load SKILL.md as the system prompt.
2. Submit a Philippine law query.
3. The orchestrator routes to the correct domain module.
```

For session continuity: load `FINAL-CONTINUATION-PACKET.md` before `SKILL.md`. It is the sole warm-start document.

---

## Contributing

Review `CONTRIBUTING.md` and `architecture.md` before any modification. Use the provided issue templates (`doctrine-gap.md`, `routing-failure.md`) to report errors in doctrine, routing, or coverage.

---

## License

```
MIT License

Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

**Third-party doctrine sources:**
- Supreme Court of the Philippines — published decisions, resolutions, and rules of procedure
- Congress of the Philippines — Republic Acts, Presidential Decrees, and Codes
- Bangko Sentral ng Pilipinas (BSP) — Monetary Board circulars and regulations
- Bureau of Internal Revenue (BIR) — revenue regulations and rulings

All primary legal materials are government publications. This repository does not claim ownership over doctrine, jurisprudence, or statutory text. The structured knowledge architecture, routing system, and module organization are original works licensed under MIT.

See [`LICENSE`](LICENSE) for full terms.

---

*Philippine law knowledge base · v7.0 · 2026*
