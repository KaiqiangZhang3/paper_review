# Changelog

All notable changes to this skill will be documented in this file.

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
