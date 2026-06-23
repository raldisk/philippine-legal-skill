# Crisis Frameworks Module

## Confidence Scale

Apply this scale to every legal conclusion. The score must match the actual quality and quantity of authority — never inflate to project certainty.

| Score | Meaning |
|---|---|
| 95–100 | Settled constitutional doctrine; controlling en banc decisions; no conflicting authority |
| 80–94 | Strong controlling authority; minor doctrinal ambiguity at edges |
| 60–79 | Competing authority exists; conflicting en banc decisions or unresolved tension |
| 40–59 | Novel issue; no directly controlling authority; analogical reasoning required |
| 20–39 | Highly uncertain; doctrine in flux; multiple plausible outcomes |
| 0–19 | No reliable authority; purely speculative analysis |

---

## Supreme Court Outcome Prediction Framework

Use this structure when asked to predict whether the Supreme Court would uphold or strike down an act, and on what grounds.

**Step 1 — Standing analysis**: Does the petitioner have (a) personal and substantial interest, (b) injury in fact, (c) traceability, (d) redressability? Note that the Court may relax standing for transcendentally important constitutional questions (*David*).

**Step 2 — Ripeness**: Is there a concrete dispute or is it premature? Courts will not issue advisory opinions.

**Step 3 — Mootness**: Is the issue moot? Apply the *David* exceptions: (a) grave constitutional violation; (b) exceptional character requiring definitive doctrine; (c) public interest; (d) capable of repetition yet evading review.

**Step 4 — Political question**: Is the matter textually committed to another branch with no judicially manageable standards? Under the expanded judicial review clause, this doctrine is narrow. If grave abuse of discretion is alleged, the Court almost always reaches the merits.

**Step 5 — Merits assessment**:
- Identify the constitutional provision allegedly violated
- Identify the strongest argument for petitioner
- Identify the strongest argument for respondent
- Apply the doctrinal test most likely to be used by the Court
- Assess likely doctrinal basis of decision

**Step 6 — Confidence score**: Apply the scale above.

**Output format**:
- Justiciability: [likely dismissed / likely reached on merits / uncertain] + confidence
- Petitioner's strongest argument: [statement]
- Respondent's strongest argument: [statement]
- Most likely doctrinal basis if merits are reached: [statement]
- Predicted outcome: [uphold / strike down / partial] + confidence
- Key uncertainty: [what fact or doctrine is pivotal]

---

## Senate Leadership Dispute Framework

For any Senate President election or removal dispute, analyze in this sequence:

**Constitutional layer**:
- Article VI, §16(1): each House elects its own officers from among its members
- Article VI, §16(2): quorum requirement
- Expanded judicial review (Article VIII, §1): Court may examine grave abuse of discretion

**Institutional rules layer**:
- What are the Senate's current rules of procedure?
- Are those rules validly adopted?
- Was the election/removal conducted in compliance with the rules?
- Was there a quorum? (Compute from all 24 senators per *Avelino*)

**Doctrinal analysis**:
- *Avelino v. Cuenco* (1949): quorum = majority of all members; Court may decline if purely political but will intervene for constitutional violations
- Post-*Francisco* doctrine: expanded judicial review permits Court to examine if grave abuse of discretion attended the process
- Continuing body doctrine: Senate rules carry over between Congresses; House rules do not

**Strongest argument for the ousted Senate President**:
Examine whether (a) the quorum was insufficient, (b) the Senate's own rules were violated, (c) the removal was in bad faith or for constitutionally impermissible reasons, (d) the expanded judicial review clause empowers the Court to examine procedural validity.

**Strongest argument for the successor**:
Examine whether (a) the required votes were present, (b) quorum was satisfied, (c) internal Senate matters are beyond judicial reach absent grave abuse, (d) political confidence of the Senate majority should not be judicially overridden.

**Most likely SC position**: The Court will likely find the matter justiciable under expanded judicial review, examine whether quorum and rule compliance were satisfied, and uphold the result if a proper quorum voted in compliance with Senate rules, declining to examine the political motivations behind the leadership change.

---

## Impeachment Crisis Framework

When an impeachment proceeding is contested or produces a constitutional crisis:

**Key questions**:
1. Was the one-year bar complied with? (*Francisco*: bar runs from filing, not from committee referral)
2. Was the complaint sufficient in form and substance? (Jurisdictional prerequisite)
3. Were Articles of Impeachment properly passed? (One-third of all House members)
4. Is the Senate conducting a proper trial? (Article XI, §3 requirements)
5. Is the two-thirds conviction threshold constitutionally fixed? (Yes — cannot be reduced by Senate rules)

**Judicial review of impeachment**: *Francisco* held that courts may examine whether the one-year bar has been violated (a constitutional requirement), even though the substance of impeachment is a political question. This limited but established the principle that at least some aspects of impeachment are judicially reviewable.

**Quo warranto risk** (*Sereno*): An impeachable officer facing difficulty in the House may face a quo warranto challenge in the SC. *Sereno*'s holding that quo warranto is available for qualification defects — distinct from impeachable offenses — remains controversial. Confidence in quo warranto as alternative to impeachment: [60–70].

---

## Constitutional Crisis Simulator

For any constitutional crisis, generate the following analysis:

**Legal trigger**: What specific act or omission triggered the crisis? Identify the constitutional provision at issue.

**Constitutional provisions implicated**: List all relevant Articles and Sections.

**Institutional actors**: Identify each branch's role, interest, and available legal tools.

**Available legal remedies**:
- Petition for certiorari / prohibition / mandamus before the SC
- Impeachment proceeding
- Legislative resolution or legislation
- Presidential proclamation or executive action
- COMELEC or electoral tribunal action (if election-related)

**Judicial intervention likelihood**: Based on justiciability analysis (steps 1–4 above).

**Best-case outcome**: Resolution through constitutional processes with legal clarity.

**Worst-case outcome**: Constitutional impasse, competing claimants, institutional breakdown.

**Most likely outcome**: Based on Philippine institutional precedent and current Court composition's doctrinal tendencies.

**Confidence score**: Apply scale above.

---

## Political Legitimacy vs. Legal Validity — Mandatory Separation

These three categories must always be analyzed separately. Conflating them is analytical error.

**Legal validity**: Does the act comply with the Constitution and applicable statutes? Determined by constitutional and statutory analysis.

**Procedural validity**: Was the act done through the proper process? Determined by rules of procedure and constitutional requirements.

**Political legitimacy**: Do affected constituencies and the public accept the act as legitimate? This is a political and sociological question, not a legal one.

An act may be legally valid but politically illegitimate (*e.g.*, a technically lawful but widely condemned executive order). An act may be politically popular but legally invalid (*e.g.*, a popular but unconstitutional statute). Legal analysis addresses only the first two categories; political legitimacy may be noted separately as context.

---

## Administrative Law Submodule

**Due process in administrative proceedings**: *Ang Tibay v. Court of Industrial Relations* (69 Phil. 635, 1940) established **seven** cardinal primary rights in administrative proceedings: (1) right to a hearing; (2) the tribunal must consider the evidence presented; (3) decision must be based on evidence presented at the hearing; (4) the tribunal must act on its own independent consideration of the law and facts, not merely accept a subordinate's unchallenged report; (5) decision must be rendered in such a manner that parties know the issues and the reason for the decision; (6) evidence must be substantial — such relevant evidence as a reasonable mind might accept as adequate; (7) decision must be rendered on the evidence presented at the hearing. Load `references/administrative-law.md` for full analysis. *Note: The count is seven, not eight — independence of judgment is part of right (4), not a separate right.*

**Judicial review of administrative decisions**: Doctrine of primary jurisdiction — courts will not interfere with the exercise of administrative functions before the agency exhausts its authority. Exhaustion of administrative remedies required before court review, subject to exceptions (*e.g.*, pure question of law, urgent necessity, denial of due process).

**Grave abuse of discretion standard**: Courts review administrative decisions for grave abuse of discretion amounting to lack of jurisdiction. This is a narrow standard — courts do not substitute their judgment on technical matters within agency expertise.
## Anti-Hallucination Guardrails — Crisis Frameworks

The confidence scale assigns scores based on quality of authority, not on political confidence in an outcome — never inflate a score to project certainty where the law is genuinely unsettled. Never state that the *Avelino* quorum doctrine was decided under the 1987 Constitution — it was a 1935 Constitution case; the doctrine applies by analogy because the quorum language is substantially identical. Never claim the Supreme Court has ruled on any specific current political controversy without verifying — the Court's docket changes rapidly and an SC ruling that exists as of one date may be superseded by a rehearing or a new en banc decision. The political question doctrine is narrow post-1987; do not apply it to avoid analysis of any action that involves a government branch. Always distinguish legal validity from political legitimacy — they are analytically independent and must be stated separately.
