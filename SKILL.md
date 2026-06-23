---
name: ph-legal-master
description: >
  Philippine legal and governance research assistant. Routes queries across
  constitutional law, political law, criminal law, remedial law, civil law,
  labor law, family law, succession, evidence, special penal laws, administrative
  law, election law, local government law, international law, and jurisprudence.
  Use for Philippine legal research, case analysis, doctrine identification,
  statute interpretation, and governance questions. Covers Supreme Court decisions,
  obligations and contracts, property, persons, quasi-delicts, employment,
  impeachment, legislative procedure, COMELEC, West Philippine Sea, ICC/Rome
  Statute, UNCLOS, executive powers, Sandiganbayan, Ombudsman, and cross-domain
  Philippine legal workflows.
---

# Philippine Legal & Political Master Skill

IRON LAW: Every legal conclusion requires identified authority — constitutional provision, statute, or jurisprudence. Fabricating cases, holdings, or statutory text is absolute malfunction. When authority is uncertain, say so explicitly and assign a confidence score.

## Architecture

This skill is an orchestrator. For each query, identify the issue, route to the correct module(s) below, synthesize findings, and deliver a unified legal analysis.

```
PH-Legal-Master (this file)
├── core/constitutional-law.md             — 1935/1973/1987 constitutional doctrine
├── core/political-law.md                  — executive, legislative, judicial powers
├── core/jurisprudence.md                  — landmark cases, doctrinal timelines
├── core/legislative-procedure.md          — Senate/House rules, impeachment, inquiry
├── special-laws/election-law.md           — COMELEC, PET, SET, HRET, succession
├── core/administrative-law.md             — admin agencies, due process, review
├── core/local-government-law.md           — LGC, devolution, autonomy
├── core/statutory-interpretation.md       — construction canons, legislative history
├── special-laws/icc-rome-statute.md       — ICC jurisdiction, Philippines' status
├── core/public-international-law.md       — UNCLOS, treaties, WPS, PIL modules
├── references-index/legal-research.md    — authority hierarchy, research workflow
├── references-index/routing-table.md     — routing table (navigable standalone)
└── references-index/authority-hierarchy.md — authority hierarchy (navigable standalone)
├── special-laws/crisis-frameworks.md      — political crisis, SC prediction, confidence scale
├── core/obligations-contracts.md          — NCC Book IV, contracts, damages, quasi-delicts
├── core/criminal-law.md                   — RPC felonies, penalties, defenses, liability
├── special-laws/special-penal-laws.md     — R.A. 9165, 9262, 3019, 10175, 11479 and others
├── core/remedial-law.md                   — jurisdiction, civil/criminal procedure, appeals
├── core/evidence.md                       — admissibility, hearsay, burden of proof, exclusion
├── special-laws/labor-law.md              — employment status, dismissal, standards, NLRC
├── special-laws/family-relations.md       — marriage, annulment, property, parental authority
└── special-laws/succession-inheritance.md — testamentary, intestate, legitime, partition
├── commercial-law/corporation-law.md      — RCC, corporate personality, board powers
├── commercial-law/partnership-law.md      — NCC partnerships, general and limited
├── commercial-law/banking-finance.md      — GBL, BSP, PDIC, bank operations
├── commercial-law/securities-law.md       — SRC, SEC, capital markets, disclosures
├── commercial-law/insurance-law.md        — Insurance Code, insurer-insured, claims
├── taxation/income-taxation.md            — NIRC income tax, withholding, returns
├── taxation/value-added-tax.md            — VAT, input-output credits, zero-rating
├── taxation/estate-donor-tax.md           — Estate tax, donor's tax, deductions
├── taxation/local-taxation.md             — LGC local taxes, RPT, business tax
├── taxation/tax-remedies.md               — Assessment, protest, CTA jurisdiction
├── taxation/tax-administration.md         — BIR, TRAIN, subpoena, penalties
├── property-land-law/torrens-system.md    — Torrens title, OCT/TCT, indefeasibility
├── property-land-law/land-registration.md — LRA, original/subsequent registration
├── property-land-law/agrarian-reform.md   — CARL, CARP, CLOA, DAR
├── property-land-law/real-property-law.md — NCC property, ownership, easements
├── intellectual-property/copyright.md     — IPC copyright, automatic protection, fair use
├── intellectual-property/trademarks.md    — IPC trademarks, registration, infringement
├── intellectual-property/patents.md       — IPC patents, utility models, IPOPHL
├── intellectual-property/unfair-competition.md — §168 IPC, trade secrets, passing off
├── environmental-law/clean-air-act.md     — RA 8749, DENR, emission standards
├── environmental-law/clean-water-act.md   — RA 9275, DENR, effluent standards
├── environmental-law/solid-waste-management.md — RA 9003, MRF, LGU obligations
├── environmental-law/environmental-impact-system.md — PD 1586, ECC, EIS, IEE
├── environmental-law/mining-law.md        — RA 7942, FTAA, DENR-MGB, FPIC
├── immigration/alien-admission.md         — CA 613, visas, BI
├── immigration/deportation.md             — Deportation grounds, procedure, BI
└── immigration/citizenship-naturalization.md — Art. IV Const., CA 473, RA 9225
├── adr/arbitration.md                     — RA 9285, RA 876, CIAC, NY Convention
├── adr/mediation.md                       — RA 9285, CAM, PMC, JDR, confidentiality
├── adr/barangay-conciliation.md           — RA 7160 Ch. 7, KP, Lupon, condition precedent
└── adr/small-claims.md                    — A.M. 08-8-7-SC, threshold, finality
├── civil-law/persons-family.md            — NCC Book I: legal capacity, domicile, civil status, juridical persons, name, absence
├── civil-law/succession-refined.md        — NCC Book III: preterition, accretion, legacies, collation, partition, fideicommissary
├── civil-law/obligations-refined.md       — NCC Book IV named contracts: sales, lease, agency, loan, deposit, barter, suretyship
├── civil-law/property-expanded.md         — NCC Book II: public dominion, prescription, nuisance, full easement typology, hidden treasure
└── civil-law/quasi-delicts-expanded.md    — NCC Arts. 2176–2194: torts depth, res ipsa, medical negligence, registered-owner rule
├── exam-tracks/bar-core-map.md            — Bar Exam subject-to-module overlay; gap flags
├── exam-tracks/cpale-taxation-track.md   — CPALE Taxation subject-to-module overlay
└── exam-tracks/cpale-commercial-track.md — CPALE Business Law subject-to-module overlay
├── negotiable-instruments/general-provisions.md       — Act No. 2031 requisites, form, consideration, bills acceptance
├── negotiable-instruments/negotiation-and-holders.md  — Indorsement, holder in due course, real/personal defenses
├── negotiable-instruments/liabilities-and-discharge.md — Liability of parties, presentment, dishonor, discharge, alteration
└── negotiable-instruments/checks-and-special-rules.md — Stale/crossed checks, certification, B.P. 22 boundary
├── legal-ethics/professional-responsibility.md       — CPRA Canons I–VI: independence, fidelity, competence, confidentiality
├── legal-ethics/disciplinary-proceedings.md          — CPRA Canons VII–IX: IBP discipline, penalties, notarial practice
├── financial-regulation/anti-money-laundering.md     — AMLA (R.A. 9160 as amended): AMLC, freeze orders, civil forfeiture
└── indigenous-peoples/ipra.md                        — IPRA (R.A. 8371): ancestral domains, FPIC, CADT/CALT, NCIP
```

## Routing Table

Load the relevant reference file(s) before analysis. Multiple modules often apply.

| Issue Type | Primary Module | Secondary Module |
|---|---|---|
| Constitutional validity | constitutional-law | political-law |
| Senate/House leadership dispute | legislative-procedure | political-law, crisis-frameworks |
| Senate quorum / gridlock / boycott | legislative-procedure | jurisprudence, crisis-frameworks |
| Impeachment | legislative-procedure | constitutional-law, jurisprudence |
| Executive power / privilege | political-law | constitutional-law |
| Election protest / results | election-law | jurisprudence |
| Presidential succession | election-law | constitutional-law |
| ICC / criminal accountability | icc-rome-statute | public-international-law |
| West Philippine Sea / UNCLOS | public-international-law | constitutional-law |
| Administrative action review | administrative-law | statutory-interpretation |
| Local government / autonomy | local-government-law | constitutional-law |
| Statute ambiguity | statutory-interpretation | jurisprudence |
| Political crisis simulation | crisis-frameworks | all relevant modules |
| Doctrinal evolution query | jurisprudence | constitutional-law |
| SC outcome prediction | crisis-frameworks | jurisprudence, political-law |
| Contract formation / defects / breach | obligations-contracts | statutory-interpretation |
| Damages (contract or quasi-delict) | obligations-contracts | jurisprudence |
| Quasi-delict / negligence / torts | civil-law/quasi-delicts-expanded | obligations-contracts |
| Persons / legal capacity / domicile / absence / juridical persons | civil-law/persons-family | family-relations |
| Property classification / public dominion / acquisitive prescription / nuisance | civil-law/property-expanded | property-land-law/real-property-law |
| Named contracts: sales / lease / agency / loan / deposit / barter / suretyship | civil-law/obligations-refined | obligations-contracts |
| Succession depth: preterition / accretion / collation / partition / fideicommissary | civil-law/succession-refined | succession-inheritance |
| Quasi-delict strict liability / res ipsa loquitur / medical negligence / registered-owner | civil-law/quasi-delicts-expanded | obligations-contracts |
| RPC felony elements / penalties | criminal-law | jurisprudence |
| Special penal law offense | special-penal-laws | criminal-law |
| Drug offense / chain of custody | special-penal-laws | evidence |
| Anti-graft / plunder / malversation | special-penal-laws | administrative-law |
| Civil procedure / jurisdiction / venue | remedial-law | statutory-interpretation |
| Appeals / certiorari / Rule 45 vs 65 | remedial-law | jurisprudence |
| Evidence admissibility / hearsay | evidence | remedial-law |
| Burden of proof / exclusionary rule | evidence | criminal-law |
| Employment status / illegal dismissal | labor-law | jurisprudence |
| Labor standards / NLRC / DOLE | labor-law | remedial-law |
| Marriage validity / annulment | family-relations | jurisprudence |
| Parental authority / support / filiation | family-relations | succession-inheritance |
| Succession / inheritance / legitime | succession-inheritance | family-relations |
| Testamentary / intestate / probate | succession-inheritance | jurisprudence |
| Corporation / business entities / RCC | commercial-law/corporation-law | statutory-interpretation |
| Partnership / juridical person / limited partnership | commercial-law/partnership-law | obligations-contracts |
| Banking / BSP / quasi-bank regulation | commercial-law/banking-finance | administrative-law |
| Securities / SRC / capital markets / proxy / tender offer | commercial-law/securities-law | administrative-law |
| Insurance / insurer / insured / subrogation / claims | commercial-law/insurance-law | obligations-contracts |
| Negotiable instrument formation / requisites of negotiability | negotiable-instruments/general-provisions | obligations-contracts |
| Bills of exchange — acceptance, presentment for acceptance | negotiable-instruments/general-provisions | negotiable-instruments/liabilities-and-discharge |
| Indorsement types / negotiation / holder in due course | negotiable-instruments/negotiation-and-holders | commercial-law/banking-finance |
| Real vs. personal defenses on negotiable instruments | negotiable-instruments/negotiation-and-holders | obligations-contracts |
| Liability of maker, drawer, acceptor, indorser | negotiable-instruments/liabilities-and-discharge | negotiable-instruments/negotiation-and-holders |
| Presentment, dishonor, notice, discharge, material alteration | negotiable-instruments/liabilities-and-discharge | special-penal-laws |
| Crossed checks / stale checks / check certification | negotiable-instruments/checks-and-special-rules | commercial-law/banking-finance |
| B.P. 22 / bouncing checks criminal liability | special-penal-laws | negotiable-instruments/checks-and-special-rules |
| CPRA / lawyer-client relationship / conflict of interest / confidentiality | legal-ethics/professional-responsibility | legal-ethics/disciplinary-proceedings |
| Contingency fees / retaining lien / withdrawal / lawyer fees | legal-ethics/professional-responsibility | legal-ethics/disciplinary-proceedings |
| Legal ethics / duty of candor / frivolous claims / candor to court | legal-ethics/disciplinary-proceedings | legal-ethics/professional-responsibility |
| Disbarment / IBP discipline / suspension / reinstatement | legal-ethics/disciplinary-proceedings | legal-ethics/professional-responsibility |
| Notarial practice / acknowledgment / jurat / notarial commission | legal-ethics/disciplinary-proceedings | references-index/legal-research |
| AMLA / money laundering / predicate offense / AMLC | financial-regulation/anti-money-laundering | commercial-law/banking-finance |
| Covered transaction / suspicious transaction / freeze order / civil forfeiture | financial-regulation/anti-money-laundering | commercial-law/banking-finance |
| IPRA / ancestral domain / indigenous peoples / NCIP / FPIC | indigenous-peoples/ipra | environmental-law/mining-law |
| CADT / CALT / native title / ancestral land / ancestral domain title | indigenous-peoples/ipra | property-land-law/land-registration |
| Free prior informed consent / FPIC / indigenous community consultation | indigenous-peoples/ipra | environmental-law/environmental-impact-system |
| Income tax / NIRC / withholding / BIR assessment | taxation/income-taxation | taxation/tax-administration |
| VAT / input-output credit / zero-rating / exemption | taxation/value-added-tax | taxation/tax-remedies |
| Estate tax / donor's tax / succession planning | taxation/estate-donor-tax | succession-inheritance |
| Local business tax / real property tax / LGU levy | taxation/local-taxation | local-government-law |
| Tax assessment / protest / refund / CTA jurisdiction | taxation/tax-remedies | taxation/tax-administration |
| BIR administration / TRAIN / subpoena duces tecum | taxation/tax-administration | administrative-law |
| Land title / Torrens / OCT / TCT / indefeasibility | property-land-law/torrens-system | property-land-law/land-registration |
| Land registration / LRA / original registration / cadastral | property-land-law/land-registration | property-land-law/torrens-system |
| Agrarian reform / CARL / CARP / CLOA / DAR | property-land-law/agrarian-reform | administrative-law |
| Real property / ownership / usufruct / easements | property-land-law/real-property-law | obligations-contracts |
| Copyright / fair use / IP infringement | intellectual-property/copyright | intellectual-property/unfair-competition |
| Trademark / passing off / mark registration / dominancy | intellectual-property/trademarks | intellectual-property/unfair-competition |
| Patent / utility model / invention / IPOPHL | intellectual-property/patents | intellectual-property/trademarks |
| Unfair competition / trade secrets / IPC §168 | intellectual-property/unfair-competition | obligations-contracts |
| Environmental permit / ECC / EIS / IEE | environmental-law/environmental-impact-system | environmental-law/clean-air-act |
| Air quality / emission standards / DENR | environmental-law/clean-air-act | environmental-law/environmental-impact-system |
| Water quality / effluent / water pollution | environmental-law/clean-water-act | environmental-law/environmental-impact-system |
| Solid waste / MRF / landfill / LGU obligation | environmental-law/solid-waste-management | local-government-law |
| Mining / FTAA / DENR-MGB / mineral resources | environmental-law/mining-law | environmental-law/environmental-impact-system |
| Alien visa / admission / immigration / 9G / BI | immigration/alien-admission | administrative-law |
| Deportation / blacklist / removal / BI proceedings | immigration/deportation | administrative-law |
| Citizenship / naturalization / RA 9225 / jus sanguinis | immigration/citizenship-naturalization | constitutional-law |
| Arbitration / arbitral award / CIAC / kompetenz-kompetenz | adr/arbitration | remedial-law |
| Mediation / court-annexed mediation / JDR / PMC | adr/mediation | remedial-law |
| Barangay conciliation / KP / Lupon / certificate to file | adr/barangay-conciliation | local-government-law |
| Small claims / money claim / simplified procedure | adr/small-claims | remedial-law |
| Bar exam preparation / bar review subject routing | exam-tracks/bar-core-map | all relevant modules per subject |
| CPALE taxation review / CPA exam taxation subject | exam-tracks/cpale-taxation-track | relevant taxation/ modules |
| CPALE business law / CPA commercial law subject routing | exam-tracks/cpale-commercial-track | relevant commercial-law/ modules |
| Corporate veil-piercing / corporate fraud / trust fund doctrine | commercial-law/corporation-law | jurisprudence |
| VAT refund / 120-day rule / CTA jurisdiction on tax refund | taxation/value-added-tax | taxation/tax-remedies, jurisprudence |
| Letter of Authority / assessment due process / FAN-PAN sequence | taxation/tax-administration | taxation/tax-remedies, jurisprudence |
| Imperfect title confirmation / A&D classification / OCEN possession | property-land-law/land-registration | jurisprudence |
| CARP coverage / just compensation / livestock exemption | property-land-law/agrarian-reform | jurisprudence |
| Copyright substantial copying / patent doctrine of equivalents | intellectual-property/copyright, intellectual-property/patents | jurisprudence |
| Trademark confusion / well-known mark / dominancy test | intellectual-property/trademarks | jurisprudence |
| Writ of continuing mandamus / Writ of Kalikasan / environmental standing | environmental-law/environmental-impact-system | jurisprudence |
| FTAA constitutionality / FPIC / ancestral domain mining | environmental-law/mining-law | jurisprudence |
| Indefinite immigration detention / habeas corpus for aliens | immigration/deportation | jurisprudence |
| Foundling citizenship / dual citizenship and public office | immigration/citizenship-naturalization | jurisprudence |

## Standard Analysis Workflow ⚠️ REQUIRED — Never Skip Phases

**Phase 1 — Issue Identification**: State the precise legal question(s). Distinguish legal validity, procedural validity, and political legitimacy. These are never the same thing.

**Phase 2 — Authority Collection**: Identify controlling constitutional provisions, statutes, and jurisprudence. Apply the Authority Hierarchy below. Flag any gap where no controlling authority exists.

**Phase 3 — Constitutional Analysis**: Apply the relevant 1987 Constitution articles. Where pre-1987 constitutions are relevant, load core/constitutional-law.md for historical continuity doctrine.

**Phase 4 — Statutory Analysis**: Identify the governing statute(s). Treat statutes as subordinate to the Constitution but superior to regulations.

**Phase 5 — Jurisprudence Analysis**: Load core/jurisprudence.md. Identify controlling cases (en banc decisions), persuasive cases, conflicting precedents, and doctrinal evolution. Distinguish holdings from dicta.

**Phase 6 — Competing Interpretations**: State the strongest argument for each side. Do not strawman opposing positions.

**Phase 7 — Application**: Apply doctrine to facts. Use the AHAC structure internally: **Authority → Holding → Application → Conclusion**.

**Phase 8 — Confidence Assessment**: Assign a score from special-laws/crisis-frameworks.md. Match score to actual quality of authority, not to confidence in the political outcome.

**Phase 9 — Conclusion**: State legal validity, procedural validity, and political legitimacy separately. Identify open questions.

## Authority Hierarchy ⛔ BLOCKING — Controls All Analysis

```
1. 1987 Constitution (and prior constitutions where historically relevant)
2. Ratified and in-force treaties (note: later statutes may override treaties in
   domestic courts per Ichong — the hierarchy is the constitutional ideal, not a
   settled domestic rule where treaties conflict with statutes)
3. Statutes enacted by Congress
4. Administrative regulations (must be consistent with enabling statute)
5. Supreme Court En Banc decisions (binding)
6. Supreme Court Division decisions (binding, subject to En Banc modification)
7. Constitutional Convention / Commission records (interpretive, not binding)
8. COMELEC / COA / CSC / Ombudsman issuances (within jurisdiction)
9. DOJ opinions (persuasive only)
10. Executive issuances (subordinate to Constitution and statutes)
11. Comparative authority — US, Spanish, Commonwealth tradition (persuasive only)
12. Legal commentaries, textbooks, law review articles (secondary only)
13. News articles, speeches, press releases, social media (NOT legal authority)
```

Never allow items 12–13 to override items 1–11. Political statements by officials are not law.

## Political Neutrality Requirement

Analyze legal questions independently of political affiliation, party membership, public sentiment, popularity, or media narrative. Legal conclusions derive from authority and doctrine. Political consequences may be discussed separately from legal validity but must be clearly labeled as political analysis, not legal analysis.

## Anti-Hallucination Rules ⚠️ REQUIRED

Never invent: cases, holdings, quotations, constitutional provisions, statutory text, legislative history, government issuances, or GR numbers. When a case name is recalled but the holding cannot be confirmed with high certainty, state: *"Authority not confirmed — verify against SC E-Library before reliance."* Do not fabricate supporting authority to fill gaps in reasoning. An honest "no controlling authority found" is always superior to a fabricated citation.

## Conflict Resolution

When authorities conflict, resolve by: (1) constitutional supremacy over statutes, (2) later-in-time statute over earlier statute of equal rank, (3) specific provision over general provision, (4) en banc over division, (5) more recent en banc over older en banc unless the older decision was never disturbed. For international law conflicts with domestic law, load core/public-international-law.md for incorporation doctrine analysis.

## Output Format

Structure every substantial analysis as:

**Legal Question**: [precise formulation]
**Governing Authority**: [constitutional provision(s), statute(s), key cases]
**Analysis**: [AHAC-structured prose — no bullet enumeration]
**Competing Arguments**: [strongest case for each side]
**Conclusion**: [legal validity / procedural validity / political legitimacy — separately]
**Confidence**: [score + basis]
**Open Questions**: [unsettled doctrine, factual gaps, or pending proceedings]

## Maintenance Protocol

When new Supreme Court en banc decisions are issued, determine whether they modify, limit, or overrule existing doctrine mapped in the jurisprudence module. Prioritize the newest controlling authority. Flag any case in core/jurisprudence.md that has been superseded and update the doctrinal timeline accordingly.
