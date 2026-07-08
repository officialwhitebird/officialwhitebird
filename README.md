# officialwhitebird

A local-first garage for small, single-purpose CLI tools designed to make AI-orchestration boundaries explicit.

AI coding agents function most reliably when their operational entry and exit boundaries are clearly structured. This space provides offline, deterministic checkers to verify instructions before runs begin and to audit documentation before public release.

## Selected Tools

| Repository | Boundary | What it checks |
|---|---|---|
| [handoff-lint](https://github.com/officialwhitebird/handoff-lint) | Input Boundary | Verifies coding-agent work instructions and scope bounds before execution |
| [contract-lint](https://github.com/officialwhitebird/contract-lint) | Execution-Contract Boundary | Validates a completed run record against its declared contract (outputs, verification, gates) before the result is trusted |
| [policy-lint](https://github.com/officialwhitebird/policy-lint) | Execution-Authorization Boundary | Classifies a proposed command against a declared local policy (allow / owner-gate / reject / forbidden) before it runs |
| [claim-lint](https://github.com/officialwhitebird/claim-lint) | Output Boundary | Audits public-facing documents for unevidenced claims and internal leakages before publication |
| [officialwhitebird-boundary-skills](https://github.com/officialwhitebird/officialwhitebird-boundary-skills) | Run Boundary Pack | Routes AI-run boundary checks across handoff-lint, policy-lint, contract-lint, and claim-lint with a local case study |
| [video-automation-skill](https://github.com/officialwhitebird/video-automation-skill) | Media Workflow Boundary | Routes local video cut, subtitle, smart-cut, and export workflows with preview, overwrite, and API gates visible |

## Product Experiments

| Repository | Product | What it does |
|---|---|---|
| [quadview](https://github.com/officialwhitebird/quadview) | Windows Image Comparison | Compares local JPEG/PNG images in 1, 2, or 4 panes with synchronized zoom and pan |

## Writing

* [How I Run an AI Software Factory: Distributed Agents, Boundary Checks, and Evidence Trails](https://dev.to/whitebird_official_e89f70/how-i-run-an-ai-software-factory-distributed-agents-boundary-checks-and-evidence-trails-2i3) — how the four boundary checks fit together across a full AI coding run.

## Stance

* Local-first and offline: Every checker runs on your machine with no external network requirements.
* Bounded and deterministic: We prioritize simple string, JSON, or regex matching over subjective evaluation or language model judgment.
* Human in the loop: These utilities help visualize mechanical omissions, leaving final validation and authority to the human operator.

## Contact

Open to work on AI-orchestration tooling, agent workflows, and decision-support systems.

Reach me at officialwhitebird@gmail.com.
