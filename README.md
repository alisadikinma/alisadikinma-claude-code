# Ali Sadikin's Claude Code Plugin

My personal Claude Code configuration for productive web development. This plugin provides **14 slash commands** and **15 color-coded AI agents** to supercharge your development workflow.

## Quick Install

```bash
# Step 1: Add the marketplace
/plugin marketplace add alisadikinma/alisadikinma-claude-code

# Step 2: Install the plugin
/plugin install alisadikinma-claude-code
```

## What's Inside

### 📋 Development Commands (7)

| Command | Description |
|---------|-------------|
| `/new-task` | Analyze code for performance issues |
| `/code-explain` | Generate detailed explanations |
| `/code-optimize` | Performance optimization |
| `/code-cleanup` | Refactoring and cleanup |
| `/feature-plan` | Feature implementation planning |
| `/lint` | Linting and fixes |
| `/docs-generate` | Documentation generation |

### 🔌 API Commands (3)

| Command | Description |
|---------|-------------|
| `/api-new` | Create new API endpoints |
| `/api-test` | Test API endpoints |
| `/api-protect` | Add protection & validation |

### 🎨 UI Commands (2)

| Command | Description |
|---------|-------------|
| `/component-new` | Create React components |
| `/page-new` | Create Next.js pages |

### 💾 Supabase Commands (2)

| Command | Description |
|---------|-------------|
| `/types-gen` | Generate TypeScript types |
| `/edge-function-new` | Create Edge Functions |

---

### 🤖 Color-Coded AI Agents (15)

Each agent has a unique color for visual identification during execution.

#### Engineering (Blue/Indigo/Violet)

| Agent | Color | Description |
|-------|-------|-------------|
| `frontend-developer` | 🔵 `#3B82F6` | Build React/Vue/Angular components with TypeScript |
| `frontend-architect` | 🔵 `#60A5FA` | Frontend architecture, design systems, scalability |
| `backend-architect` | 🟣 `#6366F1` | API design, database architecture, security |
| `system-architect` | 🟣 `#8B5CF6` | System-wide architecture, component boundaries |

#### Design (Purple)

| Agent | Color | Description |
|-------|-------|-------------|
| `ui-designer` | 💜 `#A855F7` | Visual design, design systems, accessibility |

#### Quality (Pink/Amber/Orange/Yellow)

| Agent | Color | Description |
|-------|-------|-------------|
| `qa-expert` | 💗 `#EC4899` | **Mandatory Playwright browser testing**, CRUD verification |
| `code-reviewer` | 🟡 `#F59E0B` | Code quality, security vulnerabilities, best practices |
| `refactoring-expert` | 🟠 `#F97316` | Technical debt reduction, SOLID principles |
| `performance-engineer` | 🟡 `#EAB308` | Core Web Vitals, profiling, optimization |

#### Security (Red)

| Agent | Color | Description |
|-------|-------|-------------|
| `security-engineer` | 🔴 `#EF4444` | OWASP, threat modeling, compliance |

#### Research & Analysis (Cyan/Teal)

| Agent | Color | Description |
|-------|-------|-------------|
| `deep-research-agent` | 🔵 `#06B6D4` | Multi-hop research, evidence synthesis |
| `requirements-analyst` | 🟢 `#14B8A6` | PRD creation, stakeholder analysis |
| `tech-stack-researcher` | 🔵 `#22D3EE` | Technology evaluation, trade-off analysis |

#### Documentation & Education (Emerald/Green)

| Agent | Color | Description |
|-------|-------|-------------|
| `technical-writer` | 🟢 `#10B981` | API docs, user guides, READMEs |
| `learning-guide` | 🟢 `#22C55E` | Teaching concepts, tutorials, progressive learning |

---

### 🔧 MCP Servers (3)

| Server | Package | Purpose |
|--------|---------|---------|
| **Context7** | `@upstash/context7-mcp` | Up-to-date library documentation |
| **Playwright** | `@playwright/mcp` | Browser automation & testing |
| **Supabase** | `@supabase/mcp-server-supabase` | Database operations |

---

## Key Features

### 🎨 Color-Coded Agent Identification
Each agent has a unique color so you can visually identify which specialist is working on your task.

### ✅ Mandatory QA Verification
The `qa-expert` agent enforces **Playwright browser testing** for every task completion:
- CRUD operation verification
- Zero console errors requirement
- Screenshot evidence capture
- Formal QA sign-off

### 🔒 Security-First Code Review
The `code-reviewer` and `security-engineer` agents ensure:
- OWASP Top 10 compliance
- No critical vulnerabilities before merge
- CVSS severity classification

---

## Installation

### From GitHub

```bash
# Step 1: Add the marketplace
/plugin marketplace add alisadikinma/alisadikinma-claude-code

# Step 2: Install the plugin
/plugin install alisadikinma-claude-code
```

### From Local Clone (for development)

```bash
git clone https://github.com/alisadikinma/alisadikinma-claude-code.git
cd alisadikinma-claude-code

# Install from local path
/plugin install /path/to/alisadikinma-claude-code
```

---

## Usage Examples

### Planning a Feature

```bash
/feature-plan
# Then describe your feature idea
```

### Creating an API

```bash
/api-new
# Claude scaffolds complete API route with types, validation, error handling
```

### Research Tech Choices

Just ask Claude questions like:
- "Should I use WebSockets or SSE?"
- "How should I structure this database?"

The `tech-stack-researcher` agent automatically activates.

### QA Verification

After any development task, invoke:
```
@qa-expert verify this task
```

The agent will:
1. Launch Playwright browser
2. Test all CRUD operations
3. Check for console errors
4. Capture screenshots
5. Provide formal sign-off

---

## Philosophy

This setup emphasizes:
- **Type Safety**: Never uses `any` types
- **Visual Feedback**: Color-coded agents for identification
- **Quality Gates**: Mandatory QA verification
- **Security First**: OWASP compliance enforcement
- **Best Practices**: Modern Next.js/React patterns

---

## Requirements

- Claude Code 2.0.13+
- Works with any project (optimized for Next.js + Supabase)

---

## Customization

After installation, customize any command or agent by editing files in:
- `.claude/commands/` - Slash commands
- `.claude/agents/` - AI agents

---

## Contributing

Feel free to:
- Fork and customize for your needs
- Submit issues or suggestions
- Share your improvements

---

## License

MIT - Use freely in your projects

---

## Author

Created by **Ali Sadikin** ([@alisadikinma](https://github.com/alisadikinma))

---

**Note**: This is a hybrid plugin combining best practices from multiple sources, refined for productive modern web development workflows.
