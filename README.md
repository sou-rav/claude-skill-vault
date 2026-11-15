
# Claude Skill Vault

A curated vault of Claude Code plugins, agent skills, MCP servers, CLI tools, development frameworks, and workflow repositories. Each entry includes its purpose, type, and installation method where available.

## Index

1. [Coding & Senior Dev Workflows](#1-coding--senior-dev-workflows)
2. [Research & Codebase Understanding](#2-research--codebase-understanding)
3. [Large Projects, Memory & Token Management](#3-large-projects-memory--token-management)
4. [Design & Visuals](#4-design--visuals)
5. [Writing, Productivity & Video](#5-writing-productivity--video)
6. [Frontend & UI Development](#6-frontend--ui-development)
7. [Browser Automation & Testing](#7-browser-automation--testing)
8. [Code Quality & Security](#8-code-quality--security)
9. [Deployment & Preview](#9-deployment--preview)
10. [Additional Resources](#additional-resources)
11. [Official Documentation](#official-documentation)
12. [Installation & Security Notes](#installation--security-notes)

---

## 1. Coding & Senior Dev Workflows

### [Superpowers](https://github.com/obra/superpowers)

Agentic skills framework and software development methodology with brainstorming, planning, TDD, debugging, and code review workflows.

- Type: Claude Code plugin / agent skills
- Installation:

```text
/plugin install superpowers@claude-plugins-official
```

- Alternative marketplace:

```text
/plugin marketplace add obra/superpowers-marketplace
/plugin install superpowers@superpowers-marketplace
```

### [Matt Pocock Skills](https://github.com/mattpocock/skills)

Engineering and workflow skills from Matt Pocock's `.agents` setup.

- Type: Claude Code plugin / agent skills
- Installation:

```text
/plugin install mattpocock-skills
```

- Alternative:

```bash
npx skills@latest add mattpocock/skills
```

- Run `/setup-matt-pocock-skills` after installation.

### [ECC (Everything Claude Code)](https://github.com/affaan-m/everything-claude-code)

Agent harness optimization system with skills, memory, security, hooks, and research-first development workflows.

- Type: Claude Code plugin / agent framework
- Installation:

```text
/plugin marketplace add affaan-m/everything-claude-code
/plugin install everything-claude-code@everything-claude-code
```

- npm package: `ecc-universal`
- Repository: https://github.com/affaan-m/everything-claude-code

### [Karpathy Skills](https://github.com/forrestchang/andrej-karpathy-skills)

Coding guidelines derived from Andrej Karpathy's observations on LLM coding pitfalls. Focuses on simplicity, planning, and avoiding unnecessary changes.

- Type: Claude Code plugin / project instructions
- Plugin installation:

```text
/plugin marketplace add forrestchang/andrej-karpathy-skills
/plugin install andrej-karpathy-skills@karpathy-skills
```

- Alternative project-level installation: Download the `CLAUDE.md` file and place it in your project root.
- Global setup: Merge the rules into `~/.claude/CLAUDE.md`.

### [Ponytail](https://github.com/DietrichGebert/ponytail)

Makes AI agents think like a practical senior developer. Focuses on YAGNI, standard-library-first development, and simpler implementations.

- Type: Claude Code plugin / agent skills
- Plugin installation:

```text
/plugin marketplace add DietrichGebert/ponytail
/plugin install ponytail@ponytail
```

- Skills CLI alternative:

```bash
npx skills add DietrichGebert/ponytail
```

### [Agent Skills](https://github.com/wshobson/agents)

Production-grade engineering skills, agents, and commands for AI coding tools.

- Type: Agent skills / agents / commands
- Installation: Follow the repository README to select and install the required skills.
- Additional collection: [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)

### [Jeffallan Claude Skills](https://github.com/Jeffallan/claude-skills)

Collection of specialized full-stack development skills covering frontend, backend, frameworks, testing, infrastructure, and security.

- Type: Claude Code plugin / agent skills
- Marketplace installation:

```text
/plugin marketplace add jeffallan/claude-skills
/plugin install fullstack-dev-skills@fullstack-dev-skills
```

- Skills CLI alternative:

```bash
npx skills add jeffallan/claude-skills
```

---

## 2. Research & Codebase Understanding

### [Graphify](https://github.com/safishamsi/graphify)

Turns a codebase or folder into a queryable knowledge graph.

- Type: Codebase analysis / knowledge graph
- Installation: Follow the repository README for the current package and installation procedure.
- No verified universal installation command included.

### [Agent Reach](https://github.com/Panniantong/Agent-Reach)

CLI and agent skill for searching and reading X, Reddit, YouTube, GitHub, and other platforms.

- Type: Python CLI / agent skill
- Prerequisite: `uv`
- Installation:

```bash
uv tool install https://github.com/Panniantong/Agent-Reach/releases/latest/download/agent-reach.zip
agent-reach setup
```

- Update:

```bash
agent-reach update
```

### [Understand Anything](https://github.com/lum1104/Understand-Anything)

Turns a codebase into an interactive, searchable knowledge graph.

- Type: Codebase visualization / agent tool
- Installation: Follow the repository README and setup instructions.
- No verified universal package command included.

### [Last 30 Days](https://github.com/mvanhorn/last30days-skill)

Researches topics across Reddit, X, YouTube, Hacker News, and Polymarket and synthesizes recent findings.

- Type: Claude Code plugin / research skill
- Installation:

```text
/plugin marketplace add mvanhorn/last30days-skill
```

- Skills CLI alternative:

```bash
npx skills add mvanhorn/last30days-skill -g
```

### [CareerOps](https://github.com/career-ops-hq/career-ops)

Open-source AI job search agent that scans job boards, scores roles against a CV, and tailors resumes.

- Type: Standalone AI application
- Installation:

```bash
git clone https://github.com/career-ops-hq/career-ops.git
cd career-ops
```

- Follow the repository instructions to create the Python environment and install dependencies.

### [REA](https://github.com/morluto/rea)

Reverse-engineering agent framework for inspecting native binaries, Electron apps, and websites.

- Type: Node.js CLI / MCP integrations
- Prerequisite: Supported Node.js version
- Installation:

```bash
npx rea-agents@latest setup
```

- Optional global installation:

```bash
npm install --global rea-agents
rea setup
```

- Skill-only installation:

```bash
npx skills add morluto/rea --skill reverse-engineer-anything
```

- Note: Skill-only installation does not configure the REA MCP server or analysis engines.

### [Context7](https://github.com/upstash/context7)

Provides AI coding agents with up-to-date, version-specific documentation for frameworks, libraries, and APIs.

- Type: MCP server
- Installation: Follow the official Context7 MCP setup guide.
- Documentation: https://context7.com/docs
- Configure the current endpoint and authentication requirements from the official documentation.

### [Skill Seekers](https://github.com/yusufkaraaslan/Skill_Seekers)

Converts documentation websites, GitHub repositories, and PDFs into structured AI skills.

- Type: Python CLI / skill generator / optional MCP server
- Prerequisite: Python 3.10+
- Core installation:

```bash
pip install skill-seekers
```

- Full installation:

```bash
pip install "skill-seekers[all-llms]"
```

- MCP support:

```bash
pip install "skill-seekers[mcp]"
```

- Verify:

```bash
skill-seekers --version
```

---

## 3. Large Projects, Memory & Token Management

### [GStack](https://github.com/garrytan/gstack)

Garry Tan's opinionated development setup with defined roles such as CEO, designer, QA, and engineer.

- Type: Claude Code skills / agent workflow
- Prerequisites: Claude Code, Git, Bun, and Node.js on Windows
- Installation:

```bash
git clone --single-branch --depth 1 https://github.com/garrytan/gstack.git ~/.claude/skills/gstack
cd ~/.claude/skills/gstack
./setup
```

- Check installation:

```bash
./setup --status
```

- Windows users should follow the repository's Windows-specific setup instructions.

### [Caveman](https://github.com/JuliusBrussee/caveman)

Reduces unnecessary agent output through concise communication rules and workflow integrations.

- Type: Agent installer / skills / optional CLI
- Prerequisite: Node.js 18+ for the skill installer
- Installation:

```bash
npx -y github:JuliusBrussee/caveman
```

- Windows PowerShell alternative:

```powershell
irm https://raw.githubusercontent.com/JuliusBrussee/caveman/v4.1.0/install.ps1 | iex
```

- Optional CLI:

```bash
npm install -g @caveman-ai/cli@latest
```

### [Claude-Mem](https://github.com/thedotmack/claude-mem)

Persistent memory across sessions that compresses session history and injects relevant context into later sessions.

- Type: Claude Code plugin / memory system
- Installation:

```bash
npx claude-mem install
```

- Claude Code marketplace alternative:

```text
/plugin marketplace add thedotmack/claude-mem
/plugin install claude-mem
```

- Note: Installing the SDK or library alone does not configure the plugin runtime and hooks.

### [Headroom](https://github.com/headroomlabs-ai/headroom)

Context compression layer that reduces tool outputs, logs, and files to save tokens.

- Type: Python / TypeScript CLI and compression framework
- Python CLI installation:

```bash
uv tool install --python 3.13 "headroom-ai[all]"
```

- Python project installation:

```bash
pip install "headroom-ai[all]"
```

- TypeScript installation:

```bash
npm install headroom-ai
```

- Verify:

```bash
headroom --version
```

### [GSD (Get Shit Done)](https://github.com/gsd-build/get-shit-done)

Context engineering, spec-driven development, and structured project execution system.

- Type: Development workflow / agent framework
- Installation:

```bash
npm install -g get-shit-done-cc@latest
```

- One-time execution:

```bash
npx get-shit-done-cc@latest
```

### [BMAD Method](https://github.com/bmad-code-org/BMAD-METHOD)

Breakthrough Method for Agile AI-Driven Development. Provides structured planning and multi-agent execution workflows.

- Type: Development methodology / agent framework
- Installation:

```bash
npx bmad-method install
```

- Prerequisites for the stable release: Node.js 20.12+, Python 3.10+, and uv.
- Check the repository documentation before installing preview or alpha releases.

---

## 4. Design & Visuals

### [UI UX Pro Max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)

Design intelligence skill with design systems, palettes, typography rules, UX guidelines, and framework support.

- Type: Claude Code plugin / design skill
- Installation:

```text
/plugin marketplace add nextlevelbuilder/ui-ux-pro-max-skill
/plugin install ui-ux-pro-max@ui-ux-pro-max-skill
```

- Setup guide: https://github.com/nextlevelbuilder/ui-ux-pro-max-skill/blob/main/stack/docs/SETUP.md

### [Taste Skill](https://github.com/Leonxlnx/taste-skill)

Gives coding agents art direction and layout systems to avoid generic AI-generated interfaces.

- Type: Design skill
- Installation:

```bash
npx skills add https://github.com/Leonxlnx/taste-skill
```

- Specific skill installation:

```bash
npx skills add https://github.com/Leonxlnx/taste-skill --skill design-taste-frontend
```

### [Awesome Design Skills](https://github.com/jdsadminllc/awesome-design-skills)

Curated collection of design skills covering visual styles, typography, layouts, components, and design guidelines.

- Type: Reference collection
- Installation: No standalone installer. Browse the collection and install individual projects using their own instructions.

### [Anthropic Frontend Design](https://github.com/anthropics/claude-code/tree/main/plugins/frontend-design)

Official Claude Code frontend design plugin for distinctive interfaces, deliberate visual direction, typography, colors, and polished implementation.

- Type: Official Claude Code plugin
- Installation: Use the official Claude Code plugin browser.
- Documentation: https://code.claude.com/docs/en/plugins
- The GitHub source folder is not a standalone npm package.

### [Frontend Design Pro](https://github.com/claudekit/frontend-design-pro-demo)

Collection of 11 frontend design aesthetics with master prompts, signature effects, and implementation examples.

- Type: Claude Code plugin / design skill
- Installation: Follow the repository's plugin and marketplace setup instructions.
- No universal installation command included.

### [Bencium Design Skills](https://github.com/bencium/bencium-marketplace)

Collection of UX design, visual design, typography, and design-audit skills for production interfaces.

- Type: Claude Code marketplace / agent skills
- Marketplace installation:

```text
/plugin marketplace add bencium/bencium-marketplace
```

- Browse the marketplace and install the required plugin.
- Skills CLI discovery:

```bash
npx skills add bencium/bencium-marketplace --list
```

### [Archify](https://github.com/tt-a1i/archify)

Turns ideas, plans, or codebases into interactive HTML/SVG architecture diagrams.

- Type: Agent skill / diagram generator
- Installation:

```bash
npx skills add tt-a1i/archify -g
```

### [Impeccable](https://github.com/pbakaus/impeccable)

Design vocabulary and critique/audit skill to catch generic AI-generated interface patterns before shipping.

- Type: Design skill / installer / hooks
- Installation:

```bash
npx impeccable install
```

- Update:

```bash
npx impeccable update
```

- Marketplace setup:

```text
/plugin marketplace add pbakaus/impeccable
```

### [img2threejs](https://github.com/img2threejs/img2threejs)

Reconstructs 3D objects from reference images using procedural Three.js code.

- Type: Agent skill / 3D reconstruction tool
- Prerequisites: Node.js 18+, Git, Python 3.10+
- Installation:

```bash
npx --yes img2threejs@latest install
```

- Check installation:

```bash
npx --yes img2threejs@latest doctor
```

### [PPT Master](https://github.com/hugohe3/ppt-master)

Generates editable PowerPoint decks with charts, shapes, and speaker notes from documents.

- Type: Agent skill / PowerPoint generation tool
- Prerequisite: Python 3.10+
- Skill installation:

```bash
npx skills add hugohe3/ppt-master
```

- Install Python dependencies from the repository directory:

```bash
python -m pip install -r requirements.txt
```

- Getting started: https://github.com/hugohe3/ppt-master/blob/main/docs/getting-started.md

### [Diagram Design](https://github.com/cathrynlavery/diagram-design)

Generates 45+ types of editorial HTML and SVG diagrams.

- Type: Diagram generation skill
- Installation: Follow the repository's current README and skill installation instructions.
- No verified package command included.

---

## 5. Writing, Productivity & Video

### [Skills by Anthropic](https://github.com/anthropics/skills)

Anthropic's official reference collection and Agent Skills examples.

- Type: Official agent skills / reference collection
- Installation:

```bash
npx skills add anthropics/skills
```

- Agent Skills specification: https://agentskills.io/

### [Open Montage](https://github.com/OpenMontageInc/OpenMontage)

Open-source agentic video production and montage pipeline.

- Type: Video production framework / agent skills
- Installation:

```bash
git clone https://github.com/OpenMontageInc/OpenMontage.git
cd OpenMontage
```

- Follow the repository instructions for environment setup and dependencies.

### [Hyperframes](https://github.com/heygen-com/hyperframes)

Video rendering framework that lets agents write HTML and GSAP animations and render them to MP4.

- Type: Video rendering framework / Claude Code plugin
- Installation: Follow the repository's current Claude Code plugin instructions.
- Skills CLI alternative:

```bash
npx skills add heygen-com/hyperframes
```

### [Humanizer](https://github.com/blader/humanizer)

Removes common AI writing patterns based on Wikipedia's guide to signs of AI writing.

- Type: Agent skill / Claude Code plugin
- Skills CLI installation:

```bash
npx skills add blader/humanizer
```

- Marketplace installation: Follow the repository's plugin setup instructions.

### [I Have ADHD](https://github.com/ayghri/i-have-adhd)

Formats agent responses to lead with the immediate next action, numbered steps, and minimal unnecessary text.

- Type: Agent skill
- Installation:

```bash
npx skills add ayghri/i-have-adhd
```

- Check the repository's installation guide for platform-specific setup.

### [Marketing Skills](https://github.com/coreyhaines31/marketingskills)

Collection of skills for CRO, copywriting, SEO, analytics, and growth engineering.

- Type: Marketing skills / Claude Code plugin
- Skills CLI installation:

```bash
npx skills add coreyhaines31/marketingskills
```

- Check the repository README for plugin-specific installation and configuration.

---

## 6. Frontend & UI Development

### [Framer Motion (Motion)](https://github.com/motiondivision/motion)

Production-ready animation library for React, JavaScript, and Vue. Supports gestures, spring animations, scroll effects, and layout transitions.

- Type: Frontend library
- npm package: `motion`
- Installation:

```bash
npm install motion
```

- React import:

```javascript
import { motion } from "motion/react";
```

### [21st.dev Agent Skills](https://github.com/21st-dev/skill)

Helps AI coding agents discover, generate, install, and publish React and shadcn/ui components, themes, and templates.

- Type: Agent skills / CLI integration
- Skills installation:

```bash
npx skills add 21st-dev/skill
```

- CLI authentication:

```bash
npx @21st-dev/cli login
```

- Global skill installation:

```bash
npx @21st-dev/cli skills install --global
```

### [Animation Design Skills](https://github.com/freshtechbro/claudedesignskills)

Collection of specialized skills for GSAP, Three.js, React Spring, Framer Motion, Lottie, and interactive web animations.

- Type: Claude Code plugin marketplace / animation skills
- Marketplace setup:

```text
/plugin marketplace add freshtechbro/claudedesignskills
```

- Browse the marketplace and install the required animation plugin.

### [Design Motion Principles](https://github.com/kylezantos/design-motion-principles)

Builds and audits purposeful animations using professional motion design principles, accessibility, and performance guidelines.

- Type: Agent skill
- Installation:

```bash
npx skills add kylezantos/design-motion-principles
```

### [Three.js Skills](https://github.com/CloudAI-X/threejs-skills)

Specialized skills for building interactive 3D websites, scenes, animations, and Three.js experiences.

- Type: Three.js agent skills
- Installation: Follow the repository README for the current skill installation procedure.
- No verified package command included.

### [Figma MCP](https://developers.figma.com/docs/figma-mcp-server/)

Connects AI coding agents to Figma designs, components, variables, and design specifications.

- Type: MCP server
- Installation: Follow the official Figma MCP setup guide.
- Documentation: https://developers.figma.com/docs/figma-mcp-server/
- Authentication and access permissions may be required.

### [TypeScript LSP](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/typescript-lsp)

TypeScript and JavaScript language-server integration for code intelligence, diagnostics, go-to-definition, and reference lookup.

- Type: Claude Code plugin / language server
- Language server installation:

```bash
npm install -g typescript-language-server typescript
```

- Install the Claude Code plugin through the official plugin marketplace.
- Repository: https://github.com/anthropics/claude-plugins-official/tree/main/plugins/typescript-lsp

---

## 7. Browser Automation & Testing

### [Playwright CLI](https://github.com/microsoft/playwright-cli)

Browser automation CLI designed for AI coding agents. Supports browser navigation, interaction, screenshots, and automated UI testing.

- Type: Browser automation CLI
- Installation:

```bash
npm install -g @playwright/cli@latest
```

- Documentation: https://playwright.dev/agent-cli/introduction

### [Playwright MCP](https://github.com/microsoft/playwright-mcp)

MCP server that lets AI agents control browsers, inspect pages, interact with elements, and run browser automation.

- Type: MCP server
- Installation:

```bash
claude mcp add playwright npx @playwright/mcp@latest
```

- Verify inside Claude Code:

```text
/mcp
```

### [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp)

Gives AI coding agents access to Chrome DevTools for browser debugging, network inspection, performance analysis, screenshots, and automation.

- Type: MCP server / Claude Code plugin
- MCP installation:

```bash
claude mcp add chrome-devtools --scope user npx chrome-devtools-mcp@latest
```

- Plugin installation:

```text
/plugin marketplace add ChromeDevTools/chrome-devtools-mcp
```

- Browse the marketplace and install the Chrome DevTools plugin.

### [Storybook](https://github.com/storybookjs/storybook)

Develop, document, and test UI components independently in an isolated environment.

- Type: Component development framework
- Installation inside a frontend project:

```bash
npx storybook@latest init
```

- Start:

```bash
npm run storybook
```

### [Storybook MCP](https://github.com/storybookjs/mcp)

Connects AI agents to Storybook component information, documentation, setup workflows, and component development tools.

- Type: MCP integration
- Installation: Follow the repository README for the compatible Storybook version and MCP configuration.
- No verified universal Claude Code command included.

### [axe-core](https://github.com/dequelabs/axe-core)

Automated accessibility testing engine that detects WCAG violations and accessibility issues in web applications.

- Type: Accessibility testing library
- npm package: `axe-core`
- Installation:

```bash
npm install --save-dev axe-core
```

- Playwright integration:

```bash
npm install --save-dev @axe-core/playwright
```

### [Lighthouse](https://github.com/GoogleChrome/lighthouse)

Automated website auditing tool for performance, accessibility, SEO, and web best practices.

- Type: CLI / website auditing tool
- Installation:

```bash
npm install -g lighthouse
```

- Run an audit:

```bash
lighthouse https://example.com
```

### [Web Quality Skills](https://github.com/addyosmani/web-quality-skills)

Collection of AI agent skills for website performance, Core Web Vitals, accessibility, SEO, and web quality audits.

- Type: Web quality / agent skills
- Installation: Follow the repository README and select the appropriate skill installation method.
- No verified universal install command included.

---

## 8. Code Quality & Security

### [Cloudflare Security Audit](https://github.com/cloudflare/security-audit-skill)

Security auditing skill that reviews codebases, identifies vulnerabilities, validates findings, and generates structured security reports.

- Type: Security audit skill
- Installation: Follow the repository's official installation instructions.
- No verified package name or universal install command included.

### [OWASP ASVS](https://github.com/OWASP/ASVS)

Application Security Verification Standard. Provides security requirements for designing, developing, and testing web applications and services.

- Type: Security standard / reference
- No software installation required.
- Stable release: ASVS 5.0.0
- Downloads: https://asvs.owasp.org/downloads/
- Clone source:

```bash
git clone https://github.com/OWASP/ASVS.git
```

---

## 9. Deployment & Preview

### [PinMe](https://github.com/glitternetwork/pinme)

One-command deployment CLI for frontend and full-stack projects, with Claude Code skill support.

- Type: Deployment CLI / agent skill
- Installation: Follow the repository README for the official package name and setup procedure.
- No verified package command included.

### [Vercel](https://github.com/vercel/vercel)

Deployment platform and CLI for publishing frontend projects, managing preview deployments, and connecting projects to production environments.

- Type: Deployment CLI / platform
- npm package: `vercel`
- Installation:

```bash
npm install -g vercel
```

- Login:

```bash
vercel login
```

- Deploy:

```bash
vercel
```

---

## Additional Resources

### [Awesome Claude Skills](https://github.com/ComposioHQ/awesome-claude-skills)

Large curated directory of Claude skills, plugins, MCP integrations, and workflow resources, including D3.js visualization skills.

- Type: Reference collection
- No standalone installer.
- Browse individual projects and install them using their respective instructions.

---

## Official Documentation

- [Claude Code Documentation](https://code.claude.com/docs/en/overview)
- [Claude Code Skills](https://code.claude.com/docs/en/skills)
- [Claude Code Plugins](https://code.claude.com/docs/en/plugins)
- [Claude Code MCP](https://code.claude.com/docs/en/mcp)
- [Agent Skills Specification](https://agentskills.io/)
- [Skills CLI](https://github.com/vercel-labs/skills)
- [Model Context Protocol](https://modelcontextprotocol.io/)

## Installation & Security Notes

- Read the repository README before installing.
- Check whether a repository contains a `SKILL.md`, `.claude-plugin/plugin.json`, or `.claude-plugin/marketplace.json`.
- Do not assume every GitHub repository is a Claude Code plugin.
- Do not assume a CLI package and an MCP server use the same package name.
- MCP servers may require API keys, authentication, and additional dependencies.
- Install frontend libraries inside the relevant project.
- Use project-level skills when a workflow should apply only to one project.
- Use global skills when a workflow should be available across projects.
- Review shell scripts before executing them.
- Avoid running unknown scripts with administrator privileges.
- Verify MCP connections with `/mcp`.
- Restart Claude Code when an installation requires it.
- Check compatibility with your installed Claude Code version.
