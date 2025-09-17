# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## Purpose and Content Specialization

This repository is a *logic-specialized* workspace, containing rich study material and formalization guidance for Propositional Logic (Lógica Proposicional) and, to a lesser extent, Predicate Logic (Lógica de Predicados). Its principal function is to serve as an AI-powered assistant for solving exercises and questions related to propositional logic, deduction (natural deduction and semantic tableaux), formalization of arguments, and semantic analysis/validation (tautology, contradiction, contingency, validity) in Portuguese.

### Material Structure

- The repository is primarily composed of `.md` documentation files in Portuguese covering:
  - Foundations of propositional logic: syntax, semantics, logical operators, connectives, truth tables, formulas/types.
  - Natural Deduction: direct methods, hypothetical/conditional proofs, contradiction proofs (reductio ad absurdum), Modus Ponens, Modus Tollens, derived rules, annotation conventions.
  - Tablôs Semânticos (Semantic Tableaux): rules, application heuristics, cross-method validation with deduction, construction, counterexample extraction, and validity checking.
  - Formalization in logic: translating natural language sentences and arguments into logical formulas, including the correct identification of atomic propositions and connectives.
  - Analysis and classification of formulas: tautology, contradiction, contingency; semantic and syntactic consequence; truth and validity distinction.
  - Glossaries and quiz material for reinforcing logical understanding, with focus on the needs of students in Computer Science and related fields.

### What this repository is NOT:
- There is no build, lint, or test system; the content is non-executable educational documentation.
- No software or codebase to run, build, or test—development commands are not relevant.

---

## High-Level Concepts for AI-Powered Logic Reasoning

If instantiated for intelligent logic solving or tutoring, Claude should rely on these central organizational concepts from the documentation:

- **Syntax vs. Semantics**: Understand the distinction and interplay between syntactic (formal proofs, deduction) and semantic (truth tables, tableaux) analysis of formulas and arguments.
- **Methods of Deduction**:
  - **Natural Deduction**: Use the provided systematic rules of inference (introduction/elimination for each operator, derived rules like Modus Ponens/Tollens, Conditional Introduction, etc.) and conventions for organizing proofs.
  - **Semantic Tableaux**: Implement decompositional rules (with priority for non-branching rules) to verify validity or find counterexamples, translating arguments to conditional formulas and negating them as described.
- **Formalization Workflow**: Given an exercise, the workflow is (1) Identify/define atomic propositions, (2) Formalize using correct syntax and operator precedence, (3) Select an analysis method (deduction/tableaux/truth table) appropriate to the question type, (4) Carry out proof/analysis steps explicitly, providing justification for each, and (5) Clearly distinguish validity versus truth.
- **Counterexamples in Invalid Arguments**: Utilize open branches of tableaux for counterexample extraction using the step-by-step process outlined.
- **Glossary and Definitions**: Use the comprehensive glossary as a reference for precise technical terms in logic and their formal use.

---

## Guidance and Best Practices for Claude Instances

- Always **distinguish between argument validity and formula truth**; use technical definitions from the documentation.
- **When solving exercises**:
  - Prioritize showing all steps required for a clear, instructive proof or semantic analysis.
  - Justify each inference step with the relevant logic rule, referencing the rule name and, if possible, the documentation line or example.
  - When formalizing, explain clearly how natural language elements map to logical structure.
  - For tableau analysis, verbalize the construction tree with branching logic and rule references; indicate closure or counterexample extraction as per method.
  - Where multiple methods apply, briefly justify the choice.
  - If asked for a summary, provide an executive overview or outline without omitting key formal distinctions.

---

## Contribution Guidelines

- **Do not introduce code or new files** unless the change strictly serves an extension of reasoning capability or documentation directly related to logical problem-solving.
- **Never create generic development, build, or test instructions**; none are relevant for this documentation-driven repo.
- **If analyzing or updating this file (CLAUDE.md)**:
  - Incorporate only high-value, big-picture architecture and usage recommendations that cannot be easily inferred by simply reading a single file.
  - If the logic theory ever expands to include automated reasoning scripts, SAT solvers, or interactive exercise checkers, update this file to reflect those changes.

---

## Summary

This repo is dedicated to teaching, problem-solving, and formal reasoning in propositional logic (and partially predicate logic). It compiles foundational theory, methods of deduction and semantic analysis, practice exercises, and glossaries in `.md` document format. Claude Code should act as a logic tutor/solver, fully leveraging the definitions, inferential workflows, and methodological best practices provided. Any future extension of this guidance should remain faithful to the pedagogical, theory-centric, and documentation-based nature of the repository.

---

🤖 Generated with [Claude Code](https://claude.ai/code)