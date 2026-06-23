# Architecture — Philippine Legal Operating System
## Repository: `ph-legal-skill-v3`
**Version**: 7.0 (Phases 1–14 built)  
**Migration Status**: Core + Special Laws complete (strong). Phases 1–14 (Commercial Law, Taxation, Property-Land Law, IP, Environmental Law, Immigration, ADR, Exam Tracks, Civil Law, Jurisprudence Expansion, Negotiable Instruments Law, Legal Ethics, Financial Regulation, Indigenous Peoples) complete — all production-grade.

---

## Repository Structure

```
ph-legal-skill-v3/
├── SKILL.md                          — Orchestrator: routing, authority hierarchy, workflow
├── architecture.md                   — This file: structural ground truth
├── core/                             — Foundational Philippine law (12 modules)
│   ├── constitutional-law.md
│   ├── political-law.md
│   ├── legislative-procedure.md
│   ├── administrative-law.md
│   ├── local-government-law.md
│   ├── statutory-interpretation.md
│   ├── public-international-law.md
│   ├── jurisprudence.md
│   ├── criminal-law.md
│   ├── obligations-contracts.md
│   ├── remedial-law.md
│   └── evidence.md
├── special-laws/                     — Domain-specific statutes and frameworks (7 modules)
│   ├── labor-law.md
│   ├── family-relations.md
│   ├── succession-inheritance.md
│   ├── election-law.md
│   ├── special-penal-laws.md
│   ├── icc-rome-statute.md
│   └── crisis-frameworks.md
├── references-index/                 — Navigation, authority hierarchy, research workflow
│   ├── authority-hierarchy.md
│   ├── legal-research.md
│   └── routing-table.md
├── commercial-law/                   — Phase 1 complete (5 modules)
│   ├── corporation-law.md
│   ├── partnership-law.md
│   ├── banking-finance.md
│   ├── securities-law.md
│   └── insurance-law.md
├── taxation/                         — Phase 2 complete (6 modules)
│   ├── income-taxation.md
│   ├── value-added-tax.md
│   ├── estate-donor-tax.md
│   ├── local-taxation.md
│   ├── tax-remedies.md
│   └── tax-administration.md
├── property-land-law/                — Phase 3 complete (4 modules)
│   ├── torrens-system.md
│   ├── land-registration.md
│   ├── agrarian-reform.md
│   └── real-property-law.md
├── intellectual-property/            — Phase 4 complete (4 modules)
│   ├── copyright.md
│   ├── trademarks.md
│   ├── patents.md
│   └── unfair-competition.md
├── environmental-law/                — Phase 5 complete (5 modules)
│   ├── clean-air-act.md
│   ├── clean-water-act.md
│   ├── solid-waste-management.md
│   ├── environmental-impact-system.md
│   └── mining-law.md
├── immigration/                      — Phase 6 complete (3 modules)
│   ├── alien-admission.md
│   ├── deportation.md
│   └── citizenship-naturalization.md
├── adr/                              — Phase 7 complete (4 modules)
│   ├── arbitration.md
│   ├── mediation.md
│   ├── barangay-conciliation.md
│   └── small-claims.md
├── exam-tracks/                      — Phase 8 complete (3 overlay modules)
│   ├── bar-core-map.md
│   ├── cpale-taxation-track.md
│   └── cpale-commercial-track.md
├── civil-law/                        — Phase 9 complete (5 modules)
│   ├── persons-family.md
│   ├── succession-refined.md
│   ├── obligations-refined.md
│   ├── property-expanded.md
│   └── quasi-delicts-expanded.md
├── negotiable-instruments/           — Phase 11 complete (4 modules)
│   ├── general-provisions.md
│   ├── negotiation-and-holders.md
│   ├── liabilities-and-discharge.md
│   └── checks-and-special-rules.md
├── legal-ethics/                     — Phase 12 complete (2 modules)
│   ├── professional-responsibility.md
│   └── disciplinary-proceedings.md
├── financial-regulation/             — Phase 13 complete (1 module)
│   └── anti-money-laundering.md
├── indigenous-peoples/               — Phase 14 complete (1 module)
│   └── ipra.md
└── legacy/
    └── archived-flat-modules/        — Pre-migration flat references/ structure (20 files)
```

---

## Domain Ownership

| Module | Domain | Basis |
|---|---|---|
| constitutional-law.md | core | Foundational public law; controls all other domains |
| political-law.md | core | Executive/legislative/judicial power frameworks |
| legislative-procedure.md | core | Constitutional legislative process |
| administrative-law.md | core | Agency power, administrative due process |
| local-government-law.md | core | LGC, devolution, BARMM |
| statutory-interpretation.md | core | Interpretive tools; cross-cutting |
| public-international-law.md | core | PIL, UNCLOS, WPS, treaties |
| jurisprudence.md | core | Cross-domain landmark cases |
| criminal-law.md | core | RPC — foundational penal code |
| obligations-contracts.md | core | NCC Book IV — foundational private law |
| remedial-law.md | core | Rules of Court — foundational procedure |
| evidence.md | core | Rules on Evidence — cross-cutting |
| labor-law.md | special-laws | Labor Code + DOLE/NLRC framework |
| family-relations.md | special-laws | Family Code + SC doctrine |
| succession-inheritance.md | special-laws | NCC Book III |
| election-law.md | special-laws | COMELEC, PET, SET, HRET, succession |
| special-penal-laws.md | special-laws | R.A. 9165, 3019, 10175, 11479, others |
| icc-rome-statute.md | special-laws | ICC/Rome Statute + Philippines status |
| crisis-frameworks.md | special-laws | Political crisis analysis, confidence scale |
| corporation-law.md | commercial-law | RCC, SEC; corporate personality framework |
| partnership-law.md | commercial-law | NCC Arts. 1767–1867; general and limited |
| banking-finance.md | commercial-law | GBL (RA 8791), BSP (RA 7653/11211), PDIC |
| securities-law.md | commercial-law | SRC (RA 8799), SEC, capital markets |
| insurance-law.md | commercial-law | Insurance Code (PD 1460/RA 10607) |
| income-taxation.md | taxation | NIRC, RA 10963 (TRAIN), income classification |
| value-added-tax.md | taxation | NIRC VAT provisions, input-output credits |
| estate-donor-tax.md | taxation | Estate tax (NIRC §84–97), donor's tax (§98–104) |
| local-taxation.md | taxation | LGC Secs. 129–221, RPT, local business tax |
| tax-remedies.md | taxation | Assessment, protest, CTA jurisdiction, refunds |
| tax-administration.md | taxation | BIR powers, penalties, TRAIN, subpoena |
| torrens-system.md | property-land-law | PD 1529, OCT/TCT, indefeasibility, forgery |
| land-registration.md | property-land-law | LRA, original registration, subsequent acts |
| agrarian-reform.md | property-land-law | CARL (RA 6657), CARP, CLOA, DAR, VOS |
| real-property-law.md | property-land-law | NCC Book II (Arts. 414–773), ownership, easements |
| copyright.md | intellectual-property | IPC Parts II/IV, automatic protection, fair use |
| trademarks.md | intellectual-property | IPC Part III, registration, dominancy test |
| patents.md | intellectual-property | IPC Part II, utility models, IPOPHL |
| unfair-competition.md | intellectual-property | IPC §168, trade secrets, passing off |
| clean-air-act.md | environmental-law | RA 8749, DENR, ambient/emission standards |
| clean-water-act.md | environmental-law | RA 9275, DENR-EMB, effluent standards |
| solid-waste-management.md | environmental-law | RA 9003, MRF, LGU obligation |
| environmental-impact-system.md | environmental-law | PD 1586, DENR-EMB, ECC, EIS, IEE |
| mining-law.md | environmental-law | RA 7942, FTAA, DENR-MGB, FPIC (IPRA link) |
| alien-admission.md | immigration | CA 613 (Phil. Immigration Act), BI, visa types |
| deportation.md | immigration | CA 613 deportation grounds, BI, due process |
| citizenship-naturalization.md | immigration | Art. IV Const., CA 473, RA 9139, RA 9225 |

---

## Authority Hierarchy

Defined in SKILL.md § "Authority Hierarchy ⛔ BLOCKING". Canonical version maintained in SKILL.md.  
Quick reference:
1. 1987 Constitution
2. Ratified in-force treaties (domestic courts: later-statute rule per *Ichong*)
3. Statutes
4. Administrative regulations
5. SC En Banc decisions
6. SC Division decisions
7. ConCom records (interpretive only)
8. COMELEC/COA/CSC/Ombudsman issuances (within jurisdiction)
9. DOJ opinions (persuasive)
10. Executive issuances
11. Comparative authority (persuasive)
12. Commentaries/textbooks (secondary)
13. News, speeches, social media (NOT legal authority)

---

## Drift Prevention

Before any structural change to this repository:
1. Verify against this file and SKILL.md routing table
2. Produce a Change Impact Statement (files, routing, doctrine, dependency, rollback)
3. No change proceeds if routing breaks, orphans are created, or contradictions introduced
4. Uncertainty threshold: if certainty < 95%, STOP AND REPORT

---

## Planned Expansion Domains

A domain folder may only be instantiated when:
- Purpose is documented
- Ownership boundaries are defined
- Routing implications identified
- At least one validated module exists for that domain

| Domain | Target Modules | Status |
|---|---|---|
| commercial-law | corporation, partnership, banking, securities, insurance | **COMPLETE (Phase 1)** |
| taxation | income, VAT, estate/donor, local, remedies, administration | **COMPLETE (Phase 2)** |
| property-land-law | torrens, land-registration, agrarian-reform, real-property | **COMPLETE (Phase 3)** |
| intellectual-property | copyright, trademarks, patents, unfair-competition | **COMPLETE (Phase 4)** |
| environmental-law | clean-air, clean-water, solid-waste, EIS, mining | **COMPLETE (Phase 5)** |
| immigration | alien-admission, deportation, citizenship-naturalization | **COMPLETE (Phase 6)** |
| adr | arbitration, mediation, barangay-conciliation, small-claims | **COMPLETE (Phase 7)** |
| exam-tracks | bar-core-map, cpale-taxation-track, cpale-commercial-track | **COMPLETE (Phase 8)** |
| civil-law | persons-family, property, obligations-refined, quasi-delicts, succession-refined | **COMPLETE (Phase 9)** |
| negotiable-instruments | general-provisions, negotiation-and-holders, liabilities-and-discharge, checks-and-special-rules (Act No. 2031) | **COMPLETE (Phase 11)** |
| legal-ethics | professional-responsibility, disciplinary-proceedings (CPRA 2023) | **COMPLETE (Phase 12)** |
| financial-regulation | anti-money-laundering (AMLA, R.A. 9160) | **COMPLETE (Phase 13)** |
| indigenous-peoples | ipra (R.A. 8371) | **COMPLETE (Phase 14)** |

### Future Expansion Dependencies (not yet created)
- `financial-regulation/anti-money-laundering.md` — referenced by `commercial-law/banking-finance.md`; AMLA domain (**Phase 13** — ✅ COMPLETE; see Phase 13 Domain Ownership section)
- `indigenous-peoples/ipra.md` — referenced by `environmental-law/mining-law.md`; IPRA domain (**Phase 14** — ✅ COMPLETE; see Phase 14 Domain Ownership section)

---

## Civil Law Domain Ownership (Phase 9)

| Module | Domain | Basis |
|---|---|---|
| civil-law/persons-family.md | civil-law | NCC Book I Arts. 37–413; R.A. 9048, 10172, 9255, 6809; Rule 108 |
| civil-law/succession-refined.md | civil-law | NCC Book III Arts. 774–1105 (mechanics layer); Rules 74, 90 |
| civil-law/obligations-refined.md | civil-law | NCC Book IV Arts. 1458–2084 (named contracts); R.A. 6552 |
| civil-law/property-expanded.md | civil-law | NCC Book II Arts. 414–773; NCC Arts. 1106–1155 (prescription) |
| civil-law/quasi-delicts-expanded.md | civil-law | NCC Arts. 2176–2194; SC doctrinal evolution on torts |

---

## Negotiable Instruments Domain Ownership (Phase 11)

| Module | Domain | Basis |
|---|---|---|
| negotiable-instruments/general-provisions.md | negotiable-instruments | Act No. 2031 §§1–29, 126–183 — requisites of negotiability, form, consideration, bills-of-exchange acceptance |
| negotiable-instruments/negotiation-and-holders.md | negotiable-instruments | Act No. 2031 §§30–61 — negotiation, indorsement, holder in due course, real/personal defenses |
| negotiable-instruments/liabilities-and-discharge.md | negotiable-instruments | Act No. 2031 §§60–125 — liability of parties, presentment, dishonor, discharge, material alteration |
| negotiable-instruments/checks-and-special-rules.md | negotiable-instruments | Act No. 2031 §§184–189 + banking practice/jurisprudence — checks, stale/crossed checks, B.P. 22 boundary |

**Note**: Act No. 2031 (Negotiable Instruments Law, 1911) — not B.P. 129 (Judiciary Reorganization Act of 1980, unrelated). A pre-existing mislabel of NIL as "B.P. 129" was corrected across README.md, this file, FINAL-CONTINUATION-PACKET.md, and exam-tracks/bar-core-map.md as part of Phase 11 build integrity checks.

---

## Phase 12 Domain Ownership (Legal Ethics)

| Module | Domain | Basis |
|---|---|---|
| legal-ethics/professional-responsibility.md | legal-ethics | CPRA (A.M. No. 22-09-01-SC, 2023) Canons I–VI — independence, propriety, fidelity, competence, equality, confidentiality |
| legal-ethics/disciplinary-proceedings.md | legal-ethics | CPRA Canons VII–IX + Rule 139-B + 2004 Rules on Notarial Practice — accountability, fairness, dignity, IBP discipline, penalties |

**Note**: The CPRA (April 11, 2023) supersedes the 1988 Code of Professional Responsibility in its entirety. All legal-ethics modules cite CPRA Canon/Section numbers. Historical CPR references are labeled as such.

---

## Phase 13 Domain Ownership (Financial Regulation)

| Module | Domain | Basis |
|---|---|---|
| financial-regulation/anti-money-laundering.md | financial-regulation | R.A. 9160 (AMLA 2001) as amended by R.A. 9194, 10167, 10365, 10927, 11521 — full AMLA doctrine including predicate offenses, AMLC, freeze orders, civil forfeiture |

**Boundary**: `commercial-law/banking-finance.md` retains the banking-compliance-operations layer (BSP Circular KYC requirements, bank AMLA compliance procedures). `financial-regulation/anti-money-laundering.md` owns the full statutory AMLA doctrine. No duplication; cross-referenced.

---

## Phase 14 Domain Ownership (Indigenous Peoples)

| Module | Domain | Basis |
|---|---|---|
| indigenous-peoples/ipra.md | indigenous-peoples | R.A. 8371 (IPRA 1997) — native title, four bundles of rights, FPIC procedure, CADT/CALT, NCIP jurisdiction, Regalian Doctrine interface |

**Boundary**: FPIC mining interface is documented in `environmental-law/mining-law.md` (§68–76) and `environmental-law/environmental-impact-system.md` (§109); those modules cross-reference `indigenous-peoples/ipra.md` for the foundational IPRA doctrine. CADT/Torrens distinction is in `property-land-law/land-registration.md` (§74). No duplication; cross-referenced.
