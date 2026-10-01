# Synthetic Personas 🧪

**An open protocol for AI-assisted synthetic usability testing across LLMs and agent environments.**

> Public beta: `v0.1.0-beta`

Synthetic Personas is a conversational wizard for planning, conducting and interpreting synthetic usability tests. It is vendor-neutral at the core and designed to run across ChatGPT, Claude, Hermes and other agent environments.

## Start

Load the repository in your AI environment and say:

`Install Personas`

Localized commands are supported, for example `Instalar Personas` in Portuguese. Then use `New Test` or its equivalent in your language.

The wizard guides you through project context, fidelity, materials, personas, hypotheses, missions, test planning, execution and reporting.

## Architecture

- `core/` — vendor-neutral protocol, wizard, methodology and evidence model
- `workflows/` — install, new test, run, audit and update flows
- `adapters/` — environment-specific mappings
- `integrations/` — optional design-source integrations
- `personas/` — persona schema
- `templates/` — reusable test and report structures

## Inputs

Connected design sources such as Figma may be used when supported. Screenshots, images, PDFs and user-described journeys remain valid fallbacks.

## Research integrity

Synthetic participants are simulations. They can help explore hypotheses, identify potential friction, rehearse journeys and prepare real research, but they are not substitutes for empirical user evidence.

The protocol separates provided evidence, synthetic behavior, interpretation, hypotheses, recommendations and unknowns.

## Language

Repository documentation is maintained in English for portability and open-source collaboration. The wizard itself is multilingual and should automatically use the user's language unless asked otherwise.

## Beta feedback

Feedback, test cases, adapter contributions and methodological critiques are welcome through GitHub Issues and pull requests.

## Version

`0.1.0-beta`
