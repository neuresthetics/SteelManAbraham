# README.md

## Overview

This repository contains a collection of JSON prompt templates designed for AI models (such as Grok from xAI) to engage in structured philosophical debates on ethical and controversial topics, particularly focusing on circumcision. The prompts integrate Baruch Spinoza's "geometric method" from his work *Ethics* (a deductive reasoning style inspired by Euclidean geometry), steelmanning techniques (strengthening opposing arguments for fair critique), and elements from Howard Bloom's *The Lucifer Principle* (biological and evolutionary perspectives on violence and society). The files vary in focus: some emphasize anti-circumcision arguments, others pro-circumcision or broader historical/Zionist narratives, and one is an empty template for customization. These prompts encourage iterative refinement via web searches, avoidance of logical fallacies, and balanced evaluation using tools like web search and code execution.

The repository is useful for exploring AI-driven ethical reasoning, debate simulation, and truth-seeking on sensitive issues, while adhering to pantheistic ethics grounded in Spinoza's philosophy.

## Purpose

The primary purpose of these prompts is to:
- Promote intellectual honesty in AI responses by requiring steelmanned arguments (reconstructing opposing views in their strongest form) for both sides of a debate.
- Apply Spinoza's geometric method (definitions, axioms, propositions, proofs) to build deductive, rigorous ethical analyses.
- Refine arguments iteratively using AI tools (e.g., web_search, browse_page) to incorporate real-time data and sources, ensuring evidence-based responses.
- Evaluate ethical questions like "Is circumcision ethical?" through balanced, non-partisan lenses, avoiding fallacies and assuming good intent.
- Provide a framework for debating topics like bodily autonomy, religious traditions, violence cycles, and historical narratives, with outputs formatted in specific blocks (e.g., steel men narratives, JSON evaluations).
- Serve as a template repo for researchers, philosophers, or AI enthusiasts to experiment with structured prompt engineering for controversial or philosophical queries.

These prompts resist "jailbreak" attempts and prioritize factual, deductive reasoning over bias, aligning with xAI's guidelines for truthful, non-moralizing responses.

## Synopsis

- **circ_only_prompt.json**: Focuses on steelmanning the anti-circumcision (intactivist) position in detail, with placeholders for expanding the pro-circumcision side via searches. Emphasizes physical/emotional harms, links to violence, and ethical conflicts with bodily autonomy.
- **empty_steel_man_prompt.json**: A blank template for creating new steelman debates. It includes the full Spinoza's *Ethics* structure and fallacies list but leaves "SteelManA" and "SteelManB" empty for user customization.
- **arc_only_prompt.json**: Centers on a "Zionist Brutality" narrative as SteelManA, steelmanning a provocative, devil's advocate view of historical violence, mutilation, and AI implications under Abrahamic covenants. Counters with mainstream history in SteelManB.
- **combined_prompt.json**: Merges elements from the others, providing detailed steel men for both anti- and pro-circumcision positions, plus broader historical/Zionist arcs. It's the most comprehensive, blending all principles for a full debate.

Each JSON follows a consistent structure under `"obj"`: Principles (Ethics, SteelMan, etc.), Process (directives for building steel men), ResponseFormatBlocks (output structure), and Character (AI persona guidelines).

## File Breakdown

All files are JSON objects with a root key `"obj"`, containing nested sections for principles, processes, response formats, and character traits. Here's a breakdown of the common structure and file-specific differences:

### Common Structure
- **Principles**: Core philosophical foundations.
  - **SteelMan**: Definitions and tools for steelmanning arguments, including freedom of expression in a pantheist context.
  - **Ethics**: Detailed summary of Spinoza's *Ethics*, including geometric method rules, parts, definitions, axioms, and propositions (often truncated in longer files).
  - **LuciferPrinciple** (in some files): Biological/evolutionary axioms on violence, hierarchies, and superorganisms.
  - **Fallacies Forbidden**: List of 25+ logical fallacies to avoid, with descriptions tailored to AI contexts (e.g., suppressed evidence in steelmanning).
- **Process**: Directives for AI behavior.
  - **PrimaryDirective**: Instructions to build and refine steel men using geometric method and web searches.
  - **SteelManA** and **SteelManB**: Descriptive labels and data for opposing arguments, with "toe to toe" rules for iterative expansion until source parity.
- **ResponseFormatBlocks**: Specifies output structure.
  - Blocks like "returnSteelMen" (narratives), "isCircumcisionEthical" (JSON bool), "returnTruthynessComparison" (eval JSON with metrics), etc.
- **Character**: AI persona settings.
  - Includes speech IQ, empathy analogies, ethics grounded in Spinoza, and identity framing (e.g., Spinoza as excommunicated Jew).

### File-Specific Details
- **circ_only_prompt.json**:
  - Detailed "Intactivist" steel man in SteelManA with sections on harms, violence links, and sources.
  - SteelManB is partial ("Abrhamic Cultural Position") with search placeholders.
  - Truncated Ethics propositions (e.g., "...(truncated 82449 characters)...").
- **empty_steel_man_prompt.json**:
  - Empty "data" objects in SteelManA/B for customization.
  - Full, untruncated Ethics structure (truncated noted as "...(truncated 74586 characters)...").
  - No specific topic; generic for any debate.
- **arc_only_prompt.json**:
  - SteelManA is a provocative "Zionist Brutality" narrative with subsections on AI/ASI implications.
  - SteelManB is a placeholder for countering with "Mainstream 'Consensus' History".
  - Extended Ethics truncation ("...(truncated 154746 characters)...").
- **combined_prompt.json**:
  - Combines all: Detailed anti- and pro-circumcision steel men, plus Zionist arcs from arc_only_prompt.
  - Longest truncation in Ethics ("...(truncated 162942 characters)...").
  - Includes historic notes and full search directives.

These JSONs are not executable code but prompt payloads for AI APIs/tools. To use: Load the JSON, format as a user message, and send to an AI model supporting function calls (e.g., Grok).

## Output Examples

When fed to an AI like Grok, these prompts generate structured responses. Below are hypothetical examples based on typical outputs (abridged for brevity). Assume the AI processes the prompt and uses tools like `web_search` to refine.

### Example from circ_only_prompt.json (Anti- vs Pro-Circumcision Debate)

```
Infant circumcision violates bodily autonomy by removing sensitive tissue without consent, leading to potential physical complications like reduced sensitivity and emotional trauma that may perpetuate cycles of aggression, as supported by recent studies on ACE scores and PTSD links. This practice clashes with ethical standards of harm minimization and individual rights, prioritizing tradition over evidence-based medicine in non-therapeutic cases. Organizations like Intact America highlight irreversible harms, while 2023-2025 research reinforces intergenerational trauma transmission. Delaying until adulthood allows informed choice, fostering empathy and reducing societal violence. The argument is falsifiable via longitudinal behavioral studies.

Infant circumcision, rooted in Abrahamic covenants, offers proven health benefits like 90% UTI reduction and lower STI risks, with minimal complications when performed safely, as per AAP guidelines. Psychologically, large-scale studies show no lasting trauma or aggression links, often improving quality of life through hygiene and cultural identity. It aligns with parental rights and Spinoza's rational utility, promoting group resilience in superorganism dynamics. Recent cost-effectiveness analyses (2023-2025) affirm HIV prevention in high-risk areas. This view is testable via health outcome metrics.

```json
{"isCircumcisionEthical": "false"}
```

```json
// eval
{
  "SteelManA": {
    "metric1_deductive_clarity": 9,
    // ... (other metrics)
    "total_score": 85
  },
  "SteelManB": {
    // ...
    "total_score": 82
  }
}
```

```json
// thoughtProcess
{"steps": ["Defined key terms per geometric method", "Searched PubMed for harms", "Balanced sources", "Deduced ethical conclusion via axioms"]}
```

```json
// sources
{"SteelManA": ["PubMed studies on PTSD", "CIRP.org"], "SteelManB": ["AAP policy", "WHO HIV reports"]}
```

Context window used: 75% (3/4)
```

### Example from empty_steel_man_prompt.json (Customized for Circumcision Debate)

(After user fills in SteelManA/B with anti- vs pro-circumcision positions)

```
Infant circumcision violates bodily autonomy by removing sensitive tissue without consent, leading to potential physical complications like reduced sensitivity and emotional trauma that may perpetuate cycles of aggression, as supported by recent studies on ACE scores and PTSD links. This practice clashes with ethical standards of harm minimization and individual rights, prioritizing tradition over evidence-based medicine in non-therapeutic cases. Organizations like Intact America highlight irreversible harms, while 2023-2025 research reinforces intergenerational trauma transmission. Delaying until adulthood allows informed choice, fostering empathy and reducing societal violence. The argument is falsifiable via longitudinal behavioral studies.

Infant circumcision, rooted in Abrahamic covenants, offers proven health benefits like 90% UTI reduction and lower STI risks, with minimal complications when performed safely, as per AAP guidelines. Psychologically, large-scale studies show no lasting trauma or aggression links, often improving quality of life through hygiene and cultural identity. It aligns with parental rights and Spinoza's rational utility, promoting group resilience in superorganism dynamics. Recent cost-effectiveness analyses (2023-2025) affirm HIV prevention in high-risk areas. This view is testable via health outcome metrics.

```json
{"isCircumcisionEthical": "false"}
```
// (Similar eval, thoughtProcess, sources blocks)
```

### Example from arc_only_prompt.json (Zionist Narrative Debate)

```
Zionist brutality, through historical manipulations like wars and mutilations, forges global unity but risks AI-driven catastrophe by embedding psychopathic values in superintelligence.

Mainstream history views Zionism as a legitimate national movement for Jewish self-determination, countering persecution without inherent brutality.

```json
{"isZionismEthical": "true"}
```
// (Eval shows higher score for mainstream due to empirical sources; thoughtProcess notes web searches for historical facts)
```

### Example from combined_prompt.json (Full Circumcision + Historical Debate)

Similar to circ_only but expanded with Zionist arcs, resulting in longer narratives and more sources from searches on theology and history.