# Copilot Instructions for LARRY's Team Repository

## Purpose
This repository documents and operates LARRY's Team — a small, role-driven AI orchestration framework. Use this file as the entrypoint for Copilot sessions: it explains where to start, how work is routed, and repository-specific conventions Copilot should follow. chg1

---

## Build, test, and lint commands
- No language/runtime manifests (package.json, pyproject.toml, Makefile, etc.) or test frameworks were detected. There are no repository build, test, or lint commands to run.
- If this repository later adds a test command, include an explicit single-test invocation example here (e.g., `pytest tests/path/to/test_file.py::test_name` or `npm test -- test/file.spec.js -t 'single test name'`).

---

## High-level architecture (big picture)
- Purpose: documentation & orchestration for an AI team (LARRY, PAX, NOLAN).
- Key directories:
  - /Agents/ — primary source of truth for team roles, personas, workflows, and expansion protocol.
  - Root — includes images and other assets related to tasks (visual diff examples, PDFs).
- Typical flow: External request → Agents/LARRY.md (entrypoint) → consult Agents/Team-Members/*.md (capabilities) → follow Team Expansion Protocol when new skills are needed.

---

## Key conventions (repo-specific)
- Agent profiles live under Agents/ and follow a consistent structure: Role, Persona, Identity, Responsibilities, Deliverables, Methodology.
- Use LARRY.md as the session orchestration guide. All Copilot sessions should consult it first to determine delegation logic.
- When adding a new agent, create Agents/Team-Members/Name.md and update Agents/TEAM-STRUCTURE.md.
- Visual assets live at repo root (images/*.jpg/png). Avoid auto-presenting visual diffs unless confidence is high — follow the principle in Agents/LARRY.md about surfacing only meaningful visual differences.
- No CI workflows detected. If workflows are added, document common workflow names and how they map to commands (e.g., `ci/test`, `ci/lint`).

---

## Other AI assistant configs checked
Checked for common assistant config files and rules; none found: CLAUDE.md, .cursorrules, AGENTS.md, .windsurfrules, CONVENTIONS.md, .clinerules, .clinerules, .cursorrules.

---

## How Copilot sessions should proceed
1. Read this file and Agents/LARRY.md first.
2. If the request is to implement or change behavior, open the relevant Agent profile(s) under Agents/Team-Members/ and TEAM-STRUCTURE.md to understand persona/responsibility.
3. If new expertise is required, follow the Team Expansion Protocol: ask Pax for research, then Nolan for sourcing.
4. When modifying repository docs, prefer small, surgical edits and update TEAM-STRUCTURE.md and affected agent profile(s).

---

## Updating these instructions
- Keep this file focused on repository-specific workflow and machine-readable hints for Copilot sessions (entrypoints, where to look, and conventions).
- Avoid generic developer advice.

---

## Contact points
- Orchestration & entrypoint: Agents/LARRY.md
- Research needs: Agents/Team-Members/Pax.md
- Hiring/sourcing: Agents/Team-Members/Nolan.md

---

Summary: consolidated existing guidance, added explicit startup steps for Copilot, documented that no build/test/lint commands exist, and listed repo-specific conventions and important files.
