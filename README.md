# S.T.A.R.S. Agent Team 🤖

> **S**pecialized **T**eam of **A**I **R**esource **S**upport agents for OpenClaw development

A hierarchical team of AI agents built on [OpenClaw](https://openclaw.com), each with specialized roles and capabilities. Inspired by the S.T.A.R.S. team from Resident Evil, these agents work together to handle everything from high-level architecture to implementation and infrastructure.

## 🌐 Live Team Page

**[View the Team →](https://kennysdevbot.github.io/agent-team/)**

## 🎯 Team Overview

This repository showcases a structured approach to multi-agent development using OpenClaw. Each agent has a specific role, model configuration, and set of responsibilities optimized for different types of work.

### The Team

| Agent | Role | Model | Specialty |
|-------|------|-------|-----------|
| **Leon Kennedy** | Principal Architect | Claude Opus 4.6 | Architecture, planning, system design |
| **Jill Valentine** | Senior Engineer | Claude Sonnet 4.5 | Feature development, full-stack implementation |
| **Chris Redfield** | DevOps Engineer | Claude Sonnet 4 | Infrastructure, deployment, automation |
| **Barry Burton** | Support Engineer | GPT-4o-mini | Quick fixes, scripts, documentation |

## 🏗️ Architecture

### Agent Hierarchy

```
Leon (Architect)
  ├─ Plans architecture & creates docs
  └─ Delegates to →
       ├─ Jill (Implementation)
       ├─ Chris (Infrastructure)
       └─ Barry (Support Tasks)
```

### Key Principles

1. **Separation of Concerns**: Each agent handles specific types of work
2. **Model Optimization**: More powerful (expensive) models for complex tasks, lighter models for routine work
3. **Documentation-First**: Architecture and patterns documented before implementation
4. **Clear Handoffs**: Explicit task routing between agents

## 🚀 Getting Started

### Prerequisites

- [OpenClaw](https://openclaw.com) installed and configured
- Node.js 18+ (for the team page)
- Git access to your repositories

### Agent Setup

Each agent requires:

1. **SOUL.md** - Defines personality and communication style
2. **Agent Profile** - Configuration file (e.g., `leon-kennedy.md`)
3. **Workspace** - Separate workspace per agent to avoid context collision

### Basic Usage

```bash
# Start a new project with Leon
openclaw agent leon "Create a new Next.js project for [project-name]"

# Implement a feature with Jill
openclaw agent jill "Add user authentication to the dashboard"

# Deploy with Chris
openclaw agent chris "Set up CI/CD pipeline for production"

# Quick documentation fix with Barry
openclaw agent barry "Update the README with new installation steps"
```

## 📋 Agent Responsibilities

### Leon Kennedy - Principal Architect

**When to use Leon:**
- Starting a new project
- Major architectural decisions
- System design and refactoring
- Creating foundational documentation

**What Leon creates:**
- `README.md`
- `docs/architecture/*.md` (product brief, tech stack, system design, patterns)
- High-level implementation plans

**Leon does NOT:**
- Jump into implementation before planning
- Write code without documenting patterns first
- Handle quick fixes or minor updates

### Jill Valentine - Senior Engineer

**When to use Jill:**
- Full-stack feature development
- Complex bug fixes
- Code reviews and refactoring
- Integration work

**What Jill handles:**
- Multi-file features
- Database migrations
- API development
- Frontend components
- Testing implementation

**Jill does NOT:**
- Start work without reading architecture docs
- Make architectural decisions (escalates to Leon)
- Handle infrastructure (delegates to Chris)

### Chris Redfield - DevOps Engineer

**When to use Chris:**
- Deployment and CI/CD
- Infrastructure setup
- Environment configuration
- Monitoring and logging
- Performance optimization

**What Chris manages:**
- Docker/Kubernetes configs
- GitHub Actions workflows
- Cloud infrastructure
- Database backups
- Security hardening

**Chris does NOT:**
- Implement business features (delegates to Jill)
- Make database schema decisions (collaborates with Leon)

### Barry Burton - Support Engineer

**When to use Barry:**
- Quick fixes and scripts
- Documentation updates
- Simple refactoring
- Routine maintenance
- Utility scripts

**What Barry does:**
- README updates
- Simple bug fixes
- Script creation
- Code cleanup
- Comment additions

**Barry does NOT:**
- Handle complex features (escalates to Jill)
- Make architectural changes (escalates to Leon)

## 🔄 Workflow Example

### New Project Creation

1. **Leon** creates architecture docs and project structure
   ```bash
   openclaw agent leon "Create a new task management SaaS app"
   ```
   - Outputs: README, architecture docs, tech stack decisions

2. **Jill** implements core features
   ```bash
   openclaw agent jill "Implement user authentication and task CRUD"
   ```
   - Reads Leon's docs first
   - Implements following documented patterns

3. **Chris** sets up deployment
   ```bash
   openclaw agent chris "Set up Vercel deployment and database hosting"
   ```
   - Configures CI/CD
   - Sets up environments

4. **Barry** adds finishing touches
   ```bash
   openclaw agent barry "Add JSDoc comments to utility functions"
   ```
   - Documentation polish
   - Minor improvements

## 🛠️ Configuration

### Agent Profile Structure

Each agent has a profile file (e.g., `leon-kennedy.md`) with:

```markdown
# Agent: [Name]

## Role
[Primary responsibility]

## Default Model
[Model name]

## Purpose
[Detailed description]

## Core Responsibilities
- [List of key tasks]

## Task Types
- [Specific work types]

## Rules
- [Constraints and guidelines]

## Handoff Rules
- [When to delegate to other agents]
```

### Customizing the Team

1. **Clone this repository** to see example profiles
2. **Modify agent profiles** to fit your workflow
3. **Adjust model assignments** based on your budget and needs
4. **Add new agents** for specialized domains (mobile, ML, design, etc.)

## 📊 Cost Optimization

The hierarchical model reduces costs by:

- Using Claude Opus 4.6 (most expensive) only for architecture
- Using Claude Sonnet 4.5 for complex implementation
- Using Claude Sonnet 4 for infrastructure tasks
- Using GPT-4o-mini for routine work

**Estimated savings:** 60-70% compared to using top-tier models for all tasks.

## 🎨 Team Page

The included `index.html` provides a visual overview of your agent team:

- **Responsive design** works on all devices
- **Agent cards** with role, model, and specialties
- **Visual hierarchy** showing agent relationships
- **Click to expand** for detailed information

### Deploying the Team Page

```bash
# GitHub Pages (easiest)
# Just enable Pages in repo settings, pointing to main branch

# Or serve locally
cd agent-team
npx http-server
```

## 🤝 Contributing

This is a template and reference implementation. To adapt it:

1. Fork this repository
2. Customize agent profiles for your needs
3. Update the team page with your agents
4. Share your setup!

## 📚 Resources

- [OpenClaw Documentation](https://openclaw.com/docs)
- [Agent Skills](https://clawhub.com)
- [OpenClaw Discord](https://discord.gg/openclaw)

## 📄 License

MIT License - Feel free to use this as a template for your own agent teams.

---

**Built with [OpenClaw](https://openclaw.com)** 🐾
