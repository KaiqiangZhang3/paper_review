# International Law Paper Review

A specialized Claude Code skill for reviewing international law academic papers with professor-facing diagnostic analysis.

## What This Skill Does

Reviews student papers, thesis chapters, and peer-review manuscripts in international law fields, providing:

- **Structure reconstruction** before evaluation
- **Multi-dimensional legal assessment** (thesis, sources, reasoning, literature, structure, citations, counterarguments)
- **Direct diagnostic feedback** identifying fatal vs. reparable defects
- **Professor-facing internal memoranda** (not student-facing feedback)
- **Bilingual support** (Chinese/English)

## Supported Review Types

- **Master's papers** — assessing legal training and scholarly argument at master's level
- **Doctoral papers** — evaluating advanced scholarly contribution and originality
- **Peer-review manuscripts** — assessing publishability and contribution to field

## Supported Fields

- Public international law (default)
- International economic law
- International criminal law
- Mixed fields

## Installation

### Via NPX (Recommended)
```bash
npx --yes skills add https://github.com/KaiqiangZhang3/paper_review
```

### Manual Installation
```bash
git clone https://github.com/KaiqiangZhang3/paper_review.git
cd paper_review
# Follow Claude Code skill installation instructions
```

## Usage

1. **Invoke the skill** in Claude Code:
   ```
   /international-law-paper-review
   ```

2. **Answer intake questions** (presented all at once):
   - Paper type (master's/doctoral/peer-review)
   - Material type (full paper/chapter/abstract/outline)
   - Field (public/economic/criminal international law)
   - Output language (Chinese/English)
   - Special rubric or standards
   - Citation review needed?
   - Counterargument review needed?

3. **Provide the paper** (PDF, Word, Markdown, or pasted text)

4. **Receive two outputs**:
   - Conversation memorandum
   - Saved file in `reviews/YYYY-MM-DD-<paper-title>-review.md`

## Key Features

### Smart Intake
- All questions asked at once by default
- Automatic inference of missing information
- Explicit disclosure of defaults used

### Rigorous Assessment
- Three-layer legal assessment (lex lata / lex ferenda / academic standard)
- Claim-strength calibration (checking if conclusions overreach evidence)
- Adverse-authority stress testing (identifying strongest objections)
- Citation audit (substantive quality, not just formatting)

### Location Precision
- Problems tied to specific pages, sections, paragraphs, or footnotes
- Traceable diagnostic findings

### Error Handling
- Handles extraction failures gracefully
- Adapts to partial materials (abstracts, outlines)
- Processes very short submissions appropriately
- Identifies missing thesis as primary defect

## File Outputs

Review files are saved with paper titles in the filename:

```
reviews/2026-06-27-climate-change-and-state-responsibility-review.md
reviews/2026-06-27-国际投资仲裁中的透明度问题研究-review.md
```

Chinese titles are preserved natively. Long titles are truncated with hash suffixes for uniqueness.

## Batch Review

For multiple papers:
- Process one paper fully before the next
- One memorandum file per paper
- Recommended maximum: 6 papers per batch

## Not Included By Default

This skill does NOT automatically provide:
- Numerical grades or scores (ask explicitly if needed)
- Student-facing feedback (professor-facing by default)
- Paragraph-by-paragraph marginal comments
- Priority repair checklists
- Comparative batch rankings

## Version

Current version: **1.9.0** (2026-06-27)

### What's New in v1.9.0

**Four-Dimension Framework Now Universal** — Applied to ALL papers with adjusted expectations:

Four evaluation dimensions now assess scholarly awareness at all levels:

1. **Problem Scope and Scale (多大的事儿)** — Does the paper clearly articulate what problem it addresses and at what level of significance?
2. **Methodological Path Selection (脉络选择)** — Does the paper identify its analytical framework and (for advanced work) justify it?
3. **Contribution and Challenge (贡献/挑战)** — Does the paper explicitly state what it contributes or challenges?
4. **Adverse Scholarship Engagement (学术挑战的处理)** — Does the paper identify and engage with contrary scholarly positions?

**Application by paper type**:
- **Doctoral**: Full rigor on all four dimensions
- **Peer-review**: Full rigor (maps to common reviewer objections)
- **Master's**: Moderate expectations, adjusted to program level
- **Coursework**: Selective, focus on problem clarity and contribution

Previously (v1.5.0) these were only for doctoral work. v1.9.0 recognizes that these are fundamental questions of scholarly practice at all levels, just with different expectations.

See [CHANGELOG.md](./CHANGELOG.md) for full version history.

## License

[Specify your license here]

## Author

Kaiqiang Zhang

## Feedback and Issues

Report issues at: https://github.com/KaiqiangZhang3/paper_review/issues
