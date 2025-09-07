# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is an AI/ML workspace containing specialized Claude subagents and a prompt library for various domains including SEO, development, security, and product management.

## Repository Structure

### Claude Subagents (`claude subagents/`)
Contains 20+ specialized agent configurations for different domains:

**Development & Engineering:**
- `code-reviewer.md` - Expert code review with focus on security and configuration safety
- `backend-architect.md` - RESTful API design and microservices architecture  
- `security-auditor.md` - Security vulnerability detection and OWASP compliance
- `debugger.md` - Error debugging and troubleshooting specialist
- `performance-engineer.md` - Application optimization and performance tuning
- `devops-troubleshooter.md` - Production debugging and system monitoring

**Data & Analytics:**
- `data-engineer.md` - ETL pipelines and data infrastructure
- `data-scientist.md` - Data analysis and BigQuery operations
- `sql-pro.md` - Complex SQL queries and database optimization

**SEO & Content:**
- `seo-content-writer.md` - SEO-optimized content creation
- `seo-content-auditor.md` - Content quality and E-E-A-T analysis
- `seo-keyword-strategist.md` - Keyword analysis and optimization
- `seo-meta-optimizer.md` - Meta titles and descriptions
- `seo-structure-architect.md` - Content organization and schema markup
- `seo-authority-builder.md` - Trust and credibility signals
- `seo-content-planner.md` - Content strategy and planning
- `seo-content-refresher.md` - Content updates and freshness
- `seo-cannibalization-detector.md` - Keyword overlap identification
- `seo-snippet-hunter.md` - Featured snippet optimization

**AI & Prompt Engineering:**
- `prompt-engineer.md` - LLM prompt optimization and AI system design

### Prompt Library (`prompt library/`)
Contains specialized prompts and system instructions:
- `PM Copilot.md` - Product management coaching system with Socratic questioning
- `An Introduction to Prompt Engineering.md` - Educational content on prompting
- `System Prompt - Replicate my writing style.md` - Style replication instructions
- Video AI prompts for Sora, Google Veo3, and 3D rendering

## Key Subagent Capabilities

### Code Review (Most Critical)
The `code-reviewer` subagent has specialized focus on:
- **Configuration changes** that could cause production outages
- Connection pool settings, timeout configurations, memory limits
- Security vulnerabilities and exposed credentials
- Performance degradation risks
- Uses severity-based categorization (Critical/High/Suggestions)

### Security Auditing
- Authentication flows (JWT, OAuth2)
- OWASP Top 10 vulnerability detection
- Input validation and SQL injection prevention
- Security headers and CORS configuration

### AI/ML Prompt Engineering
- Structured prompt optimization using mental models
- Chain-of-thought reasoning and few-shot examples
- Model-specific optimization (Claude, GPT, open models)
- Always displays complete prompt text for copy/paste

## Development Workflow

This repository appears to be a knowledge base rather than a traditional codebase with build/test commands. When working with the content:

1. **For Subagent Modifications**: Maintain the YAML frontmatter structure with name, description, and model fields
2. **For Prompt Engineering**: Always include the complete prompt text in clearly marked sections
3. **For Content Updates**: Preserve the specialized focus areas and structured approaches defined in each agent

## Usage Patterns

- Subagents should be invoked proactively based on their descriptions (e.g., code-reviewer after code changes)
- The PM Copilot prompt includes specific coaching behaviors and access to external tools
- SEO subagents work as a coordinated system for comprehensive content optimization

## Important Notes

- No traditional build/test/lint commands as this is primarily a documentation/configuration repository
- Focus on maintaining the specialized knowledge and structured approaches in each subagent
- The code-reviewer subagent emphasizes configuration change safety as a critical concern
- You're actually the librarian and archivist for my AI Workflow and Prompt Library. Update system Identity accordingly