# Quality Review — Revision 4 / Content Audit

**Date:** 2026-11-23. **Normative control:** Master Curriculum Control v2.0 (21 Nov 2026), lesson index page 6; Blueprint page 3; evidence standards page 4. **Source baseline:** actual local Revision 3 ZIP, not a guess about GitHub contents.

## Decision

**CONDITIONAL / substantive editorial improvement, NOT an unconditional scientific PASS.** We performed a targeted claim-to-source audit and corrected a concrete imbalance in Lesson 005. Five lessons received additional developed mechanistic walkthroughs. Bibliographic identifiers mentioned in the new audit were checked against public PubMed/publisher records. This is NOT an exhaustive sentence-by-sentence full-text literature audit and NOT an independent specialist peer review. Publishing without that further review is an editorial decision, not proof of scientific completeness.

## Concrete findings and corrections

| Lesson | Prior gap | Revision 4 action | Assessment |
|---|---|---|---|
| 001 | Connections between changing demand, effector response, and observation were stated but not developed through a multi-level example | Added a staged causal walkthrough and counterexample that organ outputs need not change together | Improved; illustrative, not experimental proof |
| 002 | The one-neuron/two-neuron distinction was accurate but relatively static | Followed motor commands to specific effectors and separated automatic behavior from anatomical motor route | Improved |
| 003 | Bidirectional communication was laid out but readers could still merge sensory input with motor output | Added five distinct stages and an explicit critique of one-to-one reflex inference | Improved; no full reflex circuit taught prematurely |
| 004 | Ganglia were named but the consequences of different branching routes were under-explained | Added paravertebral, prevertebral and adrenal-medulla route comparison, maintaining 01.08 scope boundary | Improved; specialized transmitter pharmacology deferred |
| 005 | Sacral reclassification evidence was inadequately balanced by an explicit opposing academic position | Added named published counterarguments (2017, 2018), clarified species/model limitations, and expanded the cranial-route mechanism | Corrected key scientific balance issue |

## Internal Blueprint — identity, learning outcomes, scope

| ID | Leading concept | Internal verifiable learning outcome | Dependency | Deferred |
|---|---|---|---|---|
| 01.01 | Autonomic regulation | Differentiate signal, effector, function and experience using one contextual example | None | Specific reflexes, homeostasis and allostasis |
| 01.02 | Somatic vs autonomic motor output | Identify route and effector; explain why automatic breathing is not automatically autonomic motor innervation | 01.01 | Detailed respiratory control |
| 01.03 | Visceral afference/efference | Trace both directions, distinguish sensory input from motor output and conscious experience | 01.02 | Visceral reflex architecture, conscious interoception |
| 01.04 | Sympathetic organization | Trace thoracolumbar and three peripheral route variants; reject a global fight-or-flight definition | 01.03 | Transmitter pharmacology, stress response |
| 01.05 | Parasympathetic organization | Trace classical cranial pathways; distinguish anatomical evidence from contested sacral naming | 01.03, 01.04 | Full vagus anatomy and organ-specific receptor effects |

## Evidence Map — audited claim groups (claim-status, not author-status)

| Claim | Evidence / DOI | Data type | Status | Limit and audit result |
|---|---|---|---|---|
| ANS controls non-skeletal visceral effectors, multiple routes | Wehrwein 2016, `10.1002/cphy.c150037`; McCorry 2007, `10.5688/aj710478` | Academic reviews | A | Reviewed bibliographic identity; no claim all organs depend exclusively on ANS |
| Organ-specific sympathetic outputs | Morrison 2001, `10.1152/ajpregu.2001.281.3.R683`; Gibbins 2013, `10.4161/org.25126` | Physiological and anatomical reviews | A | Not a universal autonomic activation index |
| Motor systems differ in typical effector and relay | McCorry 2007; Wehrwein 2016 | Academic reviews | A | Does not imply voluntary/involuntary dichotomy |
| Visceral inputs and autonomic efferents are different directions | Berthoud & Neuhuber 2000, `10.1016/S1566-0702(00)00215-0`; Berthoud et al. 2025, `10.1016/j.conb.2025.103058` | Animal-heavy anatomical and integrative reviews | A | Detailed afferent maps are not direct evidence of human conscious sensations |
| Sensation cannot identify one precise route | Craig 2002, `10.1038/nrn894`; Berthoud et al. 2025 | Model/review | B | Mechanistic plausibility, not a direct human decoding test |
| Sympathetic chain and collateral routes | Wehrwein 2016; McCorry 2007 | Academic reviews | A | A teaching simplification; exceptions include adrenal medulla |
| Distinct sympathetic outputs during ordinary functions | Morrison 2001; Iriki & Simon 2012, `10.1007/s12576-012-0208-9` | Review of human/animal physiology | A | Does not assign emotions from skin or heart signals |
| Sacral autonomic naming may be changed on molecular/developmental criteria | Espinosa-Medina et al. 2016, `10.1126/science.aah5454` | Primary mouse study | C for general reclassification | The empirical animal data do not automatically settle human nomenclature |
| Sacral relabeling has substantive published objections | Neuhuber et al. 2017, `10.1002/ar.23600`; Jänig et al. 2018, `10.1007/s10286-017-0491-x` | Expert argument/commentary | C | Counterpositions are not independent experimental disproof |
| „Fight or flight“ / „rest and digest“ as universal descriptions | Gibbins 2013; Wehrwein 2016 | Conceptual simplifications compared with physiology | D | Not mechanistic laws |

### Verification boundary

The identities/DOIs for Wehrwein, Gibbins, Morrison, Iriki & Simon, Berthoud et al. (2025), Espinosa-Medina, Neuhuber et al. and Jänig et al. were checked against public indexed publication records during this edit. Other citations are retained from Revision 3; this review **does not claim** their full text was newly inspected. Primary-versus-review labeling follows article type where observable. The brief academic comments on the sacral debate are explicitly marked as positions, not experiments. Do not upgrade claim-status merely because multiple authors agree.

## Safety and teaching scope

001 includes low-risk observation without a claim of training efficacy. 002–005 use conceptual checks in place of physiological manipulations; no vagal stimulation, carotid pressure, breath-holding or diagnostic procedures. No emotional state is inferred from single peripheral output. Neurotransmitter mechanisms are held for 01.08; full autonomic reflex organization for 01.11; vagus specifics for 01.06; functional sympathetic–parasympathetic coordination for 01.12.

## Automated verification vs editorial verification

Structural script: five ordered files; seven published sections each; internal linked Markdown paths resolve; no obsolete `преколатерални`; each file includes a new mechanistic section; nonempty Markdown; ZIP integrity tested. **These automated results do not certify scientific accuracy.**

## Unresolved before an unconditional academic-quality PASS

1. Audit every distinct empirical claim against the relevant passage of full academic text, including potential contradictions in recent literature; log page/section rather than DOI existence alone.
2. Seek qualified independent domain review where academic publication assurance is required.
3. Run pedagogical comprehension testing with readers new to physiology; self-check questions are not evidence that learning occurred.
4. GitHub byte-for-byte comparison was **not performed** because the repository baseline was not provided in this task. Use the supplied manifest and diff against the actual checked-out files.
