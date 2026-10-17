# CLAUDE.md

The [Channel] Partner Experience API. Owned by the channel team. Ground rules live in the
[ai-intelligence-domain](https://github.com/azure-intelligence-domain/ai-intelligence-domain)
repository (ADR 0017 experience layer).

- No code: `openapi.yaml` is a subset of the 3PL System API's contract, served by the gateway under
  `/partner` with the partner's sign-in. Every operation must exist, with the same shape, in the
  released 3PL System API the gateway calls.
- Contract first, with a higher `info.version` on every change.
