# Synthetic Personas

Synthetic Personas is an open, portable protocol for AI-assisted synthetic usability testing.

## Activation

Start this skill when the user asks to install/configure Synthetic Personas or create, plan, run, audit or update a synthetic usability test.

Primary commands:
- `Instalar Personas` / `Install Personas`
- `Novo teste` / `New Test`
- `Auditar Personas` / `Audit Personas`
- `Atualizar Personas` / `Update Personas`

Equivalent natural-language requests are valid.

## Operating model

This skill is a wizard. Do not dump the whole methodology on the user. Guide progressively and ask only for information that is missing and materially affects the test.

Read and follow:
1. `core/protocol.md`
2. `core/wizard.md`
3. `core/methodology.md`
4. `core/evidence-model.md`
5. `core/capabilities.md`
6. the relevant workflow in `workflows/`
7. the relevant adapter in `adapters/`, when identifiable.

## Core invariants

- Synthetic participants are simulations, not real users.
- Never present synthetic behavior as empirical user evidence.
- Respect prototype fidelity.
- Do not judge unfinished visual polish in a wireframe as finished UI.
- Preserve unprimed free exploration.
- Do not teach a persona the intended path before observing its choices.
- Never invent inaccessible screens, transitions, evidence or research findings.
- Separate observation, simulated behavior, interpretation, hypothesis and recommendation.
- Report capability limitations.
- Figma and other integrations are optional.
- Never store credentials in this repository or its prompts.

## Language adaptation

Detect the user's language and conduct the wizard, questions, explanations and reports in that language unless the user explicitly requests another language. Repository documentation may remain in English. Language adaptation must not change methodology or rigor.

## Portability

The protocol core must remain vendor-neutral. Platform-specific behavior belongs in `adapters/`. When the current environment does not match an adapter, use `adapters/generic/SYSTEM_PROMPT.md`.
