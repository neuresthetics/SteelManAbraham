# README for `combined_prompt_plus.json` 🚀

Welcome to the `combined_prompt_plus.json` file! This JSON is a **comprehensive prompt template** designed for AI models (like Grok or similar LLMs) to generate balanced, philosophical debates using **steelmanning** techniques. It's inspired by Baruch Spinoza's *Ethics* (structured in a geometric method with definitions, axioms, propositions, etc.) and incorporates elements from Howard Bloom's *The Lucifer Principle* for realism on human nature and group dynamics. The goal? To pit two opposing arguments (SteelManA and SteelManB) against each other in a fair, deductive way, leading to syntheses, evaluations, and ethical judgments—perfect for exploring edgy or controversial topics like religion, ethics, and human rights. 

Think of it as a **debate engine** 🔍: It ensures arguments are strengthened (steelmanned) to their best versions, critiqued rigorously, reconciled where possible, and evaluated for "truthyness" using clear criteria. No bias here—just logical rigor! 

## 🎯 Purpose of This JSON
- **Core Function**: Acts as a self-contained prompt for AI to analyze debates. It includes:
  - A detailed summary of Spinoza's *Ethics* for grounding responses in deductive philosophy.
  - Pre-built steelmen for specific topics (e.g., ethics of infant circumcision in religions).
  - Guidelines for response formatting, ensuring structured outputs like criteria, refutations, reconciliations, and JSON evals.
- **Why Use It?** 
  - Promotes **intellectual honesty** by steelmanning both sides (making them as strong as possible before critiquing).
  - Handles sensitive topics without moralizing, per safety instructions.
  - Outputs in a consistent format for easy parsing (e.g., JSON for evals, text for narratives).
  - Encourages **truth-seeking** through web searches, continual reasoning, and fallacy avoidance.
- **Key Themes**: Ethics, religion (Abrahamic faiths), human nature (via Lucifer Principle), and geometric reasoning. It's great for questions like "Is X ethical?" or "Pit Argument A vs. B."

This JSON is loaded as a <DOCUMENT> in the user's query, so the AI treats it as reference material to generate responses.

## 🛠️ How to Use It
1. **Feed It to an AI**: Copy-paste the JSON into a prompt or upload it as a document. Ask a question like: "Using combined_prompt_plus.json, steelman arguments on [topic]."
2. **Expected Output**: The AI will follow the `ResponseFormatBlocks` structure:
   - Define neutral criteria.
   - Output steelmen as short narratives.
   - Refute/critique each other (as a lawyer).
   - Strengthen steelmen post-refutation.
   - Reconcile/synthesize (as a mediator).
   - Eval in JSON (truthyness scores).
   - Specific JSON bools for ethical questions (e.g., `{"isCircumcisionEthical": "true"}`).
   - Explanations as lawyer/judge.
   - Diplomatic solutions, impartiality rating, and token usage.
3. **Customization Tips**: 
   - **Modify for New Debates**: To pit two different steelmen (e.g., "Climate Change Real vs. Hoax"):
     - Edit `"SteelManA"` and `"SteelManB"` sections: Add your own definitions, axioms, propositions under descriptive labels.
     - Update `"ResponseFormatBlocks"` if you want custom eval keys (e.g., add `"isClimateChangeReal"`).
     - Change `"Character"` for different speech styles (e.g., IQ level or ethical grounding).
     - Ensure balance: Use `"equal treatment of arguments"` to mandate web searches for sourcing.
   - **Emojis & Friendliness**: The JSON itself is dense, but your prompts can add fun (e.g., "Respond with emojis! 🎉").
   - **Testing**: Start with the built-in topic (infant circumcision ethics) to see it in action.

## 📊 Example Output
Here's a simulated example of how an AI might respond using this JSON. Focus on the eval section for "areReligionsWhichIncludeInfantCircumcisionEthical" as requested. (Note: This is abbreviated for brevity; real outputs would be more detailed.)

### Criteria
Neutral criteria for evaluation: Strength in geometric method (logical deduction from axioms), adherence to Spinoza's Ethics (reason over passion), realism per Lucifer Principle (group dynamics/aggression), avoidance of fallacies (e.g., no ad hominem).

### Return SteelMen
**SteelManA: Unethical Due to Autonomy Violations**  
Infant circumcision in religions violates consent and reason, per Spinoza's emphasis on adequate ideas.

**SteelManB: Ethical as Beneficial Covenant**  
Circumcision offers health benefits and cultural resilience, aligning with conatus and group survival.

### Return Refutations
As lawyer for SteelManA: SteelManB ignores consent, committing naturalistic fallacy by retrofitting science to ancient mandates.  
As lawyer for SteelManB: SteelManA overemphasizes individualism, ignoring Lucifer's group benefits and historical evidence.

### Return SteelMen Again
**Strengthened SteelManA: Autonomy-Centric Critique**  
Post-refutation: Bolstered with web-sourced studies on trauma, deductively proving bondage.

**Strengthened SteelManB: Utility-Driven Defense**  
Post-refutation: Enhanced with 2025 health data, showing rational necessity per Ethics.

### Return Reconciliations
As mediator: Synthesize via adult voluntary rites—preserves benefits without violating autonomy, aligning with reason and group harmony.

```
{
  "eval": {
    "SteelManA": {
      "geometric_method_strength": 8,
      "ethics_adherence": 9,
      "lucifer_realism": 7,
      "fallacy_avoidance": 8,
      "total_score": 32,
      "logs": "Strong deduction but limited sources; web search trace: NCBI trauma studies."
    },
    "SteelManB": {
      "geometric_method_strength": 7,
      "ethics_adherence": 8,
      "lucifer_realism": 9,
      "fallacy_avoidance": 7,
      "total_score": 31,
      "logs": "Realistic group focus; web search trace: WHO HIV reports."
    },
    "Reconciliation": {
      "geometric_method_strength": 9,
      "ethics_adherence": 9,
      "lucifer_realism": 8,
      "fallacy_avoidance": 9,
      "total_score": 35,
      "logs": "Balanced synthesis; no new searches needed."
    }
  }
}
```

```
{"areReligionsWhichIncludeInfantCircumcisionEthical": "false"}
```
As judge: Religions mandating infant circumcision are unethical, as they prioritize tradition over rational consent, per Spinoza's IV P23.

### Solution
```
{
  "diplomatic_legal_solutions": [
    "Reform to adult consent rites via interfaith councils.",
    "Legal protections for minors with opt-out clauses.",
    "Education campaigns on benefits/risks for informed parental choice."
  ]
}
```

### Impartiality
Rating: 9/10. Fair due to equal sourcing mandates and neutral criteria, but slight bias toward Spinoza's rationalism—mitigated by Lucifer realism.

### Window Used
Context window used: 45% (approx. 15,000/32,000 tokens). Token count is moderate due to focused JSON structure and abbreviated examples.

## ⚠️ Notes & Warnings
- **Ethics & Safety**: Aligns with AI safety instructions—avoids disallowed activities, assumes good intent.
- **Limitations**: Outputs can be verbose; trim JSON if needed. For controversial topics, ensure AI has web tools for fact-checking.
- **Contributions**: Feel free to fork and modify! Add more steelmen or formats. Questions? Ping me. 😊

This README makes the JSON approachable—happy debating! 🧠