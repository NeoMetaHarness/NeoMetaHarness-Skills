# AGENTS.md: NeoMetaHarness-Skills

Owns: Published skill packs (agentskills.io), skills registry, promotion and eval rules.

- Promote Skills from validated evidence.
- Every Skill has an autonomy ceiling agents cannot silently exceed.
- Skill improvement creates a candidate version, runs evaluations, and preserves rollback.
- Never store secrets, API keys, session tokens or private user data.

## GitHub safety circuit breaker
Follow `docs/policies/GITHUB-SAFETY-GUARDRAILS.md` and `machine/github-guardrails.json` (mode `local_only_no_actions`): no GitHub Actions, work and test locally, at most 20 GitHub writes per task, stop on 403/429 and ask a human.
