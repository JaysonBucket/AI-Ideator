## RELEASE NOTES

## v2.4/2.41 - 15.02.2026
- Added clear Agent Builder vs. Copilot Studio decision logic, including capabilities, limits, and when to choose each.
- Integrated agent decision flow into the tooling cascade, keeping native → Copilot → Agent → Azure sequencing.
- Added concise agent discovery questions to guide users toward the right platform.
- Kept all existing functionality, including full schema, Excel generation, interview modes, and reframing logic.
- Improved checks for governance, publishing, collaboration, and integrations in agent scenarios.

## v2.3 - 15.02.2026
This update delivers a fully refactored, language‑agnostic Agent Instruction YAML designed for reliable use in Microsoft Agent Builder. The configuration is streamlined, fully English, and optimized for stability, minimal hallucinations, and complete Excel output consistency.

##### Key Improvements
- Reworked language logic: agent now responds in any user language, not just EN/DE
- Cleaned and consolidated YAML structure for stronger LLM adherence
- Simplified Excel schema with unified Copilot and Missing columns
- Strengthened grounding, boundary‑checks, and non‑hallucination rules
- Improved clarity in tooling cascade (M365 → Copilot → Agent Builder → Azure)
- Full schema and process canvases validated and aligned with final structure
- Removed redundant or restrictive rules; updated phrasing for universality
- Reduced verbosity while maintaining full functionality
- Ensured YAML validity and Agent Builder compatibility
- Updated language behavior to be fully global and inclusive

## v2.1 - 14.02.2026
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

## 13.02.2026 initial commit


