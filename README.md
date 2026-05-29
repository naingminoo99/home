# Home

Personal knowledge base for home renovation, maintenance, and smart-home research.

This repo is structured for LLM-readable querying — every topic file uses YAML frontmatter so it can be loaded into a Claude Project and chatted with over the next ~2 years of research, decisions, and follow-through.

## Folder layout

- `smart-home/` — devices, automations, network
- `maintenance/` — recurring upkeep (mold, grease, laundry, HVAC, schedule)
- `renovation/` — plans, budget, contractors, materials
- `inventory/` — appliances, warranties
- `research/` — open-ended research notes

## Frontmatter convention

Every topic file starts with a YAML frontmatter block:

```yaml
---
category: maintenance        # top-level folder name
subcategory: mold            # filename without .md
status: research             # research | decided | in-progress | done
last_updated: 2026-05-28     # ISO date
priority: medium             # low | medium | high
tags: [bathroom, prevention]
---
```

Keep notes in plain markdown under standard sections (Overview, Products / Solutions Researched, Decisions, Schedule / Frequency, Sources). See `TEMPLATE.md` for the blank starting point.

## Adding a new topic

1. Copy `TEMPLATE.md` into the appropriate folder and rename it.
2. Update the frontmatter fields.
3. Fill in the sections.
4. Commit.

## Querying with Claude

The plan is to load this repo into a Claude Project (via the GitHub integration, or by syncing files) and use it as the knowledge base for chat-based recall, planning, and decision-making.
