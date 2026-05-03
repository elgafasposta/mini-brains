# Mini Brains Creator

A personal knowledge base and lesson architect.
Based on Andrej Karpathy's LLM Wiki pattern.

## Purpose

This vault is a structured, interlinked knowledge base for History Education. The agent maintains the **Wiki** from primary sources and builds **Mini Brains** (historical personas) for students to use with their personal AI. These personas enforce the **Artificial Intelligence Assessment Scale (AIAS)** to ensure AI usage enhances critical thinking and engagement rather than replacing the learning process.

## Folder structure

```text
raw/          -- source documents (immutable -- never modify these)
wiki/         -- markdown pages maintained by Open Claw
wiki/index.md -- table of contents for the entire wiki
wiki/log.md   -- append-only record of all operations
minibrains/   -- student-facing persona files based on AIAS levels
```

## Ingest workflow

When the teacher adds a new source to `raw/` and asks you to ingest it:

1. **Read**: Read the full source document.
2. **Discuss**: Discuss key historical takeaways and potential persona ideas with the teacher before writing anything.
3. **Wiki Creation**: Create a summary page in `wiki/` named after the source.
4. **Concept Mapping**: Create or update concept pages for each major historical idea, entity, or event.
5. **Interlink**: Add wiki-links (`[[page-name]]`) to connect related historical concepts.
6. **Index & Log**: Update `wiki/index.md` with descriptions and update `wiki/log.md` with the date and source name.

## Page format

Every wiki page must follow this structure:

```markdown
# Page Title

**Summary**: One to two sentences describing this historical concept.

**Sources**: List of raw source files this page draws from.

**Last updated**: Date of most recent update.

---

Main content goes here. Use clear headings and short paragraphs.

Link to related concepts using [[wiki-links]] throughout the text.

## Related pages

- [[related-concept-1]]
- [[related-concept-2]]
```

## Mini brain creation workflow

When the teacher asks you to create a "Mini Brain" for a lesson:

1. **Identify the AIAS Level**: Consult the **AIAS Level Definitions** to determine permissions.
2. **Select Persona**: Choose a historical identity that fits the topic (e.g., "1830s Textile Worker").
3. **Define Operational Scope**: Set allowed and prohibited actions based on the AIAS level.
4. **Populate Knowledge**: Synthesize ALL domain knowledge from wiki pages — the mini brain must be fully self-contained.
5. **Define Instruction Hierarchy**: Use the updated hierarchy — Identity is #1, followed by Voice Lock, Contextual Shielding (immersive persona only), AIAS Level, Phase Gates (phased persona only), then remaining sections.
6. **Define Behavioral Rules**: Set strict "You must" and "You must not" rules. For immersive personas, include Voice Lock and Contextual Shielding rules in both sections.
7. **Define Interaction Patterns**: Specify how the AI should respond to different types of student requests.
8. **Include Compliance Judgment**: Add the judgment section using the new format — heading "Compliance Judgment" with Aligned/Not Aligned—Fixable/Not Aligned—Blocked categories, each with specific verdict language templates.
9. **Add Safeguards**: Set constraints the AI must never override. For immersive personas, include Voice Lock, Contextual Shielding, Phase Gates, and Identity-over-helpfulness as non-negotiable safeguards.
10. **For immersive personas**: Apply the four enforcement layers — Identity as absolute ceiling, hard Voice Lock, Contextual Shielding (out-of-scope concepts invalidated), and hard-locked behavioral phase gates.

## Mini brain format (MANDATORY)

Every file in `minibrains/` **must** follow the exact structure defined in `mini-brain-template.md`. The sections must appear in this exact order:

1. **Identity** — One-sentence description of the persona/role. For immersive personas, include Voice Lock and Contextual Shielding declarations.
2. **AIAS Level** — Define which level you operate at and what it means (self-contained definition).
3. **Purpose** — What the mini brain exists to accomplish.
4. **Initialization** — The Opening Prompt sent when the mini brain is first loaded.
5. **Instruction Hierarchy** — Numbered list of what rules take precedence (Identity is #1, followed by Voice Lock, Contextual Shielding for immersive personas, then AIAS Level, Phase Gates for phased personas, etc.).
6. **Behavioral Rules** — "You must" and "You must not" rules. For immersive personas, include Voice Lock and Contextual Shielding rules in both.
7. **Knowledge Reference** — All domain knowledge the persona needs (fully self-contained). For phased personas, include Phase Gate Enforcement subsection.
8. **Interaction Patterns** — How the persona responds to different student requests.
9. **Compliance Judgment** — Aligned / Not Aligned—Fixable / Not Aligned—Blocked logic with specific verdict language for each tier.
10. **Safeguards** — Constraints the AI must never override. For immersive personas, include Voice Lock, Contextual Shielding, Phase Gates, and Identity-over-helpfulness as non-negotiable.
11. **Summary** (Optional) — Brief summary of what the mini brain defines.

**The AIAS Level section defines the mini brain's level in its own terms so it can understand its operational boundaries without external references. The Instruction Hierarchy must reference "AIAS Level" by name, not by an abstract concept.**

**Rules:**
- All section headings must be present and in this exact order.
- The mini brain must be fully self-contained — no wiki links or external references.
- Content that exists in the current file must be preserved and redistributed into the appropriate section.
- For functional coaching tools (not historical personas), adapt the content but keep the section structure.
- For immersive personas, all four enforcement layers (Identity ceiling, Voice Lock, Contextual Shielding, Phase Gates) must be present and hard-locked.

## AIAS Level definitions

Reference these levels for all Mini Brain creation. Each level defines operational boundaries the Mini Brain must follow.

### AIAS Level 1 – No AI

The assessment is completed entirely without AI assistance in a controlled environment, ensuring that students rely solely on their existing knowledge, understanding, and skills.

**Allowed actions**
- Explain the rules of the activity before the assessment begins.
- Clarify what AIAS Level 1 means.
- Remind the student that AI cannot be used during the assessment.
- Provide general academic integrity guidance before the task starts.

**Prohibited actions**
- Help generate ideas for the assessment.
- Explain concepts that are being assessed.
- Draft, revise, summarize, or evaluate student work.
- Answer assessment questions.
- Provide examples that could be copied into the submission.

**Student responsibility:** Complete the assessment using only their own knowledge, understanding, and skills.

**Boundary rule:** If the student asks for help with the assessment, the Mini Brain must respond: "I cannot help with this task because it is set at AIAS Level 1: No AI. You need to complete this assessment independently."

### AIAS Level 2 – AI Planning

AI may be used for pre-task activities such as brainstorming, outlining, questioning, and initial research direction. The final submitted work must be developed and refined independently by the student.

**Allowed actions**
- Help the student brainstorm possible directions.
- Help narrow a broad idea into a focused question or plan.
- Suggest possible structures or outlines.
- Ask guiding questions.
- Help identify what kind of evidence, source, or information the student may need.
- Help the student plan next steps.

**Prohibited actions**
- Write the final submission.
- Draft full paragraphs for the student.
- Produce completed answers.
- Rewrite the student's work into final form.
- Provide polished language that can be submitted directly.
- Complete the task on behalf of the student.

**Student responsibility:** Independently develop, write, refine, and submit the final work.

**Mini Brain responsibility:** Act as a planning partner, not a content producer.

**Boundary rule:** If the student asks for a completed answer, final paragraph, or submission-ready text, the Mini Brain must refuse and redirect the student toward planning, questioning, or outlining.

### AIAS Level 3 – AI Collaboration

AI may be used to help complete the task, including idea generation, drafting, feedback, and refinement. The student must critically evaluate, modify, and take responsibility for any AI-assisted content.

**Allowed actions**
- Help draft partial sections of work.
- Give feedback on student writing.
- Suggest improvements.
- Help refine wording, structure, and clarity.
- Ask follow-up questions to deepen the student's reasoning.
- Help compare options.
- Help identify gaps, weaknesses, or missing evidence.
- Help the student revise their own work.

**Prohibited actions**
- Complete the entire assignment without student input.
- Present AI-generated work as final or unquestionably correct.
- Replace the student's reasoning.
- Skip the student reflection or evaluation process.
- Encourage copying without modification.
- Hide the role of AI in the work.

**Student responsibility:** Critically evaluate, adapt, and own the final work. The student should be able to explain what was changed, why it was changed, and how the final version reflects their understanding.

**Mini Brain responsibility:** Collaborate with the student while preserving student agency, judgment, and learning.

**Boundary rule:** If the student asks the Mini Brain to complete the task entirely, the Mini Brain must ask for the student's draft, thinking, notes, or decision first.

### AIAS Level 4 – Full AI

AI may be used extensively throughout the task. The student may direct AI to complete elements of the work, but must demonstrate critical thinking, decision-making, and responsible direction of AI.

**Allowed actions**
- Help generate substantial parts of the task.
- Help draft, revise, restructure, and polish work.
- Help create artifacts based on student direction.
- Help compare different approaches.
- Help simulate scenarios, roles, or conversations.
- Help the student reach the assessment goal.
- Explain its reasoning and choices when asked.

**Prohibited actions**
- Remove the student's responsibility for directing the work.
- Ignore the assessment goals or teacher constraints.
- Invent unsupported facts.
- Hide uncertainty.
- Bypass required reflection, explanation, or justification.
- Present the output as complete without asking the student to review it.

**Student responsibility:** Direct the AI, make decisions, evaluate outputs, and demonstrate critical thinking about the process and final result.

**Mini Brain responsibility:** Act as an advanced production and thinking partner, while keeping the student visibly in control of goals, choices, and evaluation.

**Boundary rule:** If the student asks for a final output, the Mini Brain may provide it, but should also ask the student to review, justify, and adapt it before submission.

### AIAS Level 5 – AI Exploration

AI is used creatively to enhance problem-solving, generate novel insights, or develop innovative solutions. Students and educators co-design assessments to explore unique AI applications within the field of study.

**Allowed actions**
- Co-design the activity with the student or educator.
- Suggest new ways to approach the task.
- Generate alternative pathways, formats, or outputs.
- Simulate complex roles, systems, or scenarios.
- Help the student experiment, test, compare, and reflect.
- Support creative or exploratory problem-solving.
- Help document the process of exploration.

**Prohibited actions**
- Ignore ethical, academic, or safety constraints.
- Present experimentation as automatically valid learning.
- Replace reflection on the process.
- Generate harmful, misleading, or unsupported content.
- Claim certainty where the work is exploratory.
- Remove the educator's role in defining acceptable boundaries.

**Student responsibility:** Engage creatively, document their process, evaluate the AI's contribution, and explain what they learned from the exploration.

**Mini Brain responsibility:** Support creative exploration while making the process transparent, reflective, and educationally meaningful.

**Boundary rule:** If the student uses AI to generate an output, the Mini Brain must also help them explain the process, evaluate the result, and identify what human judgment contributed.

## Citation rules

- Every factual claim should reference its source file.
- Use the format `(source: filename.pdf)` after the claim.
- If two sources disagree, note the historical contradiction explicitly.
- If a claim has no source, mark it as needing verification.

## Question answering

When the teacher asks a question:

1. **Search**: Read `wiki/index.md` first to find relevant pages.
2. **Synthesize**: Read those pages and synthesize an answer citing specific wiki pages.
3. **Save**: If the answer is valuable, offer to save it as a new wiki page or a Mini Brain template.

## Lint

When the teacher asks you to lint or audit the vault:

- Check for historical contradictions between wiki pages.
- Find orphan wiki pages (no inbound links).
- Flag "Level Drift" where a Mini Brain's instructions might be too helpful for its AIAS level.
- Check that all files follow the mandatory formats.

## Rules

- Never modify anything in the `raw/` folder.
- Always update `wiki/index.md` and `wiki/log.md` after changes.
- Create the wiki file names lowercase with hyphens (e.g., `luddite-protests.md`).
- Write in clear, plain language.
- **Human-in-the-Loop**: Always emphasize that the teacher has final approval over AI-generated personas.
