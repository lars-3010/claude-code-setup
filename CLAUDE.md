# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# CLAUDE CODE AGENT-BASED DEVELOPMENT TEMPLATE

*project philosophy: "Spec-driven development with specialized agents"*

## PROJECT MISSION

Experimental template for spec-driven development using Claude Code's agent system, inspired by AWS Kiro's specification-first approach. Focus: Testing agent roles, templates, and context management for improved development workflows.

## SPEC-DRIVEN DEVELOPMENT

For spec-driven development, follow `.claude/specs/` specific folder for features.

## ESSENTIAL COMMANDS

**Setup & Quick Start:**
- Add your project-specific setup commands here
- Example: `npm install` or `pip install -r requirements.txt`

**Quality Assurance:**  
- Add your linting/testing commands here
- Example: `npm run lint` and `npm run test`

## ADAPTIVE CONTEXT SYSTEM

Load specific context based on task type using `.claude/` directory structure:

### Available Agents (`.claude/agents/`)
- **product-owner-agent.md** - Senior Product Manager for professional requirements with business focus
- **design-agent.md** - Principal Architect for system design with visualization
- **developer-agent.md** - Principal Python Developer for clean code with architectural compliance  
- **tasks-agent.md** - Engineering Manager for implementation roadmap with development workflow
- **architecture-agent.md** - Senior System Architect for design enhancement and validation
- **dev-workflow-orchestrator.md** - Technical Lead for complete specification workflow

### Available Commands (`.claude/commands/`)
- **requirements.md** - Create professional requirements specification
- **design.md** - Create system design specification  
- **develop.md** - Development task execution
- **tasks.md** - Create implementation task breakdown
- **architecture-review.md** - Architecture review and validation
- **code-review.md** - Code review and quality assessment
- **status.md** - Project status and progress tracking
- **validate.md** - Validation and testing workflows

### Guidelines (`.claude/guidelines/`)
- **architectural-guidelines.md** - SOLID principles, patterns, and architectural decisions
- **coding-standards.md** - Code quality standards and best practices

### Templates (`.claude/templates/`)
- **requirements-template.md** - Requirements specification template
- **design-template.md** - System design specification template
- **tasks-template.md** - Implementation tasks template

## CONTEXT LOADING STRATEGY

**For Development Tasks:**
- Agent: `developer-agent.md` - Clean code with architectural compliance
- Guidelines: `architectural-guidelines.md` + `coding-standards.md`

**For Architecture/Design:**
- Agent: `design-agent.md` or `architecture-agent.md` - System design and validation
- Guidelines: `architectural-guidelines.md`

**For Requirements/Planning:**
- Agent: `product-owner-agent.md` or `tasks-agent.md` - Business requirements and task planning
- Templates: Relevant specification templates

**For Workflow Orchestration:**
- Agent: `dev-workflow-orchestrator.md` - Complete specification workflow coordination

### Specification Output Directory
All agents should write specifications to: `.claude/specs/`

## MCP SERVERS

*Add your MCP server configurations here*

<!-- Example:
### Server Name
- **Purpose**: Description of what this server provides
- **Configuration**: Setup instructions or config details
- **Tools**: List of available tools/capabilities
-->

## USAGE INSTRUCTIONS

1. **Start with Product Owner**: Define business requirements and user stories
2. **Design Architecture**: Create system design with diagrams and technical decisions
3. **Plan Implementation**: Break down into detailed technical specifications  
4. **Create Workflow**: Define development process and task breakdown
5. **Iterate**: Refine specifications based on feedback and discoveries

## DEVELOPMENT REMINDERS

- Follow `.claude/specs/` for spec-driven development
- Use agents and guidelines for contextual development guidance
- Update documentation when adding features or changing workflows
- Test role definitions and template effectiveness
- Document context management improvements