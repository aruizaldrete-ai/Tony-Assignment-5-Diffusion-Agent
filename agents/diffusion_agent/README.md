# Assignment 5 Week 7 Emerging Technology Diffusion Agent

Version: 0.2-student. Specialty: Technology and Application Diffusion.

Assesses how far LLMs/Generative AI and the specified application have spread, what accelerates/inhibits diffusion, and bounded timing/peer-position implications. Applies Rogers' five characteristics separately without scores and uses adopter categories as qualified population-specific interpretations. Keeps general, application, and organization findings distinct within the unchanged common output contract.

## Cases
- cases/primary.json: industrial operations/maintenance knowledge assistant; petrochemical/energy; moderate/fast-follower; next 12–24 months.
- cases/contrast_1.json: marketing content and campaign ideation; consumer retail; aggressive/leading-edge; next 6–12 months.
- cases/contrast_2.json: exact primary case with only adoption_posture changed to conservative/risk-averse.

These are supplied hypothetical contexts, not observed deployments. Organizational posture is not measured market position.

## Workflow from scaffold root
```bash
python3 -B tools/build_prompt.py --agent agents/diffusion_agent --case agents/diffusion_agent/cases/primary.json
python3 -B tools/validate_response.py agents/diffusion_agent/responses/primary_response.json
python3 -B tools/check_frozen_core.py
```
The response validation command is for after an actual response has been saved. Repeat prompt construction with the contrast case paths. Run packets in ChatGPT with access to appropriate evidence, preserve actual JSON outputs under responses/, validate them, compare stable and changed conclusions, preserve a weakness, revise, retest, and complete records/agent_record.md. No API key is required.

## Status
Actual ChatGPT primary and context-contrast tests at v0.1 and the same-case primary retest at v0.2 are preserved and structurally valid. The v0.1 unsupported cross-application diffusion ranking is preserved in specialist_instructions.md; v0.2 requires comparable definitions, populations, geography, observation periods, adoption stages, and deployment-depth measures before ranking penetration. The primary retest explicitly abstains where evidence is incomparable. The Agent Record contains the student's supplied judgment and team handoff.

The v0.2 contrast and optional posture-only test were not run. The remaining broad-AI versus generative-AI evidence mismatch is documented. Source claims were researched in the supplied ChatGPT runs; Codex has not independently audited every external source. Structural validation does not establish factual accuracy.

Branch: lab5-diffusion-agent. See records/agent_record.md for candidate commit and repository status. GitHub publication and Brightspace submission remain separate steps. Existing specialists, core, tools, and template are preserved.
