# Output File Protocol

Each reviewed paper must produce two outputs:

1. A review memorandum in the conversation.
2. A Markdown file saved in the workspace.

## Default File Location

Save review files under:

```text
reviews/YYYY-MM-DD-<sanitized-title>-review.md
```

Use the current date from the runtime environment.

### Title Extraction Priority

Extract the paper title in this order:

1. **From document metadata** (if PDF/Word has title field)
2. **From first heading** (# or ## in Markdown, or largest heading in document)
3. **From file name** (remove extension and path)
4. **Fallback**: Use material type + timestamp (e.g., `master-paper-143022`)

**Always include the paper title in the file name** to make reviews easily identifiable.

## Sanitizing Titles

### Basic Rules

Create file names by:

1. Extract core title words (remove subtitles after colons if title is long)
2. For **English titles**:
   - Lowercase all characters
   - Replace spaces with hyphens
   - Remove punctuation: `.,;:!?'"()[]{}` → removed
   - Keep only: `a-z`, `0-9`, `-`
   - Example: "Climate Change and State Responsibility: A Critical Analysis" → `climate-change-and-state-responsibility`

3. For **Chinese titles**:
   - Keep Chinese characters as-is (do not transliterate)
   - Remove punctuation: `，。；：！？""''（）【】《》` → removed
   - Example: "气候变化与国家责任：批判性分析" → `气候变化与国家责任`

4. For **Mixed-language titles**:
   - Keep both language parts
   - Example: "论WTO争端解决机制的改革" → `论wto争端解决机制的改革`

### Length Limits

- **Maximum 60 characters** for the sanitized title portion
- If title exceeds 60 characters:
  1. Truncate at last complete word before 60-char limit
  2. Append 4-character hash for uniqueness
  3. Example: `climate-change-state-responsibility-emerging-norms-customary-international-law` (85 chars) → `climate-change-state-responsibility-emerging-norms-a3f9`

### Collision Handling

If a file with the same name already exists:

1. Check if content is identical → skip saving duplicate
2. If content differs, append counter: `-2`, `-3`, etc.
   - Example: `2026-06-27-climate-refugees-review.md` → `2026-06-27-climate-refugees-review-2.md`

### Examples

```
Title: "国际投资仲裁中的透明度问题研究"
File:  reviews/2026-06-27-国际投资仲裁中的透明度问题研究-review.md

Title: "The Fragmentation of International Law"
File:  reviews/2026-06-27-the-fragmentation-of-international-law-review.md

Title: "论《联合国海洋法公约》中的专属经济区制度：以中国实践为中心的分析"
File:  reviews/2026-06-27-论联合国海洋法公约中的专属经济区制度-b7e4-review.md
       (truncated + hash due to length)

Fallback (no title available):
File:  reviews/2026-06-27-doctoral-paper-143022-review.md
```

## Batch Review

For multiple papers:

- Process one paper fully before starting the next.
- Generate one Markdown file per paper.
- Do not generate a comparative overview.
- Do not rank papers against each other.
- Treat six papers as the recommended maximum unless the professor explicitly asks to continue.

## Location References

When available, include page, section, paragraph, heading, or footnote references for important judgments.

If exact page references are unavailable, use the most precise available reference and state the limitation.

## Default Exclusions

Do not include these unless the professor asks:

- Score or grade.
- Student-facing or author-facing feedback.
- Paragraph-by-paragraph marginal comments.
- Priority repair checklist.
- Comparative batch overview.
- Claim of comprehensive external source verification.

Sharper diagnostic sections do not override these exclusions. Citation audits, claim-strength calibration, and adverse-authority testing are internal professor-facing diagnostic tools, not priority repair checklists or student-facing revision plans.

## Limited Material Statement

When reviewing partial material, include one sentence in the Evidence Limits section that states the review scope. Examples:

- "This memorandum reviews only the submitted abstract and cannot judge the full paper's evidentiary support."
- "This memorandum reviews the submitted chapter and does not assess the absent introduction, conclusion, or full citation apparatus."
- "This memorandum reviews the outline as a project design document rather than as a completed paper."
