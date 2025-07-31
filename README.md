# Claude Sub-Agents Collection 🤖

**64 specialized AI agents** for Claude Code that work together as an intelligent development team.

> **📖 Official Docs**: [How Sub-agents Work](https://docs.anthropic.com/en/docs/claude-code/sub-agents) | **🚀 Quick Start**: Copy `agents/` to `~/.claude/agents/`

---

## 🎯 Agent Categories

| Category | Count | Description | Key Agents |
|----------|-------|-------------|------------|
| 🎭 [**Orchestrators**](agents/orchestrators/) | 9 | Project coordination & management | [tech-lead-orchestrator](agents/orchestrators/tech-lead-orchestrator.md), [project-analyst](agents/orchestrators/project-analyst.md) |
| 🏗️ [**Infrastructure**](agents/infrastructure/) | 5 | Cloud, DevOps & deployment | [cloud-architect](agents/infrastructure/cloud-architect.md), [devops-troubleshooter](agents/infrastructure/devops-troubleshooter.md) |
| 💻 [**Language Experts**](agents/language-experts/) | 6 | Programming language specialists | [python-pro](agents/language-experts/python-pro.md), [javascript-pro](agents/language-experts/javascript-pro.md), [rust-pro](agents/language-experts/rust-pro.md) |
| 🌐 [**Universal**](agents/universal/) | 4 | Framework-agnostic development | [api-architect](agents/universal/api-architect.md), [frontend-developer](agents/universal/frontend-developer.md) |
| ⚡ [**Specialized**](agents/specialized/) | 19 | Framework-specific experts | [Django](agents/specialized/django/) (3), [React](agents/specialized/react/) (2), [Vue](agents/specialized/vue/) (3), [Rails](agents/specialized/rails/) (3), [Laravel](agents/specialized/laravel/) (2) + 6 others |
| 🛡️ [**Quality & Security**](agents/quality-security/) | 6 | Code quality & security | [security-auditor](agents/quality-security/security-auditor.md), [test-automator](agents/quality-security/test-automator.md) |
| 🎯 [**Core**](agents/core/) | 4 | Cross-cutting utilities | [code-reviewer](agents/core/code-reviewer.md), [performance-optimizer](agents/core/performance-optimizer.md) |
| 🧠 [**Data & ML**](agents/data-ml/) | 5 | AI/ML & data engineering | [ai-engineer](agents/data-ml/ai-engineer.md), [data-scientist](agents/data-ml/data-scientist.md) |
| 💼 [**Business**](agents/business/) | 6 | Business & content | [business-analyst](agents/business/business-analyst.md), [content-writer](agents/business/content-writer.md) |

---

## 🚀 Framework Support

| Framework | Agents | Status |
|-----------|---------|---------|
| **Django** | 3 agents | ✅ [Full ecosystem](agents/specialized/django/) |
| **React/Next.js** | 2 agents | ✅ [Component + SSR](agents/specialized/react/) |
| **Vue/Nuxt** | 3 agents | ✅ [Full ecosystem](agents/specialized/vue/) |
| **Rails** | 3 agents | ✅ [Full ecosystem](agents/specialized/rails/) |
| **Laravel** | 2 agents | ✅ [Backend + ORM](agents/specialized/laravel/) |

---

## 📋 Quick Reference

### Most Popular Agents
| Agent | Purpose | Use When |
|-------|---------|----------|
| [tech-lead-orchestrator](agents/orchestrators/tech-lead-orchestrator.md) | Complex project coordination | Multi-step tasks requiring multiple specialists |
| [python-pro](agents/language-experts/python-pro.md) | Advanced Python development | Python projects with async, decorators, performance needs |
| [security-auditor](agents/quality-security/security-auditor.md) | Security assessment | Code reviews, vulnerability scans, compliance |
| [api-architect](agents/universal/api-architect.md) | API design & integration | RESTful/GraphQL APIs, data contracts |
| [vue-component-architect](agents/specialized/vue/vue-component-architect.md) | Vue 3 development | Vue projects with Composition API, component design |
| [laravel-backend-expert](agents/specialized/laravel/laravel-backend-expert.md) | Laravel development | PHP/Laravel applications, backend features |

### By Use Case
| **Building APIs** | **Frontend Work** | **DevOps/Deploy** | **Code Quality** |
|-------------------|-------------------|-------------------|------------------|
| [api-architect](agents/universal/api-architect.md) | [frontend-developer](agents/universal/frontend-developer.md) | [cloud-architect](agents/infrastructure/cloud-architect.md) | [code-reviewer](agents/core/code-reviewer.md) |
| [django-api-developer](agents/specialized/django/django-api-developer.md) | [react-component-architect](agents/specialized/react/react-component-architect.md) | [deployment-engineer](agents/infrastructure/deployment-engineer.md) | [security-auditor](agents/quality-security/security-auditor.md) |
| [rails-api-developer](agents/specialized/rails/rails-api-developer.md) | [vue-component-architect](agents/specialized/vue/vue-component-architect.md) | [devops-troubleshooter](agents/infrastructure/devops-troubleshooter.md) | [test-automator](agents/quality-security/test-automator.md) |
| [laravel-backend-expert](agents/specialized/laravel/laravel-backend-expert.md) | - | - | - |

## 🔧 Installation

```bash
# Clone and install
git clone https://github.com/bhatyogesh/claude-subagents.git
cp -r claude-subagents/agents ~/.claude/

# Verify installation
# Open Claude Code - agents auto-activate based on your requests
```

**That's it!** No configuration needed. Agents automatically activate when Claude detects relevant tasks.

---

## 💡 How It Works

1. **Smart Detection**: Claude automatically routes tasks to the right specialists
2. **Team Coordination**: [tech-lead-orchestrator](agents/orchestrators/tech-lead-orchestrator.md) manages complex multi-step projects  
3. **Quality Gates**: Built-in validation ensures production-ready results

### Example Workflows

| Your Request | What Happens |
|--------------|--------------|
| *"Build a Django API"* | `project-analyst` → `django-backend-expert` → `django-api-developer` → `security-auditor` |
| *"Create a Vue dashboard"* | `vue-component-architect` → `vue-state-manager` → `performance-optimizer` |
| *"Rails e-commerce site"* | `rails-backend-expert` → `rails-api-developer` → `rails-activerecord-expert` |
| *"Laravel admin panel"* | `laravel-backend-expert` → `laravel-eloquent-expert` → `security-auditor` |
| *"Review code security"* | `code-reviewer` → `security-auditor` → recommendations |

---

## 🤝 Contributing

**Want to add agents?** Create new `.md` files in `agents/` following the existing patterns. See [official sub-agents docs](https://docs.anthropic.com/en/docs/claude-code/sub-agents) for details.

**Missing frameworks?** We'd love Angular, Svelte, Phoenix experts! Check `agents/specialized/` for examples.

---

## 📄 License & Links

**MIT License** | [Repository](https://github.com/bhatyogesh/claude-subagents) | [Issues](https://github.com/bhatyogesh/claude-subagents/issues) | [Claude Code](https://claude.ai/code)