# Peleke Sengstacke

Principal engineer & architect — cloud, AI, and the systems that ship them.

[peleke.me](https://peleke.me) · [Writing](https://peleke.me/writing) · [LinkedIn](https://linkedin.com/in/peleke) · [peleke.s@pm.me](mailto:peleke.s@pm.me)

All the work below was built with Claude's assistance.

### Agent security: Inside the Machine

I took OpenClaw apart, threat-modeled it, and found what I'd thought: A wide-open, utterly unprotected identity layer. Plain-text Markdown the agent loads verbatim into its system prompt is a considerable exposure, but remains a standard "feature" in many agentic harness configurations. [Inside the Machine](https://peleke.me/writing/inside-the-machine) is the four-article record. The same class of problem drew wider attention in October 2026, from [Forever Security](https://forever.security/blog/hijacking-ai-agents-via-downloads-folder/) and the [Cloud Security Alliance](https://labs.cloudsecurityalliance.org/research/csa-research-note-agent-instruction-file-poisoning-20261027/). You'll probably keep seeing it. 

- [Vindler](https://github.com/Peleke/openclaw): OpenClaw fork for experimenting with agent monitoring and learning
- [Bilrost](https://github.com/Peleke/openclaw-sandbox): Lima VM that isolates the agent (because properly hardening it is difficult).

### Skills, marketplaces, security

- [Skillipedia](https://github.com/Peleke/skillipedia): browsable index of agent skills ([live](https://skillipedia.vercel.app))
- [Brunnr](https://github.com/Peleke/brunnr): security scanner and skills marketplace for Claude Code, with a [worked bypass](https://github.com/Peleke/brunnr/tree/main/exploits/glassworm-bypass) showing where scanners fall short.

### Fiat Vox (book, in progress)

- [Fiat Vox](https://peleke.github.io/fiat-vox/): sound, phonetics, and DSP, working toward animal linguistics. Source: [Peleke/fiat-vox](https://github.com/Peleke/fiat-vox).
