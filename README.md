# AI Awesome Skills

A curated list of tools to help you review, secure, and trust AI agent skills (Claude Code, MCP servers, and similar) before you install them.

## Security & Review

### [SkillSpector](https://github.com/NVIDIA/SkillSpector) by NVIDIA

Open source scanner that checks a Claude Code, Codex, or MCP skill for vulnerabilities before you install it. Runs static analysis (with an optional LLM semantic pass) across 71 attack patterns in 17 categories, including prompt injection, data exfiltration, privilege escalation, and supply chain risks. Returns a risk score from 0 to 100 in terminal, JSON, Markdown, or SARIF format.

NVIDIA's own research scanned 31,132 skills pulled from major marketplaces: 26.1% had at least one vulnerability, and 5.2% showed signs of likely malicious intent.

```bash
uv tool install git+https://github.com/NVIDIA/skillspector.git
skillspector scan ./path-to-skill --no-llm
```

License: Apache-2.0.

---

More tools get added here as I find and vet them. Suggestions are welcome via issues or PRs.
