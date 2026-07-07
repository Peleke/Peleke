# Profile Sync Notes (2026-07-07)

Synced this profile README to the live portfolio at [peleke.me](https://peleke.me). Source of truth: the `portfolio` repo (Astro site), pages `index.astro`, `about.astro`, `lab.astro`, `cv.astro`, `projects/index.astro`, and the `src/content/writing` collection.

## What the portfolio positioning is now

- **Homepage headline:** "Agent infrastructure that learns safely." Sub: agents that learn from usage can just as easily learn the wrong things; I build the infrastructure that keeps that from happening.
- **About one-liner:** "Secure learning architectures for AI agent systems." Focus tags: agent security, adaptive retrieval, exploit research, observability, Old Norse.
- **CV one-liner:** "I build agent systems that learn from production usage and the observability to prove they're working and improving over time."
- **Research framing (Lab / qlawbox):** "A Measurement Thesis." Central question: can agents learn to optimize their own context? Context engineering treated as a reinforcement-learning problem, instrumented so learning can be measured (RMR, tokens per task, arm convergence).

The dominant frame is now **agent infrastructure + security + measurable learning + observability.** The old "I study how languages work and build tools from what I find" language-first framing is demoted; Old Norse / linguistics is now a personal-interest tag, and Interlinear is one product among several.

## What I changed and why

1. **Headline.** Replaced "I study how languages work and build tools from what I find" with the portfolio's security-learning positioning. The old line no longer matches the site.
2. **Research question.** Old README asked "Can agents learn from their own performance?" The live lab asks "Can agents learn to optimize their own context?" Reworded to match, kept the "remembering, not adapting" distinction (it survives verbatim on the site).
3. **The stack table (biggest fix).** The old table was stale:
   - Layer 02 listed **buildlog / openclaw** as "Learning." The live lab has no buildlog layer; it added a dedicated **Observability** layer (`qortex-observe`). Updated.
   - Runtime was listed as **openclaw + sandbox**. Both were renamed: **vindler** (hardened OpenClaw fork) + **bilrost** (the sandbox, now on PyPI). Updated names. The GitHub Pages URLs are unchanged (`/openclaw/`, `/openclaw-sandbox/`), so the links still resolve.
   - New five-layer order per the lab: 01 Knowledge+Learning (qortex), 02 Observability (qortex-observe), 03 Runtime (vindler+bilrost), 04 Nervous System (cadence), 05 Interoception.
4. **Products.** Old README featured six (Interlinear, Swae OS, LinWheel, LangLine, ComfyUI MCP, Graphix). The portfolio's homepage and `/projects` now feature only three: **Interlinear, LinWheel, Swae OS.** Trimmed to those three to match, added case-study links (`peleke.me/projects/...`), and pointed to `github.com/peleke` for the rest. See open questions on the dropped three.
5. **Selected Writing (new section).** Added four flagship essays that ground the security + learning positioning, all verified to exist in `src/content/writing`. This was missing entirely from the old README.
6. **Background line.** Two corrections:
   - Old README said **"AI Systems Fellow @ Overclock."** No source uses that title. CV and the portfolio's own draft both say **SME** (subject-matter expert) for the agentic-engineering curriculum at Overclock Accelerator. Changed to "Agentic AI SME @ Overclock Accelerator."
   - Dropped **"Partner @ Endstation LLC"** (see open questions). Framed current work through the verified Principal Engineer / first-engineer / SME history plus AWS cert and Princeton.
7. **Links.** Added a Writing link. Switched the email to **peleke@pm.me** (the address the live index/about/cv all use; the old README used peleke@peleke.me).
8. **system-diagram.svg.** Refreshed two stale labels in place: the Learning layer's dead "buildlog / openclaw" sublabel became "accept / reject feedback", and the Runtime box "openclaw + sandbox" became "vindler + bilrost". No geometry changed. See open questions: the SVG still shows a 5-box layout without a dedicated Observability box; the canonical diagram at peleke.me/lab now breaks Observability out as its own layer.

## Open questions / needs your confirmation

- **Endstation title.** The old README said "Partner @ Endstation LLC"; your `portfolio/github-profile-readme.md` draft says "CTO at Endstation"; the live About page names no company, just "consulting on agent architecture and AI security." I left Endstation out of the background line to avoid asserting a title that the live site does not. Tell me which you want (Partner / CTO / Founder / omit) and I will add it back.
- **"Princeton" vs "Princeton CS."** The old README said "Princeton CS." Your CV lists only "Princeton University, 2012–2014" with no major. I used "Princeton" to avoid asserting a degree the CV does not state. Confirm the major if you want "CS" back.
- **Dropped projects (LangLine, ComfyUI MCP, Graphix).** These are real repos of yours but are not featured on the current portfolio homepage or `/projects`. I removed them from the README's Products section to match the site and left a general link to `github.com/peleke`. If you want any of them back as flagship items, say so (LangLine has a project page at `/projects/langline`; ComfyUI MCP and Graphix are GitHub-only).
- **system-diagram.svg full regen.** The in-repo SVG is a simplified 5-box copy. It now has no dead names, but it still does not show Observability as its own box the way peleke.me/lab does. If you want a 1:1 match, regenerate the SVG from the live lab diagram. The README embed and the lab are consistent enough for now; this is a polish item.
- **Overclock dates.** CV says Sep 2025–Jan 2026; the draft README said 2024–26. I left dates off the background line. Add them if you want.

## Repo state

The Peleke repo was clean and on `main` at the start. Work is on a new branch `profile-sync-2026-07-07`. Nothing pushed. No existing work was stashed or discarded.
