# CPALE Commercial Track — CPA Licensure Examination (Business Law)

## Purpose and Constraint

**Overlay only.** This file contains no doctrine. It maps the Philippine CPA Licensure Examination (CPALE) Business Law and Taxation subject — specifically its business law component — to existing skill modules. For all substantive analysis, load the routed module. Do not derive legal conclusions from this file.

**Exam authority**: Professional Regulation Commission (PRC) and Board of Accountancy (BOA). The BOA Table of Specifications (TOS) for the business law component covers obligations and contracts, partnerships, corporations, negotiable instruments, insurance, banking, and selected special laws. Verify the current year's PRC-BOA TOS; BOA revises the TOS periodically.

---

## CPALE Business Law — Subject Overview

CPALE Business Law examines the legal framework within which business transactions in the Philippines occur. It tests NCC obligations and contracts as the foundational private law layer, then tests the special commercial statutes that modify or supplement that layer. Unlike the Bar, the CPALE does not test criminal law, remedial law, or political law. The emphasis is on transaction-level legal analysis: capacity, consent, corporate structure, liability, and enforcement.

---

## Module Routing by Topic

### Obligations and Contracts (NCC Book IV)

| Coverage Area | Module | Notes |
|---|---|---|
| Obligations: sources, types, effects, extinguishment | core/obligations-contracts | — |
| Contracts: essential requisites, perfection, defects | core/obligations-contracts | — |
| Specific named contracts: sales, lease, agency, loan, deposit | core/obligations-contracts | ⚠️ See gap notice below |
| Quasi-contracts | core/obligations-contracts | — |
| Quasi-delicts / torts / damages | core/obligations-contracts | core/jurisprudence |
| Contract interpretation, novation, rescission, annulment | core/obligations-contracts | core/statutory-interpretation |

**High-frequency CPALE topics**: void vs. voidable vs. rescissible contracts; essential requisites of a valid contract; effect of simulation; modes of extinguishing obligations; solidary vs. joint obligations; damages (actual, moral, nominal, exemplary).

> **GAP NOTICE**: `core/obligations-contracts.md` covers NCC Book IV comprehensively. However, named contract depth (agency authority limits, contract of sale vs. contract to sell, commodatum vs. mutuum distinctions at the level of CPALE coverage) is partially addressed. Where NCC Book IV named contracts require deeper routing, note that `civil-law/` (planned) will expand this coverage. For CPALE purposes, `core/obligations-contracts.md` is sufficient for most query types.

---

### Partnership Law

| Coverage Area | Module | Notes |
|---|---|---|
| Nature and formation of partnership | commercial-law/partnership-law | — |
| General vs. limited partnership | commercial-law/partnership-law | — |
| Rights and obligations of partners | commercial-law/partnership-law | — |
| Dissolution and winding up | commercial-law/partnership-law | — |
| Partnership vs. corporation distinctions | commercial-law/partnership-law | commercial-law/corporation-law |
| Industrial partner restrictions | commercial-law/partnership-law | — |

**High-frequency CPALE topics**: liability of general vs. limited partners to third persons; effect of apparent authority; distinction between dissolution and termination; partnership by estoppel.

---

### Corporation Law (Revised Corporation Code)

| Coverage Area | Module | Notes |
|---|---|---|
| Nature, classification, and incorporation | commercial-law/corporation-law | — |
| One Person Corporation (OPC) | commercial-law/corporation-law | — |
| Board of directors: powers, duties, BJR, fiduciary duties | commercial-law/corporation-law | — |
| Stockholder rights: voting, inspection, pre-emptive, appraisal | commercial-law/corporation-law | — |
| Corporate powers: express, implied, ultra vires | commercial-law/corporation-law | — |
| Capital structure: authorized, subscribed, paid-up capital | commercial-law/corporation-law | — |
| Mergers, consolidations, dissolution | commercial-law/corporation-law | — |
| Piercing the corporate veil | commercial-law/corporation-law | core/jurisprudence |
| Close corporations | commercial-law/corporation-law | — |
| Foreign corporations | commercial-law/corporation-law | immigration/alien-admission |

**High-frequency CPALE topics**: business judgment rule; derivative suit (requisites); watered stock liability; de facto corporation doctrine; close corporation stockholder direct management; appraisal right trigger events.

---

### Banking Law

| Coverage Area | Module | Notes |
|---|---|---|
| General Banking Law (R.A. 8791) | commercial-law/banking-finance | — |
| BSP authority and supervision | commercial-law/banking-finance | core/administrative-law |
| Types of banks and quasi-banks | commercial-law/banking-finance | — |
| Bank secrecy (R.A. 1405, FCDA) | commercial-law/banking-finance | — |
| PDIC coverage and limits | commercial-law/banking-finance | — |
| Bank conservatorship and liquidation | commercial-law/banking-finance | — |
| AMLA (R.A. 9160 as amended): covered transactions, suspicious transactions | financial-regulation/anti-money-laundering | ✅ See updated gap notice above |

**High-frequency CPALE topics**: exceptions to bank secrecy; PDIC insured deposit amount; distinction between deposit substitutes and deposit accounts; BSP Monetary Board receivership power; AMLA covered institution obligations.

> **GAP NOTICE — RESOLVED (Phase 13)**: Full AMLA doctrine is now covered by `financial-regulation/anti-money-laundering.md` (AMLC authority, freeze orders, civil forfeiture, predicate offenses, covered/suspicious transactions, criminal penalties). `commercial-law/banking-finance.md` retains the banking-compliance-operations layer (KYC, BSP Circular requirements). Both modules cross-referenced; no duplication.

---

### Securities Regulation Code

| Coverage Area | Module | Notes |
|---|---|---|
| SRC registration requirements | commercial-law/securities-law | — |
| Exempt securities and exempt transactions | commercial-law/securities-law | — |
| Manipulation and insider trading | commercial-law/securities-law | — |
| Proxy solicitation and tender offers | commercial-law/securities-law | — |
| SEC adjudicatory jurisdiction | commercial-law/securities-law | core/administrative-law |

**High-frequency CPALE topics**: elements of insider trading; material non-public information; distinction between exempt securities and exempt transactions; tender offer threshold; SRC §57 penalties.

---

### Insurance Law

| Coverage Area | Module | Notes |
|---|---|---|
| Insurable interest (life, property) | commercial-law/insurance-law | — |
| Concealment, representation, warranties | commercial-law/insurance-law | — |
| Double insurance and over-insurance | commercial-law/insurance-law | — |
| Subrogation | commercial-law/insurance-law | core/obligations-contracts |
| Life vs. non-life insurance | commercial-law/insurance-law | — |
| Claims settlement and the Insurance Commission | commercial-law/insurance-law | core/administrative-law |
| Cancellation requirements | commercial-law/insurance-law | — |

**High-frequency CPALE topics**: insurable interest in life insurance (unlimited) vs. property insurance (extent of interest); effect of concealment vs. misrepresentation; constructive total loss; return of premium; CTPL as compulsory insurance.

---

### Negotiable Instruments Law (NIL)

| Coverage Area | Module | Gap Flag |
|---|---|---|
| Requisites of negotiability | negotiable-instruments/general-provisions | ✅ RESOLVED |
| Indorsement types and effects | negotiable-instruments/negotiation-and-holders | ✅ RESOLVED |
| Holder in due course (HDC) | negotiable-instruments/negotiation-and-holders | ✅ RESOLVED |
| Defenses (real vs. personal) | negotiable-instruments/negotiation-and-holders | ✅ RESOLVED |
| Liability of parties: maker, drawer, acceptor, indorser | negotiable-instruments/liabilities-and-discharge | ✅ RESOLVED |
| Presentment, dishonor, notice | negotiable-instruments/liabilities-and-discharge | ✅ RESOLVED |
| Check clearing; stale/crossed checks | negotiable-instruments/checks-and-special-rules | ✅ RESOLVED |
| BP 22 criminal liability | special-laws/special-penal-laws | ✅ RESOLVED (pre-existing; cross-referenced, not duplicated) |

> **GAP NOTICE — RESOLVED (Phase 11)**: Negotiable Instruments Law is now covered by `negotiable-instruments/` (4 modules: general-provisions, negotiation-and-holders, liabilities-and-discharge, checks-and-special-rules; Act No. 2031). `special-laws/special-penal-laws.md` continues to cover BP 22 (Bouncing Checks Law) criminal elements separately — the civil/commercial NIL layer and the criminal BP 22 layer are cross-referenced, not merged, to avoid doctrine duplication.

---

### Intellectual Property Code

| Coverage Area | Module | Notes |
|---|---|---|
| Copyright: automatic protection, economic rights, fair use | intellectual-property/copyright | — |
| Trademarks: registration, dominancy test, infringement | intellectual-property/trademarks | intellectual-property/unfair-competition |
| Patents: patentability, utility models, IPOPHL | intellectual-property/patents | — |
| Unfair competition: passing off, trade secrets | intellectual-property/unfair-competition | core/obligations-contracts |

**High-frequency CPALE topics**: copyright protection without registration; trademark dominancy test vs. holistic test; prior art; patent licensing and compulsory licensing; trade secret protection under IPC §168 vs. obligations/contracts.

---

### Other Special Laws (CPALE Scope)

| Coverage Area | Module | Gap Flag |
|---|---|---|
| Electronic Commerce Act (R.A. 8792) | — | ⚠️ No module exists |
| Data Privacy Act (R.A. 10173) | — | ⚠️ No module exists |
| Anti-Cybercrime Law (R.A. 10175) — civil aspects | special-laws/special-penal-laws | Penal aspects only; no dedicated module |
| Consumer Act (R.A. 7394) | — | ⚠️ No module exists |
| AMLA (full doctrine) — Phase 13 | ✅ RESOLVED | 1 module built and routed: financial-regulation/anti-money-laundering |

---

## Module Loading Order for CPALE Business Law Queries

Obligations/contracts → `core/obligations-contracts.md`.
Partnership → `commercial-law/partnership-law.md`.
Corporation → `commercial-law/corporation-law.md`.
Corporation + obligations interplay (ultra vires contracts) → load both.
Banking → `commercial-law/banking-finance.md`; add `core/administrative-law.md` for BSP regulatory queries.
Securities → `commercial-law/securities-law.md`.
Insurance → `commercial-law/insurance-law.md`; add `core/obligations-contracts.md` for subrogation and warranty analysis.
IP → load relevant `intellectual-property/` module.
NIL → load relevant `negotiable-instruments/` module (general-provisions, negotiation-and-holders, liabilities-and-discharge, or checks-and-special-rules per sub-topic); add `special-laws/special-penal-laws.md` for BP 22 criminal liability queries.

---

## Gap Summary

| Gap | Severity | Dependency |
|---|---|---|
| Negotiable Instruments Law — Phase 11 | ✅ RESOLVED | 4 modules built and routed |
| E-Commerce Act (R.A. 8792) | MEDIUM | Phase TBD |
| Data Privacy Act (R.A. 10173) | MEDIUM | Phase TBD |
| `financial-regulation/anti-money-laundering.md` — Phase 13 | ✅ RESOLVED | 1 module built and routed |
| Consumer Act (R.A. 7394) | LOW | Phase TBD |
| Named contracts depth (civil-law/) | LOW — obligations-contracts.md covers CPALE scope adequately | Phase 8 civil-law |
