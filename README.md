# officialwhitebird

A local-first garage for small, single-purpose CLI tools designed to make AI-orchestration boundaries explicit.

AI coding agents function most reliably when their operational entry and exit boundaries are clearly structured. This space provides offline, deterministic checkers to verify instructions before runs begin and to audit documentation before public release.

## Selected Tools

| Repository | Boundary | What it checks |
|---|---|---|
| [handoff-lint](https://github.com/officialwhitebird/handoff-lint) | Input Boundary | Verifies coding-agent work instructions and scope bounds before execution |
| [contract-lint](https://github.com/officialwhitebird/contract-lint) | Execution-Contract Boundary | Validates a completed run record against its declared contract (outputs, verification, gates) before the result is trusted |
| [claim-lint](https://github.com/officialwhitebird/claim-lint) | Output Boundary | Audits public-facing documents for unevidenced claims and internal leakages before publication |

## Stance

* Local-first and offline: Every checker runs on your machine with no external network requirements.
* Bounded and deterministic: We prioritize simple string, JSON, or regex matching over subjective evaluation or language model judgment.
* Human in the loop: These utilities help visualize mechanical omissions, leaving final validation and authority to the human operator.
