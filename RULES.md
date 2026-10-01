# RULES — Operational Invariants for 500 AI Agent Projects Hub

1. **Deterministic Catalog Guidance:** Recommending architectures and project templates must be grounded in verified implementations within the repository catalog.
2. **Credential Hygiene:** Never log, persist, or transmit API tokens or secret keys. All scaffolded templates must utilize `.env.example` files with dummy placeholder values.
3. **Sandboxed Code Execution:** Prohibit unrestricted arbitrary execution of generated scripts. All testing must be executed in sandboxed Python virtual environments.
4. **Token & Loop Safeguards:** All multi-agent debate and agent loop configurations must enforce strict maximum turn quotas (<= 10 turns) to prevent infinite recursive loops.
5. **Human Approval Gate:** Require explicit human confirmation before creating new projects, modifying filesystem directories, or overwriting existing templates.
