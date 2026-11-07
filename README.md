# Peleke Sengstacke

Principal engineer & architect — cloud, AI, and the systems that ship them.

[peleke.me](https://peleke.me) · [Writing](https://peleke.me/writing) · [LinkedIn](https://linkedin.com/in/peleke) · [peleke.s@pm.me](mailto:peleke.s@pm.me)

### Agent security: Inside the Machine

I took OpenClaw apart, threat-modeled it, and found the identity layer wide open: plain-text Markdown the agent loads verbatim into its system prompt. [Inside the Machine](https://peleke.me/writing/inside-the-machine) is the four-article record. Forever Security later [published on a related class of problem](https://forever.security/blog/hijacking-ai-agents-via-downloads-folder).

- [Vindler](https://github.com/Peleke/openclaw): OpenClaw fork for experimenting with agent monitoring and learning
- [Bilrost](https://github.com/Peleke/openclaw-sandbox): Lima VM that isolates the agent, because properly hardening it is difficult

### Skills, marketplaces, security

- [Skillipedia](https://github.com/Peleke/skillipedia): browsable index of agent skills ([live](https://skillipedia.vercel.app))
- [Brunnr](https://github.com/Peleke/brunnr): security scanner and skills marketplace for Claude Code, with a [worked bypass](https://github.com/Peleke/brunnr/tree/main/exploits/glassworm-bypass) showing where scanners fall short
