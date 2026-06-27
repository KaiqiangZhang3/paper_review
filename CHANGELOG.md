# Changelog

All notable changes to this skill will be documented in this file.

## [1.9.0] - 2026-06-27

### Major Change: Four-Dimension Framework Now Universal

**Breaking conceptual change**: The four assessment dimensions introduced in v1.5.0 for doctoral work are now applied to **ALL papers** (master's, doctoral, peer-review, coursework), with expectations adjusted by paper type.

### Rationale

These dimensions assess fundamental scholarly awareness that should be present at all levels:
- **Problem clarity** matters for all academic work
- **Methodological awareness** helps even master's students understand what they're doing
- **Contribution articulation** distinguishes argument from description at all levels
- **Literature engagement** is expected even in coursework papers

The difference is **rigor and depth**, not presence/absence.

### Changed

**File renamed**:
- `references/thesis-assessment-framework.md` → `references/four-dimension-framework.md`

**Application rules revised**:
- **Doctoral dissertations**: Full rigor on all four dimensions (unchanged from v1.5.0)
- **Peer-review manuscripts**: Full rigor, especially Dimensions 2, 3, 4 (maps to common reviewer objections)
- **Master's papers**: Moderate expectations adjusted to program level (NEW)
- **Coursework papers**: Selective application, focus on Dimensions 1 and 3 (NEW)

**Mode standards enhanced**:
- All three mode standards (Master's, Doctoral, Peer-Review) now include four-dimension guidance
- Each mode specifies adjusted expectations
- Common defects updated to include dimension-specific issues

**Memorandum template updated**:
- Section title changes by paper type: "Four-Dimension Assessment" (doctoral/peer-review) or "Scholarly Awareness Assessment" (master's)
- Each dimension's template now includes adjusted expectations for different paper types

**SKILL.md updated**:
- `four-dimension-framework.md` is now mandatory reference for all papers (not conditional)

### Philosophy

v1.5.0 created these dimensions for doctoral work because that's where they're most critical. v1.9.0 recognizes that these are fundamental questions of scholarly practice that apply at all levels, just with different expectations.

A master's paper should still articulate what problem it addresses (Dimension 1), even if the scope is narrower than doctoral work. A peer-review manuscript must explicitly state its contribution (Dimension 3) or face "so what?" from reviewers.

### Backward Compatibility

Reviews of doctoral work are unchanged in rigor from v1.5.0. Reviews of master's and peer-review work gain additional diagnostic dimensions that were previously implicit in "Literature Engagement" and "Research Question" assessments.

---

## [1.5.0] - 2026-06-27

### Added - Thesis-Specific Assessment Framework

**New reference file**: `references/thesis-assessment-framework.md`

Four new assessment dimensions for **doctoral dissertations and thesis chapters**:

1. **Problem Scope and Scale (多大的事儿)**
   - Assesses whether the thesis clearly articulates what problem or theoretical question it addresses
   - Evaluates problem significance and boundary definition
   - Identifies scope inflation, unstated boundaries, and problem-solution mismatch

2. **Methodological Path and Alternatives (脉络选择)**
   - Assesses whether the thesis explains its chosen analytical framework (doctrinal, theoretical, empirical, normative, institutional)
   - Evaluates whether alternatives are acknowledged and the chosen path is justified
   - Identifies methodological silence, method-problem mismatch, and unacknowledged alternatives

3. **Contribution and Challenge (贡献/挑战)**
   - Assesses whether the thesis explicitly states what it contributes or challenges
   - Evaluates whether contribution is demonstrated vs. merely asserted
   - Distinguishes doctrinal refinement, theoretical framework, empirical finding, normative critique, and institutional design contributions
   - Identifies contribution by topic selection alone, implicit contributions, and overstated/understated claims

4. **Adverse Scholarship Engagement (学术挑战的处理)**
   - Assesses whether the thesis identifies scholarship that challenges its claims
   - Evaluates whether contrary positions are addressed substantively in analytical chapters (not just cited in literature review)
   - Identifies strawman engagement, citation without engagement, and evasion through scope claims

### Changed

- **Doctoral Paper mode standard** enhanced with thesis-specific dimensions
- **Memorandum template** now includes "Thesis-Specific Assessment" section for doctoral work
- **SKILL.md** now requires reading `thesis-assessment-framework.md` for doctoral dissertations

### Design Philosophy

These dimensions assess **scholarly self-awareness**: whether the doctoral candidate understands what they are doing, why, and how it fits into existing scholarship. They supplement rather than replace standard legal review dimensions.

---

## [1.1.0] - 2026-06-27

### Added
- **One-time intake questioning**: All 7 intake questions now presented at once by default for better user experience
- **Smart defaults**: Automatic inference of missing intake information with explicit disclosure
- **Error handling**: Comprehensive edge case handling for extraction failures, missing thesis, short materials, mixed languages, and file access issues
- **Concrete examples**: Format examples in memo-template.md showing diagnostic structure and language style
- **Enhanced file naming**: Paper titles now included in review file names with collision handling and length limits
- **Diagnostic language patterns**: Explicit guidance on direct vs. weak language in SKILL.md
- **Problem entry format**: Structured format for location + diagnosis + severity in problem descriptions

### Changed
- **Intake flow**: Default changed from sequential questioning to batch presentation (interactive mode still available on request)
- **Output file protocol**: Now extracts paper titles with priority order (metadata → heading → filename → fallback)
- **File naming strategy**: Supports Chinese titles natively, adds hash suffix for long titles, handles collisions with counters

### Improved
- **Location precision**: Enhanced guidance on using page/section/paragraph references
- **Judgment style**: More specific examples of diagnostic sentences
- **Template flexibility**: Examples explicitly marked as format guides, not rigid templates

## [1.0.0] - 2026-06-01

### Added
- Initial release
- Support for master's, doctoral, and peer-review manuscript modes
- 7-dimension review framework
- Citation audit capability
- Bilingual support (Chinese/English)
- Structure reconstruction methodology
- Legal assessment tests (three-layer, claim-strength calibration, adverse-authority stress test)
- Professor-facing internal memorandum output

### Reference Standards
- `mode-standards.md`: v1.0
- `review-dimensions.md`: v1.0
- `legal-assessment-tests.md`: v1.0
- `citation-audit.md`: v1.0
- `structure-reconstruction.md`: v1.0
- `memo-template.md`: v1.0
- `output-file-protocol.md`: v1.0
