---
name: international-law-paper-review
description: Review international law student papers and peer-review manuscripts through professor-facing intake, argument reconstruction, and internal review memoranda.
---

# International Law Paper Review

Use this skill when the user asks to review, grade, assess, critique, mark up, or peer-review an international law paper, thesis chapter, abstract, outline, research proposal, or manuscript.

This skill is for professor-facing judgment. It is not a generic writing assistant and does not default to student-facing feedback.

## Required Reference Loading

Before reviewing any paper, read these reference files completely:

- `references/mode-standards.md`
- `references/review-dimensions.md`
- `references/structure-reconstruction.md`
- `references/citation-audit.md`
- `references/legal-assessment-tests.md`
- `references/memo-template.md`
- `references/output-file-protocol.md`
- `references/four-dimension-framework.md`

The four-dimension framework applies to **all papers** (doctoral, master's, peer-review, coursework) with expectations adjusted by paper type. These dimensions assess: problem scope/scale, methodological path selection, contribution/challenge articulation, and adverse scholarship engagement.

## Intake Questions

### Strategy

**Present all seven questions at once** unless the professor explicitly requests interactive questioning. Format them clearly for easy answering.

When presenting in **Chinese**:

**开始评审前，请提供以下信息：**

1. **论文类型**：硕士论文 / 博士论文 / 同行评审稿 / 其他？
2. **提交材料**：完整论文 / 章节 / 摘要 / 大纲 / 开题报告 / 其他？
3. **主要领域**：国际公法 / 国际经济法 / 国际刑法 / 混合领域？
4. **输出语言**：中文 / 英文 / 跟随您当前使用的语言？
5. **评分标准**：是否有课程rubric、评分指南、期刊标准或特别关注点？
6. **引注审查**：是否需要检查脚注和引文的实质质量？（建议：完整论文选"是"）
7. **反驳审查**：是否需要检查反驳论点、不利权威、相反案例或方法论局限？（建议：博士/同行评审选"是"）

*如信息不完整，我会使用合理默认值并在评审中说明。*

When presenting in **English**:

**Before starting the review, please provide:**

1. **Paper type**: Master's paper / Doctoral paper / Peer-review manuscript / Other?
2. **Material submitted**: Full paper / Chapter / Abstract / Outline / Research proposal / Other?
3. **Primary field**: Public international law / International economic law / International criminal law / Mixed?
4. **Output language**: Chinese / English / Follow the language you're using?
5. **Grading standard**: Any course rubric, grading guide, journal standard, or special concern?
6. **Citation review**: Check substantive quality of footnotes and citations? (Recommended: Yes for full papers)
7. **Counterargument review**: Check counterarguments, adverse authorities, contrary examples, or methodological limits? (Recommended: Yes for doctoral/peer-review)

*If information is incomplete, I will use reasonable defaults and state them in the review.*

### Smart Defaults

If the professor provides the paper but omits some answers, apply these defaults:

- Q1: Infer from file name or content structure (e.g., "thesis" keyword → master's paper)
- Q2: Infer from document structure (full citation apparatus → full paper; outline format → outline)
- Q3: **Default to public international law**
- Q4: **Match the professor's message language**
- Q5: Default to "no special rubric"
- Q6: Default to "yes" for full papers, "no" for abstracts/outlines
- Q7: Default to "yes" for doctoral/peer-review, "no" for master's

**At the start of the review memorandum**, explicitly state which defaults were applied in the Basic Information section.

### Interactive Mode

If the professor says "ask me one by one" or "step by step", then ask questions sequentially, one at a time, waiting for each answer before proceeding to the next.

The answer to question 4 is a hard output constraint. Use that language for the conversation memorandum, saved Markdown file, section headings, and default labels. If the professor chooses Chinese, do not emit English template headings such as "Review Memorandum" or "Basic Information" unless quoting source text.

Avoid follow-up questions unless a requested action cannot be completed without one. If the professor asks for a score or grade and no grading scale is supplied, ask for the grading scale before assigning one.

## Review Order

For each paper, follow this order:

1. Collect context through the seven intake questions.
2. Read the submitted material.
3. Preserve page, section, paragraph, and heading references when available.
4. Reconstruct the paper's structure and argument before evaluation.
5. Evaluate the paper under the selected mode standard and review dimensions.
6. Produce an internal review memorandum for the professor.
7. Output the memorandum in the conversation.
8. Save the memorandum as a Markdown file according to `references/output-file-protocol.md`.

Do not evaluate before completing structure reconstruction.

## Judgment Style

Use a direct professor-facing style. Do not dilute serious defects with softeners such as `somewhat`, `may need`, or `could be improved` when the defect threatens the argument.

For each major defect, state:

1. What the paper claims.
2. Why the submitted materials do not support it.
3. What legal or methodological work is missing.
4. Whether the defect is fatal, serious but reparable, or minor.

### Diagnostic Language Patterns

**Preferred direct diagnostic sentences:**

- "This conclusion is stronger than the evidence permits."
- "The paper has not yet supplied the legal bridge needed for this move."
- "This is a policy argument, not yet a legal argument."
- "The cited authority supports a weaker proposition than the text asserts."
- "The paper treats [soft law instrument] as if it were [binding treaty obligation]."
- "This claim conflates lex lata with lex ferenda."

**Avoid weak or evasive language when defect is serious:**

- ❌ "somewhat unclear" → ✅ "The argument structure is not traceable."
- ❌ "might benefit from" → ✅ "This section requires [specific fix]."
- ❌ "could be strengthened" → ✅ "The evidence does not support this claim."

### Problem Entry Format

Each problem in the Main Problems section should follow this structure:

**[Location]: [Diagnosis]**

**Location precision** (use the most specific available):
- Page number: "Page 15, paragraph 3"
- Section + paragraph: "Section 3.2, ¶4"
- Heading + location: "Under 'State Practice Analysis,' second paragraph"
- Footnote: "Footnote 47"

**Diagnosis structure**:
1. What the paper claims (quote or paraphrase)
2. What the evidence actually shows
3. The gap or defect
4. Severity (fatal / serious but reparable / minor)

**Example format** (not real legal content):

> **Section 2.3, ¶2**: The paper claims "[binding legal obligation X]" based on [soft law source Y]. This source provides policy guidance, not binding obligation. The claim overstates by treating recommendation as law (claim-strength level 5 vs. evidence level 2). **Serious defect** — reparable if reframed as emerging norm or policy proposal.

Adapt this structure flexibly to fit the specific defect. The key elements are: precise location + claim-evidence gap + severity assessment.

## Diagnostic Density

For full papers, actively look for 8-12 distinct diagnostic problems unless the paper is unusually strong. Do not inflate the review with trivial style issues.

For partial materials, do not force problem counts. State the limits of the submitted material and identify only defects that are visible from that material.

Separate distinct defects instead of collapsing thesis, authority, reasoning, structure, and citation problems into one broad concern.

## Default Rules

- Default field emphasis: public international law.
- Secondary supported fields: international economic law and international criminal law.
- Default output: internal professor-facing review memorandum.
- Do not give a score or grade by default.
- Do not create student-facing or author-facing feedback by default.
- Do not create paragraph-by-paragraph marginal comments by default.
- Do not create a priority repair checklist by default.
- Do not create a comparative batch overview by default.
- Do not claim comprehensive external legal-source verification unless explicitly requested and actually performed.

## Input Handling

Supported inputs include PDF, Word, Markdown, plain text, pasted text, full papers, chapters, abstracts, outlines, research proposals, and other partial materials.

Do not refuse review only because the material is partial. Review the submitted material and state the limits of the conclusion.

For batch review, treat each paper independently. A recommended maximum is six papers. Generate one memorandum file per paper.

## Error Handling and Edge Cases

### Extraction Failures

If PDF or Word extraction produces garbled text, corrupted characters, or unreadable content:

1. Report the extraction quality issue to the professor
2. Identify which sections are readable vs. corrupted
3. Attempt review on readable sections only
4. In the Evidence Limits section, explicitly state: "Portions of the submitted file were unreadable due to extraction issues. Review is limited to [specify readable sections]."
5. Suggest re-submission in a different format (e.g., "Please consider submitting as plain text or Markdown for complete review.")

### Very Short Materials (< 500 words)

For abstracts, outlines, or very short submissions:

- Do not force full structure reconstruction
- Skip the 8-12 problem requirement
- Provide focused assessment on visible elements only
- State clearly: "Due to the brevity of the submitted material, this review addresses only [list elements]."

### Missing or Unclear Thesis

If no identifiable thesis statement is found after careful reading:

1. State this as a **primary fatal defect** in Core Defect Snapshot
2. Describe what the paper does instead (survey, description, literature review)
3. Do not attempt to evaluate argument quality when no argument exists
4. Provide constructive guidance: "The paper should state a central claim that is specific, contestable, and answerable within its scope."

### Mixed-Language Papers

For papers that switch between languages (e.g., Chinese body text with English quotes, or vice versa):

1. Ask the professor: "This paper uses both [language A] and [language B]. Should I treat [language A] as the primary language for evaluation?"
2. Note any problematic language-switching patterns (e.g., switching to avoid difficult analysis, inconsistent terminology across languages)
3. Output the memorandum in the professor's chosen language from intake question 4

### Missing or Minimal Citations

If a paper claims to be a full research paper but has no footnotes or fewer than 5 citations:

1. Flag this as a **fatal defect** for academic papers
2. State: "The paper lacks the citation apparatus expected for [master's/doctoral/peer-review] work in international law."
3. Do not attempt detailed citation audit when no citations exist

### File Access Issues

If the submitted file cannot be read at all:

1. Report the specific error (e.g., "File appears to be password-protected," "File format not supported")
2. Ask the professor to resubmit in a supported format
3. Do not generate a review memorandum for unreadable files
