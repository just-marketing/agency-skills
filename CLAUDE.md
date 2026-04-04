# Juma Agency Skills - Contributor Guidelines

## Overview

This repository contains Claude Code skills built by Juma.ai for marketing agencies managing multiple clients. Each skill produces client-deliverable outputs following agency workflows.

## Skill Format

Every skill lives in `skills/<skill-name>/SKILL.md` and follows this structure:

### YAML Frontmatter (required)

```yaml
---
name: juma-skill-name
description: "Use when [trigger 1], [trigger 2], or [trigger 3]. [What it produces]."
---
```

- `name`: Must use `juma-` prefix
- `description`: Must start with "Use when" and describe triggering conditions + output

### Required Sections

1. **Overview** - 2-3 sentences explaining what the skill does and why agencies need it
2. **When to Use** - Bullet list of triggering conditions
3. **Prerequisites** - Always include `juma-client-context`. List other dependent skills
4. **Process** - Step-by-step instructions (numbered steps with sub-steps)
5. **Output Format** - Exact deliverable structure with headers and template
6. **Common Mistakes** - What goes wrong and how to avoid it
7. **Related Skills** - Cross-references to connected skills

## Key Principles

- **`juma-client-context` is always a prerequisite** - Every skill must reference client context
- **Client-deliverable quality** - Outputs should be ready to present to clients (except internal-only skills like `juma-retainer-review`)
- **Agency perspective** - Frame everything from the agency's viewpoint, not the client's in-house team
- **Actionable outputs** - Every deliverable must include specific next steps or recommendations
- **Cross-referencing** - Skills should reference related skills where workflows connect

## Naming Convention

All skills use the `juma-` prefix to avoid namespace collisions:
- `juma-seo-audit` not `seo-audit`
- `juma-client-context` not `client-context`

## Skill Categories

| Category | Skills | Purpose |
|----------|--------|---------|
| Foundation | client-context, client-brief | Core data every other skill needs |
| Revenue | proposal, sow, reporting, client-qbr | Deliverables that generate/retain revenue |
| Audit/Strategy | channel-audit, competitor-intel, seo-audit, geo-audit, cro-audit, campaign-plan | Assessment and planning |
| Execution | content-calendar, paid-media-plan, ab-test-plan, analytics-setup | Implementation planning |
| Business Ops | case-study, upsell-finder, retainer-review, onboarding-checklist | Internal agency operations |
