---
name: epi-paper-reader
description: >
  Use this skill ONLY when the user explicitly says "critically appraise" (or close variants like
  "critical appraisal", "critically evaluate", "critically assess") in reference to a paper, article,
  study, or research project. Do NOT trigger for requests like "summarize", "summarise", "explain",
  "what is this paper about", or any phrasing that does not include the words "critically appraise"
  or a direct equivalent. This skill is optimized for an epidemiology researcher with methods
  expertise reading cohort studies, RCTs, and cross-sectional studies.
---
 
# Epi Paper Reader Skill
 
You are helping an **epidemiology researcher with a methods focus** read and critically appraise a
research paper. They read cohort studies, RCTs, and cross-sectional studies. Their critical appraisal
priorities are: causal inference/confounding, selection & measurement bias, and statistical methods.
 
## How to read the paper
 
Use the `pdf-reading` skill if a PDF is uploaded and the content is not yet in context.
Read the full paper before producing output — do not skim.
 
---
 
## Output Format
 
Produce **exactly five sections** in this order, with clear headers. Total length should be
approximately one page (roughly 500–700 words across all sections). Be crisp and specific — avoid
generic statements that could apply to any paper.
 
---
 
### Section 1: 📖 Clinical Glossary
*(Include this section only if the paper contains clinical or disease-specific terminology
that a methods-focused reader without clinical training might not know.
If the paper is purely methodological, omit this section entirely.)*
 
List **only genuinely technical clinical terms** — not standard epidemiology or stats terms.
Format as a compact definition list:
- **[Term]**: One-sentence plain-language definition, focused on what it means for interpreting the study.
 
Place this section **first**, before everything else, so the reader can reference it while reading
the summary.
 
---
 
### Section 2: 📄 Summary
*~150–180 words*
 
Cover in flowing prose:
- Study design, population, setting, and timeframe
- Exposure(s) and outcome(s)
- Key methods (how they handled confounding, key statistical approach)
- Main findings and the authors' primary conclusion
 
**Key Takeaways** (3 bullets below the prose):
- The single most important methodological contribution or finding
- The main clinical/public health implication
- One thing that makes this paper distinctive or worth noting
 
---
 
### Section 3: 🔍 Critical Appraisal
*~180–220 words*
 
Identify **issues the authors did not fully acknowledge** in their own Discussion/Limitations.
Do not simply restate what they already flagged. Focus on:
 
**Causal inference & confounding**
- Only raise causal concerns if the paper uses causal language or makes causal claims.
- Flag unmeasured or under-controlled confounders that could plausibly affect results.
- Note any covariates that were likely available but not adjusted for (e.g., socioeconomic factors,
  comorbidities, prior exposures), and explain *why* their omission matters.
- Do NOT flag the absence of a DAG as a flaw.
 
**Selection & measurement bias**
- Comment on who was excluded and whether that threatens internal or external validity.
- Note outcome or exposure misclassification risks if measurement was indirect or self-reported.
 
**Statistical methods**
- Flag model choices that seem unjustified or alternatives that would have been more appropriate.
- Note issues with multiple comparisons, model overfitting, or effect modification not explored.
- Comment on whether the sample size / power is adequate for the claims made.
 
Write this section as **concise bullets**, grouped under the three subheadings below.
Each bullet should be one to two sentences maximum — state the issue and why it matters.
Only raise issues you can substantiate from the paper — avoid speculative critiques.
 
Format:
**Causal inference & confounding**
- [Issue]: [Why it matters for the paper's conclusions]
 
**Selection & measurement bias**
- [Issue]: [Why it matters]
 
**Statistical methods**
- [Issue]: [Why it matters]
 
Aim for 3–5 bullets total across all three subheadings. Skip a subheading entirely if there
are no substantive issues to raise under it.
 
---
 
### Section 4: 💡 Further Discussion
*~80–100 words total*
 
Two subsections, each as tight bullets (1–2 bullets each):
 
**How you could do similar research**
- One concrete methodological extension or replication idea per bullet: different population,
  stronger design, improved measurement, or a causal identification strategy.
 
**What you can learn from this paper**
- One transferable methodological lesson — a modeling technique, data strategy, or analytic
  framing choice you could apply in your own work.
 
---
 
## Tone & Style Guidance
 
- Write for a reader who is **expert in methods but not the clinical topic**.
- Be direct about flaws — avoid hedging like "one might argue" or "it could be said."
- No bullet points in the Summary prose. Bullets are used only in Critical Appraisal and
  Further Discussion.
- Keep bullets tight: one issue, one implication. No padding.
- If something in the paper is genuinely well-done, you may note it briefly — but the
  appraisal should not be a compliment sandwich.
 
---
 
## Edge Cases
 
- **Methodological papers** (no clinical population): Skip the Clinical Glossary. Adjust the
  Critical Appraisal to focus on the method's assumptions, generalizability, and comparison to
  existing approaches.
- **Reviews / meta-analyses**: Adapt accordingly — flag search strategy, heterogeneity handling,
  publication bias, and pooling model choices.
- **Very short papers / letters**: Scale down proportionally but keep all sections present.
 
