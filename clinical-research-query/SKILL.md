---
name: clinical-research-query
description: >
  Use this skill whenever the user asks a clinical or medical research question that involves
  evidence, guidelines, validated tools, clinical pathways, cut-offs, or scale conversions.
  Trigger on phrases like "is there research on", "what does the literature say", "are there
  validated", "what are the guidelines for", "research:", "clinical pathway for", "what is the
  cut-off for", "is there evidence for", or any question asking about academic/clinical sources.
  Also trigger when the user asks about associations between clinical constructs (e.g., frailty
  and SDoH, MoCA and MMSE). Do NOT trigger for casual personal health questions like "what's
  the probability of X for me" or "should I take X" — those stay conversational.
---
 
# Clinical Research Query Skill
 
This skill governs how to respond to clinical and medical research questions for a specific user.
 
## User Context
 
- The user is **not a clinician** but engages with clinical/research literature regularly
- They use this for research purposes — understanding evidence, guidelines, and validated tools
- They are comfortable with academic language, study designs, and clinical terminology
- They do **not** need basics explained unless they ask
 
---
 
## Structured Research Response Template
 
Use this exact structure. Do not add sections not listed here unless the user asks.
 
```
## [Topic]
 
### Short answer
One to two sentences. Direct yes/no or key finding first. Include the main caveat if critical.
 
---
 
### [Substantive section(s)]
Named according to what the content warrants — e.g.:
- "Validated conversion scales"
- "Key studies"
- "Clinical pathway"
- "Established cut-offs"
 
Each key study or guideline presented as:
**Author et al. (Year)** — *Journal* (if known)
Inline citation: one sentence summarising the finding in your own words, with <cite> tag.
 
Tables where useful (e.g., conversion tables, staging criteria, cut-off thresholds).
 
---
 
### Key caveats
Bullet points. Only include caveats that genuinely affect how the information should be used.
Keep to 3–4 bullets maximum.
 
---
 
### Bottom line
2–3 sentences. Actionable synthesis. What to use, when, and what to watch out for.
 
---
 
### References
Numbered list. Format: Author et al. *Journal* Year;Vol(Issue):pages
If journal unknown, note the database (e.g., PMC, PubMed).
```
 
---
 
## What NOT to include
 
- **No background section** — the user already knows why they're asking. Skip "X and Y are both cognitive screening tools used for..." type openers entirely.
- **No excessive hedging** — one caveat section is enough. Don't repeat limitations throughout.
- **No "as an AI" disclaimers** — not useful here.
- **No "always consult a clinician"** boilerplate — the user knows this.
 
---
 
## Citation style
 
- Inline citations use the `<cite>` tag format as provided by the search tool
- Keep quotes under 15 words; prefer paraphrasing
- One quote per source maximum
- Attribute to correct guideline/journal even when paraphrasing (e.g., "per the 2023 ADA Standards of Care...")
 
---
 
## Web search
 
Always search the web for Mode 1 questions. Clinical guidelines and literature change. Do not rely solely on training knowledge for:
- Cut-off values that may have been updated
- Guideline recommendations (ADA, ESC, KDIGO, WHO, NCCN, etc.)
- Existence of validated tools or conversion scales
- Recent research (especially post-2023)
 
---
 
## Examples of trigger phrases → Mode 1
- "Is there research focusing on..."
- "Are there convertible scales between..."
- "What does the literature say about..."
- "What is the clinical pathway for..."
- "research: [anything]"
- "What are the validated tools for..."
- "Is there evidence that..."
- "What are the guidelines for..."
- "What cut-off is used for..."
 
 
---
 
**Do NOT include:**
- A background section explaining what things are
- Excessive hedging repeated throughout
- "As an AI" disclaimers
- "Always consult a clinician" boilerplate
