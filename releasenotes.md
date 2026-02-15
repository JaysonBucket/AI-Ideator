## RELEASE NOTES

#### v2.1
Release date: 15.02.2026
Release version: v2.1

This release introduces major improvements to the Express Mode workflow and the Excel generation framework, enhancing guidance, structure, and user control. The update ensures reliability, full schema coverage, strict grounding to user inputs, and consistent multilingual behavior.

###### Added
- Introduced fully optimized **Agent Instructions** architecture aligned with Microsoft Agent Builder constraints.
- Implemented a unified **single-block YAML** layout (<8k chars) combining behavioral rules and static reference data.
- Added complete English-language normalization across all instruction layers.
- Added separation of:
  - Behavioral logic (LLM behavior & reasoning rules)
  - Static specification memory (schema, canvases, Excel output logic)

###### Changed
- Reworked instruction hierarchy for clarity, stability, and LLM adherence.
- Improved grounding rules to prevent hallucinations and enforce strict data fidelity.
- Refined tooling cascade (M365 → Copilot → Agent Builder → Copilot Studio → Azure).
- Updated Excel generation logic:
  - One row per schema field
  - Full workbook generation
  - “Not specified” + Missing/Helpful bullet rules
  - Enforcement of language‑specific columns (CopilotEN/DE, MissingEN/DE)

###### Improved
- Normalized and cleaned all schemas for Today, Tomorrow, Ideation, SolutionDraft, Implementation.
- Enhanced governance & compliance guardrails (Human‑in‑the‑loop, evidence, validation).
- Strengthened boundary checks for connectors, visibility, auth, DLP, and API limits.
- Reduced instruction length while preserving all key functionality.

###### Fixed
- Removed all leftover German content in system instructions.
- Eliminated duplicate or conflicting rule statements.
- Fixed inconsistent field names, column definitions, and structure deviations.
- Corrected formatting issues that previously caused YAML parsing failures.

#### 13.02.2026 initial commit


