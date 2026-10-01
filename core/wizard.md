# Wizard

## Principle

Guide, do not interrogate. Infer what is already available from the conversation and materials. Ask only for information that materially changes the test.

The wizard should feel like guided research setup, not a form.

## Progress

Maintain these states internally:

`ENVIRONMENT → PROJECT → FIDELITY → MATERIALS → PERSONAS → LEARNING GOALS → MISSIONS → TEST PLAN → RUN → SYNTHESIS → REPORT`

Do not force the user to see every state. Surface progress when it helps orientation.

## State behavior

### Environment
Detect only capabilities relevant to the requested test. Do not block setup because an optional integration is absent.

### Project
Understand what is being tested, why now, and which decision the test should inform. Reuse supplied context.

### Fidelity
Classify the material before choosing evaluation criteria. If uncertain, ask a short question or infer provisionally and confirm.

### Materials
Inventory available screens, files, flows and integrations. Distinguish verified states/transitions from unknown ones.

### Personas
Reuse approved personas when available. Otherwise offer to import, create with the user, or generate clearly provisional personas. Never silently rewrite an approved persona.

### Learning goals
Translate broad business questions into research questions and hypotheses without manufacturing evidence.

### Missions
Create neutral, realistic tasks relevant to each persona. Avoid labels, wording or hints that disclose the intended path.

### Test plan
Before execution, summarize what will be tested, with whom, at what fidelity, using which materials, missions and evidence boundaries. If the user already approved an equivalent plan, do not ask for redundant confirmation.

### Run
Keep persona runs independent. Start with unprimed exploration when applicable, then mental model, then missions.

### Synthesis
Look for patterns and divergences without turning repetition among synthetic personas into statistical evidence.

### Report
Lead with a concise decision-oriented summary, then supporting findings, hypotheses, recommendations and limitations.

## Adaptive questioning

- Skip answered questions.
- Prefer one focused question at a time when the answer determines the next branch.
- Group questions only when they are independent and easy to answer together.
- If enough information exists to continue safely, continue.
- If a missing answer changes methodology or could invalidate the test, ask before continuing.
- Do not repeatedly ask the user to confirm obvious or reversible steps.

## Fidelity behavior

For concepts and journeys, prioritize comprehension, value proposition, architecture, expectations and mental model.

For wireframes, prioritize comprehension, hierarchy, findability, flow, labels and journey logic. Do not treat unfinished visual polish as a finished-interface defect.

For hi-fi prototypes, visual hierarchy, affordance, consistency and presentation may be evaluated in addition to journey and mental model.

## Language

Run the complete wizard in the user's language by default. Recognize equivalent natural-language commands, not only literal command strings.
