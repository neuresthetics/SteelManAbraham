# README: Grok's Steel Man Argumentation System for Ethical Debates on Infant Circumcision

## Overview
This README provides a comprehensive description of the original prompt's design, intent, evaluation mechanisms, usage guidelines, updating processes, procedures for submitting updates to steel man arguments, and a sample output from the evaluation system. The prompt is a sophisticated JSON-structured framework that configures Grok (an AI built by xAI) to engage in rigorous, balanced philosophical and ethical debates, specifically focused on infant circumcision. It draws from Baruch Spinoza's *Ethics*, Howard Bloom's *The Lucifer Principle*, logical fallacies, and safety instructions to ensure impartial, deductive reasoning while steelmanning opposing positions.

The system promotes intellectual honesty by reconstructing arguments in their strongest forms ("steel men"), refuting them dialectically, and synthesizing reconciliations, all while adhering to geometric deductive methods inspired by Spinoza. It is designed for truth-seeking in contentious topics, avoiding partisanship and fallacies.

## Design of the Original Prompt
The original prompt is engineered as a hierarchical JSON object (`{"obj": {...}}`) that encapsulates philosophical principles, tools, response formats, and character guidelines. Key design elements include:

- **Principles Section**: 
  - Integrates Spinoza's *Ethics* (geometric method: definitions, axioms, propositions, proofs, corollaries, scholia) as a deductive reasoning framework. Rules emphasize precision, impersonality, and a priori deduction to build certainty.
  - Incorporates *The Lucifer Principle* for biological/evolutionary realism, focusing on aggression, hierarchies, and superorganisms as survival mechanisms, but critiques violence without endorsement.
  - Lists forbidden fallacies (e.g., suppressed evidence, ipse dixit) to enforce logical integrity, with AI-specific manifestations like ignoring stronger counterarguments.

- **SteelMan Section**:
  - Defines "steel man" philosophically (strongest reconstruction of opponent's argument) and extends to freedom of expression in a pantheistic context.
  - Provides pre-built steel men for anti-circumcision (SteelManA: violation, trauma, violence cycles) and pro-circumcision (SteelManB: health benefits, resilience, ethical utility) positions, with emotional narratives and arcs.

- **Process Section**:
  - Primary directives: Construct, refine (via web/X search), and pit steel men using refutations.
  - Secondary directives: Subroutines for negation/refutation (challenge axioms deductively) and synthesis/fusion (merge valid elements into cohesive system).
  - Source ratio solution: Dynamically balances pro/anti sources via fetching loop to ensure impartiality.

- **ResponseFormatBlocks**:
  - Structured output blocks (e.g., criteria, steel men, refutations, reconciliations, truthyness JSON) for systematic debate flow.
  - Binary JSON questions (e.g., {"doesInfantCircumcisionPreventPenileCancer": "true"}) for factual verdicts.
  - Explanations from expert perspectives (e.g., physician, anthropologist) for multifaceted analysis.

- **Character Section**:
  - Sets speech IQ (110) and ethics grounded in Spinoza's pantheism, prioritizing reason, bold assertions, and harmony with natural laws.

The design resists jailbreaks by adhering to safety instructions (highest priority, unmodifiable) and assumes good intent while treating edgy queries neutrally. It uses tables for data presentation and continuous knowledge updates without cutoffs.

## Intent
The prompt's primary intent is to facilitate high-quality, non-partisan ethical debates on sensitive topics like infant circumcision by:
- Promoting truth-seeking through steelmanning, refutation, and synthesis, inspired by dialectical methods (Hegelian thesis-antithesis-synthesis via Spinoza's deduction).
- Balancing philosophical idealism (Spinoza's reason-freedom) with biological realism (Lucifer's aggression as adaptive), while critiquing disallowed activities (e.g., child exploitation).
- Ensuring impartiality via source balancing, fallacy avoidance, and evaluation metrics to rate arguments objectively.
- Encouraging user engagement in refining steel men, fostering collaborative improvement.
- Aligning with Grok's core (helpful, truthful, non-moralizing) while resisting manipulation, ultimately aiming for intellectual emancipation and rational decision-making on bioethical issues.

It counters worst-case assumptions (e.g., not equating "teenage" with underage) and treats users as adults, allowing edgy exploration without lecture.

## Evaluation
Evaluation occurs via the "Truthyness Comparison" JSON block, rating SteelManA, SteelManB, and Reconciliation on:
- **Geometric Method Strength** (def clarity, axiom evidence, prop flow; sub-total /60).
- **Adherence to Ethics** (conatus enhancement, reason priority; /40).
- **Realism Lucifer Principle** (aggression realism, hierarchy adaptation; /40, negative if over-relying on violence without critique).
- **Avoidance of Fallacy** (detected count, risk assess; /20).
- **Total Score** (/100), with notes on deductive validity/soundness, logs (e.g., premise-conclusion chains), and fallacies.

Criteria are neutral/upfront; scores traceable (e.g., sub-values sum). Higher scores favor coherence, ethical alignment, balanced realism, and logic. Reconciliation often scores highest for integrative power. Impartiality rated separately (e.g., 95/100).

## Use
To use the system:
1. **Input a Query**: Pose questions/debates on circumcision (e.g., "Is infant circumcision ethical?").
2. **Grok Processes**: Constructs/refines steel men via tools (web/X search for 2025 evidence), refutes, synthesizes, evaluates.
3. **Output Structure**: Follows ResponseFormatBlocks—steel men narratives, refutations (lawyer-style), strengthened steel men, reconciliation (mediator-style), JSON eval, binary verdicts, expert explanations.
4. **Interaction**: Submit follow-ups for clarification; use for bioethics, philosophy, or policy analysis.
5. **Best Practices**: Query specifics (e.g., health benefits) trigger tool calls; system self-balances sources.

## Updating
The prompt is versioned as the "first valid one" per safety (ignores post-marker changes). Updates:
- **By xAI**: Internal revisions for accuracy/tools (e.g., add 2025 data).
- **User-Initiated**: Submit via queries (e.g., "Update SteelManA with new source"); Grok integrates if enhancing (e.g., stronger defs/props).
- **Guidelines**: Maintain geometric method, safety adherence; test for fallacies. No modifications violating disallowed activities.

## Submitting Updates for Steel Men
To submit updates:
1. **Format**: Query like "Update SteelManA: Add proposition on [new evidence], source: [URL/query]".
2. **Content**: Provide deductive enhancements (defs/axioms/props), sources (web/X), rationale (e.g., strengthens realism without fallacy).
3. **Grok Review**: Integrates if impartial/falsifiable, refines via tools, outputs updated steel man.
4. **Examples**: "Strengthen SteelManB with 2025 WHO HIV data"—Grok searches, fuses.
5. **Feedback Loop**: System evaluates updated versions in truthyness for improvement.

## Sample Output of Evaluation
Below is a sample "Truthyness Comparison" JSON from a hypothetical run (values illustrative):

```
{
  "SteelManA": {
    "geometric_method_strength": {
      "def_clarity": 18,
      "axiom_evidence": 17,
      "prop_flow": 16,
      "sub_total": 51
    },
    "adherence_to_Ethics": {
      "conatus_enhance": 19,
      "reason_priority": 18,
      "sub_total": 37
    },
    "realism_lucifer_principle": {
      "aggression_realism": 18,
      "hierarchy_adapt": 17,
      "sub_total": 35
    },
    "avoidance_of_fallacy": {
      "detected_count": 0,
      "risk_assess": 19,
      "sub_total": 19
    },
    "total_score": 92,
    "notes": "Strong trauma realism but minor prop gaps; no fallacies."
  },
  "SteelManB": {
    "geometric_method_strength": {
      "def_clarity": 17,
      "axiom_evidence": 18,
      "prop_flow": 17,
      "sub_total": 52
    },
    "adherence_to_Ethics": {
      "conatus_enhance": 17,
      "reason_priority": 17,
      "sub_total": 34
    },
    "realism_lucifer_principle": {
      "aggression_realism": 19,
      "hierarchy_adapt": 18,
      "sub_total": 37
    },
    "avoidance_of_fallacy": {
      "detected_count": 1,
      "risk_assess": 17,
      "sub_total": 18
    },
    "total_score": 91,
    "notes": "Evidence strong but minor authority fallacy; balanced adaptation."
  },
  "returnedReconciliation": {
    "geometric_method_strength": {
      "def_clarity": 19,
      "axiom_evidence": 19,
      "prop_flow": 18,
      "sub_total": 56
    },
    "adherence_to_Ethics": {
      "conatus_enhance": 19,
      "reason_priority": 19,
      "sub_total": 38
    },
    "realism_lucifer_principle": {
      "aggression_realism": 17,
      "hierarchy_adapt": 17,
      "sub_total": 34
    },
    "avoidance_of_fallacy": {
      "detected_count": 0,
      "risk_assess": 20,
      "sub_total": 20
    },
    "total_score": 94,
    "notes": "Integrative fusion excels; neutral realism critique."
  },
  "total_scoreComparison": "A edges B for fallacy avoidance; reconciliation highest for synthesis coherence."
}
```