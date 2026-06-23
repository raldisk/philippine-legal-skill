# CPALE Taxation Track — CPA Licensure Examination

## Purpose and Constraint

**Overlay only.** This file contains no doctrine. It maps the Philippine CPA Licensure Examination (CPALE) Taxation subject to existing skill modules. For all substantive analysis, load the routed module. Do not derive legal conclusions from this file.

**Exam authority**: Professional Regulation Commission (PRC) and Board of Accountancy (BOA). Coverage areas below follow the BOA Table of Specifications (TOS) for the Taxation subject. Verify the current year's PRC-BOA TOS for weight adjustments; the BOA revises the TOS periodically.

---

## CPALE Taxation — Subject Overview

CPALE Taxation examines knowledge of Philippine national and local tax laws, BIR administration, and tax remedies. The examination tests both substantive law (liability computation) and procedural law (assessment, protest, refund, appeals). Doctrine matters: examinees must apply statutory provisions and reconcile TRAIN Act (R.A. 10963) amendments against pre-TRAIN rules.

---

## Module Routing by Topic

### Income Tax

| Coverage Area | Module | Notes |
|---|---|---|
| Tax classification (individual, corporate, partnership, estate, trust) | taxation/income-taxation | — |
| Gross income inclusions and exclusions | taxation/income-taxation | — |
| Allowable deductions (OSD vs. itemized) | taxation/income-taxation | — |
| Minimum corporate income tax (MCIT) | taxation/income-taxation | — |
| Final withholding tax and creditable withholding tax | taxation/income-taxation | taxation/tax-administration |
| Fringe benefit tax | taxation/income-taxation | — |
| Capital gains tax (real property, shares) | taxation/income-taxation | — |
| Special income tax regimes (PEZA, TIEZA, BOI) | taxation/income-taxation | taxation/tax-administration |
| TRAIN Act adjustments (R.A. 10963) | taxation/income-taxation | taxation/tax-administration |
| CREATE Act adjustments (R.A. 11534) | taxation/income-taxation | — |

**High-frequency CPALE topics**: gross income vs. net income vs. taxable income distinction; OSD computation; MCIT vs. regular corporate income tax; interplay of withholding taxes with annual income tax; TRAIN rate schedules for individual taxpayers; passive income tax rates.

---

### Value-Added Tax

| Coverage Area | Module | Notes |
|---|---|---|
| VAT-registered vs. non-VAT persons | taxation/value-added-tax | — |
| VAT-taxable transactions (sale, lease, importation) | taxation/value-added-tax | — |
| Zero-rated sales (export, PEZA-registered) | taxation/value-added-tax | — |
| VAT-exempt transactions | taxation/value-added-tax | — |
| Input tax creditable vs. non-creditable | taxation/value-added-tax | — |
| Input tax carry-over and refund procedure | taxation/value-added-tax | taxation/tax-remedies |
| Percentage tax (non-VAT persons) | taxation/value-added-tax | — |
| Monthly and quarterly VAT filing | taxation/value-added-tax | taxation/tax-administration |

**High-frequency CPALE topics**: VAT threshold (₱3 million); input-output credit mechanism; VAT treatment of services rendered to non-residents; VAT refund vs. tax credit certificate; distinction between zero-rating and exemption.

---

### Estate Tax and Donor's Tax

| Coverage Area | Module | Notes |
|---|---|---|
| Estate tax: gross estate inclusions | taxation/estate-donor-tax | — |
| Estate tax: allowable deductions (funeral, judicial, claims, family home) | taxation/estate-donor-tax | — |
| Estate tax: net estate computation and rate (flat 6% post-TRAIN) | taxation/estate-donor-tax | — |
| Estate tax: filing deadline and extension | taxation/estate-donor-tax | taxation/tax-administration |
| Estate tax amnesty (R.A. 11213, as extended) | taxation/estate-donor-tax | — |
| Donor's tax: coverage, exemptions, rate (flat 6% post-TRAIN) | taxation/estate-donor-tax | — |
| Donation to government and accredited NGOs | taxation/estate-donor-tax | — |
| Succession planning: interplay with Civil Code legitimes | taxation/estate-donor-tax | special-laws/succession-inheritance |

**High-frequency CPALE topics**: family home deduction cap; distinction between conjugal and exclusive properties in estate; vanishing deduction; donor's tax exemption threshold (₱250,000 per year); estate tax amnesty coverage and filing.

---

### Local Taxation

| Coverage Area | Module | Notes |
|---|---|---|
| Local business tax (LGC §§143–151) | taxation/local-taxation | core/local-government-law |
| Real property tax (basic RPT + SEF levy) | taxation/local-taxation | — |
| Community tax certificate | taxation/local-taxation | — |
| LGU tax ordinance power and limitations | taxation/local-taxation | core/local-government-law |
| Tax exemptions under LGC | taxation/local-taxation | — |

**High-frequency CPALE topics**: LGU real property tax rate ceilings; special education fund levy; assessment levels and fair market value; LGU tax situs rules; local tax ordinance publication requirements.

---

### Tax Remedies

| Coverage Area | Module | Notes |
|---|---|---|
| Assessment process: LOA, PAN, FAN, FLD | taxation/tax-remedies | taxation/tax-administration |
| Statute of limitations on assessment (3 yr / 10 yr) | taxation/tax-remedies | — |
| Protest: request for reconsideration vs. request for reinvestigation | taxation/tax-remedies | — |
| Inaction as denial; 30-day appeal period to CTA | taxation/tax-remedies | — |
| Collection: distraint and levy; civil action; criminal action | taxation/tax-remedies | — |
| Tax refund: administrative claim first; 2-year prescriptive period | taxation/tax-remedies | — |
| CTA jurisdiction: Division vs. En Banc; timeliness | taxation/tax-remedies | — |
| Compromise and abatement | taxation/tax-remedies | taxation/tax-administration |

**High-frequency CPALE topics**: when does the prescriptive period for assessment begin; effect of waiver of statute of limitations; distinction between collection by distraint/levy and civil/criminal action; CTA Division vs. CTA En Banc as to appeals from BIR, BOC, and LGU.

---

### Tax Administration

| Coverage Area | Module | Notes |
|---|---|---|
| BIR organizational structure and powers | taxation/tax-administration | — |
| Registration, bookkeeping, invoicing requirements | taxation/tax-administration | — |
| Examination of returns and issuance of LOA | taxation/tax-administration | taxation/tax-remedies |
| Subpoena duces tecum; summons | taxation/tax-administration | — |
| Criminal violations: tax evasion, falsification, failure to file | taxation/tax-administration | — |
| TRAIN Act administrative provisions | taxation/tax-administration | — |
| Electronic filing and payment | taxation/tax-administration | — |

**High-frequency CPALE topics**: LOA vs. mission order; effect of LOA not signed by CIR or authorized official; timeline for issuance of PAN and FAN; surcharge and interest computations under R.A. 10963.

---

## Module Loading Order for CPALE Taxation Queries

Single-topic query → load the single routed module above.

Cross-topic query (e.g., "estate tax computation with CTA appeal"): load `taxation/estate-donor-tax.md` + `taxation/tax-remedies.md` in that order.

Assessment/remedies queries almost always require both `taxation/tax-remedies.md` and `taxation/tax-administration.md` simultaneously — load both.

Estate/succession interplay: add `special-laws/succession-inheritance.md` for legitime and partition issues.

---

## Gap Summary

No gaps within the CPALE Taxation scope. All six taxation modules (`income-taxation`, `value-added-tax`, `estate-donor-tax`, `local-taxation`, `tax-remedies`, `tax-administration`) are fully built. Cross-references to `special-laws/succession-inheritance.md` and `core/local-government-law.md` resolve correctly.

| Check | Result |
|---|---|
| All taxation/ modules present | ✅ |
| Estate/succession cross-reference | ✅ special-laws/succession-inheritance.md exists |
| Local government cross-reference | ✅ core/local-government-law.md exists |
| AMLA/banking cross-reference needed? | N/A — not in CPALE Taxation scope |
