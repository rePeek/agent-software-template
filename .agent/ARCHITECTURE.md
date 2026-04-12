# Agent Architecture

## Project Operating Rules

This repository is a generic template for agent-oriented software projects. It organizes agent work around a small set of operating assets: processes, skills, and rules.

`AGENTS.md` is the repository-wide operating contract. It defines the project goal, directory semantics, core objects, invariants, and output standards.

`.agent/ARCHITECTURE.md` defines how the project operates and keeps the lightweight registry for reusable agent assets.

`.agent/process/` contains repeatable execution processes for common work.

`.agent/skills/` contains scoped task capabilities or instructions.

`.agent/rules/` contains durable behavioral or technical constraints.

The agent runtime is the active executor. It reads the repository contract, selects or creates a process, applies relevant skills and rules, performs the work, and records any maintenance needs.

Agents should use process-first execution. Before substantial work, an agent should look for an applicable process. If one exists, the agent should follow it and apply relevant skills and rules.

If no existing process applies, the agent may create a process when the work is within the repository goal and could plausibly repeat. The process should be small, explicit, and recorded in the registry section below.

Processes should be maintained when repeated work exposes ambiguity, missing steps, missing inputs, missing outputs, or unnecessary friction. Similar processes should be consolidated when they repeat the same pattern or overlap in purpose.

======================

## Registry Notes

The registry below is a lightweight index for reusable agent assets. It is not a substitute for full process, skill, or rule files. Each entry should stay brief and point to the canonical file when one exists.

## Processes

Processes define repeatable execution paths for common work. Agents should prefer an existing process before creating a new one. New process entries should describe the trigger, purpose, canonical path or notes, and current status.

| Name | Path or Notes | Purpose | Status |
| --- | --- | --- | --- |
| _None yet_ | | | |

## Skills

Skills define scoped task capabilities, specialized instructions, or reusable task knowledge. Add a skill when repeated specialized work appears and a process alone is not enough.

| Name | Path | Purpose | Status |
| --- | --- | --- | --- |
| _None yet_ | | | |

## Rules

Rules define durable constraints that agents must follow across processes and skills. Add a rule when a constraint should apply broadly and remain stable over time.

| Name | Path | Purpose | Status |
| --- | --- | --- | --- |
| _None yet_ | | | |
