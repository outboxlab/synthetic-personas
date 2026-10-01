# Synthetic Personas 🧪

**Test ideas before testing people.**

Synthetic Personas is an open protocol for AI-assisted synthetic usability testing across LLMs and agent environments.

> Public beta: `v0.1.0-beta`

It guides AI agents through structured synthetic usability tests for concepts, journeys, wireframes and prototypes while keeping simulated behavior clearly separated from real user evidence.

## What it does

The conversational wizard helps you define the research goal, understand prototype fidelity, inspect available materials, select or create personas, formulate neutral missions, run the simulation and synthesize findings.

You do not need to know how to structure a usability test before starting.

## Quick start

### ChatGPT
Provide this repository or its files to a ChatGPT environment that can read them. Start with `SKILL.md`, then say `Install Personas` or `Instalar Personas`.

### Claude
Make the repository files available in the Claude environment/project. Start with `SKILL.md` and `adapters/claude/SKILL.md`, then say `Install Personas`.

### Hermes
Make the repository available to the Hermes workspace/agent. Load `SKILL.md` and `adapters/hermes/SKILL.md`, then say `Install Personas`.

### Other agents
Load `SKILL.md` and `adapters/generic/SYSTEM_PROMPT.md`. The protocol will adapt to the capabilities actually available.

> Exact installation mechanics vary by host. Synthetic Personas does not require a specific vendor, MCP server or design integration.

## Your first test

After setup, say `New Test` or its equivalent in your language. The wizard will progressively guide you through:

`Project → Fidelity → Materials → Personas → Learning goals → Missions → Test plan → Run → Synthesis → Report`

It skips information you already provided instead of turning setup into a questionnaire marathon.

## Inputs

Use whatever the environment supports:
- connected design sources such as Figma;
- screenshots or images;
- PDFs;
- accessible prototype links;
- user-described journeys.

Figma is optional.

## Method

The default test sequence is:
1. free exploration without mission or priming;
2. mental-model investigation;
3. persona-specific neutral missions;
4. consolidation across personas;
5. findings, uncertainties, hypotheses and recommendations.

Evaluation changes with fidelity. A wireframe is evaluated as a wireframe, not as finished visual design.

## Example

See `examples/first-test.md` for a compact end-to-end example.

## Architecture

- `core/` — vendor-neutral protocol, wizard, methodology, capabilities and evidence model
- `workflows/` — install, new test, run, audit and update flows
- `adapters/` — environment-specific mappings
- `integrations/` — optional design-source integrations
- `personas/` — persona schema and examples
- `templates/` — reusable briefing, test-plan and report structures
- `examples/` — runnable examples

## Research integrity

Synthetic participants are simulations. They can help explore hypotheses, identify potential friction, rehearse journeys and prepare real research, but they are not substitutes for empirical user evidence.

The protocol separates provided evidence, synthetic behavior, interpretation, hypotheses, recommendations and unknowns.

## Language

Repository documentation is maintained in English for portability and open-source collaboration. The wizard itself is multilingual and should automatically use the user's language unless asked otherwise.

## Feedback

This beta is intentionally public. Feedback, test cases, adapter contributions and methodological critiques are welcome through GitHub Issues and pull requests.

Use the issue templates for beta feedback, methodology feedback, bugs or adapter requests.

## License

A project license is being selected during the public beta. Until a license is added, default copyright rules apply.

## Version

`0.1.0-beta`
