# AI Workflow & Prompt Library 🤖

A curated collection of specialized Claude subagents and production-ready prompts for AI-powered workflows across development, content creation, security, and product management.

## What This Repository Is

This is a **living knowledge base** that transforms how you work with Claude Code and other AI systems. Instead of starting from scratch each time, you get:

- **20+ Specialized Subagents** that act as domain experts
- **Battle-tested Prompts** for complex workflows
- **CLAUDE.md Integration** for seamless AI assistance in your projects
- **Production-ready Templates** you can immediately use

Think of it as your AI workforce - each subagent is a specialist that knows exactly how to help with specific tasks, from code reviews that prevent outages to SEO content that ranks.

## Repository Structure

```
ai/
├── claude subagents/           # 20+ specialized AI agents
│   ├── code-reviewer.md       # Security-focused code review
│   ├── prompt-engineer.md     # LLM optimization expert
│   ├── backend-architect.md   # API & system design
│   ├── security-auditor.md    # OWASP compliance
│   └── seo-*.md              # Complete SEO workflow
├── prompt library/            # Production prompts & templates
│   ├── PM Copilot.md         # Product management coaching
│   └── System Prompt - *.md  # Specialized system prompts
├── CLAUDE.md                  # Repository guidance for Claude Code
└── README.md                  # This file
```

## 🎯 Understanding CLAUDE.md Files

`CLAUDE.md` files are **game-changers** for AI-assisted development. They're instruction files that tell Claude Code exactly how to work with your specific codebase.

### Why CLAUDE.md Matters

Without CLAUDE.md:
```
User: "Run the tests"
Claude: "I don't know your test command. Is it npm test? pytest? cargo test?"
```

With CLAUDE.md:
```
User: "Run the tests"  
Claude: *immediately runs `npm run test:watch` because it knows your setup*
```

### What Goes in CLAUDE.md

1. **Build & Development Commands**
   ```markdown
   # Development Commands
   - Build: `npm run build`
   - Tests: `npm run test:watch`
   - Lint: `npm run lint:fix`
   ```

2. **Architecture Overview**
   ```markdown
   # Architecture
   - `/src/components` - React components with TypeScript
   - `/src/hooks` - Custom hooks following useX pattern
   - `/src/utils` - Pure functions, no React dependencies
   ```

3. **Project-Specific Context**
   ```markdown
   # Important Notes
   - Always run security audit after auth changes
   - Database migrations require staging deployment first
   - API rate limits: 100 req/min in development
   ```

### CLAUDE.md Best Practices

- ✅ **Include actual commands**, not generic descriptions
- ✅ **Explain non-obvious architecture decisions**
- ✅ **Document common gotchas and debugging steps**
- ❌ Don't repeat what's obvious from file structure
- ❌ Don't include generic development advice

## 🤖 The Subagent System

Subagents are **specialized AI personas** designed for specific domains. Each has deep expertise and follows proven patterns.

### How Subagents Work

Each subagent is a markdown file with:

```yaml
---
name: code-reviewer
description: Expert code review specialist. Use immediately after writing code.
model: sonnet
---

# Specialized instructions and expertise...
```

### Key Subagents Explained

#### 🔍 `code-reviewer.md`
**The Production Safety Guardian**

- **Specialty**: Configuration changes that cause outages
- **Focus**: Connection pools, timeouts, memory limits
- **Use When**: After any code changes, especially config
- **Unique Feature**: Categorizes issues by production risk

Example output:
```
🚨 CRITICAL: Database pool size reduced from 20 to 5
This will cause connection starvation under normal load.
Recommendation: Test with production traffic first.
```

#### 🏗️ `backend-architect.md`  
**The System Designer**

- **Specialty**: API design and service boundaries
- **Focus**: RESTful APIs, microservices, database schemas
- **Use When**: Designing new services or major refactors
- **Unique Feature**: Contract-first API design

#### 🔐 `security-auditor.md`
**The Security Specialist**

- **Specialty**: OWASP Top 10, auth flows, encryption
- **Focus**: JWT, OAuth2, input validation, SQL injection
- **Use When**: Security reviews, auth implementation
- **Unique Feature**: Severity-based vulnerability reports

#### 🎯 `prompt-engineer.md`
**The AI Optimizer**

- **Specialty**: LLM prompt optimization
- **Focus**: Chain-of-thought, few-shot examples, model-specific tuning
- **Use When**: Building AI features, improving responses
- **Unique Feature**: Always shows complete, copy-pasteable prompts

#### 📝 SEO Workflow (7 agents)
**The Content Marketing System**

Complete SEO workflow from strategy to optimization:
- `seo-content-planner.md` → Strategy and topic clusters
- `seo-content-writer.md` → SEO-optimized content creation  
- `seo-keyword-strategist.md` → Keyword analysis and density
- `seo-meta-optimizer.md` → Titles, descriptions, schemas
- `seo-structure-architect.md` → Content organization
- `seo-content-auditor.md` → Quality and E-E-A-T analysis
- `seo-authority-builder.md` → Trust signals and credibility

## 🚀 How to Use This Repository

### 1. **For Your Projects**

Copy `CLAUDE.md` to your project root and customize:

```bash
cp CLAUDE.md /path/to/your/project/CLAUDE.md
# Edit to match your project's commands and architecture
```

### 2. **For Specialized Tasks**

Reference subagents in Claude Code conversations:

```
"Act as the code-reviewer subagent from my AI library and review this pull request"
```

### 3. **For Prompt Engineering**

Use prompts from the library as starting points:

```markdown
# From prompt-engineer.md
Always display complete prompt text in clearly marked sections.
Never describe a prompt without showing it.
```

### 4. **For Team Workflows**

Share specific subagents with team members:

```
"Use the security-auditor approach for all auth-related PRs"
"Run backend-architect analysis before system design meetings"  
```

## 💡 Pro Tips

### **Combining Subagents**
```
"Use code-reviewer for security issues, then backend-architect for API design recommendations"
```

### **Context Switching**
```
"Switch to seo-content-writer mode and create a blog post about [topic]"
```

### **Project-Specific Adaptation**
```
"Act as code-reviewer but focus on our GraphQL schema changes and Redis caching patterns"
```

## 📚 Featured Prompts

### **PM Copilot**
- Socratic questioning for product decisions
- First-principles thinking frameworks
- Tradeoff analysis with logical reasoning
- Integration with analytics and project tools

### **System Prompts**
- Writing style replication
- Video AI generation (Sora, Veo3)
- 3D rendering from reference images

## 🔄 Workflow Examples

### **Code Review Workflow**
1. Write/modify code
2. Invoke `code-reviewer` subagent
3. Get severity-categorized feedback
4. Address critical issues first
5. Implement suggestions

### **Content Creation Workflow**  
1. `seo-content-planner` → Strategy
2. `seo-keyword-strategist` → Keywords
3. `seo-content-writer` → Content
4. `seo-meta-optimizer` → Metadata
5. `seo-content-auditor` → Quality check

### **System Design Workflow**
1. `backend-architect` → Service boundaries
2. `security-auditor` → Security review
3. `performance-engineer` → Optimization
4. `code-reviewer` → Implementation review

## 🤝 Contributing

This is a living library. Contributions welcome:

- **New Subagents**: Follow the YAML frontmatter format
- **Prompt Improvements**: Test with real scenarios first
- **Documentation**: Share your workflow discoveries
- **Examples**: Add production use cases

## 🎓 Learning Resources

- **CLAUDE.md Best Practices**: See examples in this repo
- **Subagent Design**: Study existing agents for patterns
- **Prompt Engineering**: Check `prompt-engineer.md` for techniques
- **AI Workflows**: Explore `prompt library/` for inspiration

---

**Ready to 10x your AI productivity?** Start with CLAUDE.md in your next project and experiment with the subagents. Your future self will thank you.

*Built for the AI-native workflow. Optimized for Claude Code.*