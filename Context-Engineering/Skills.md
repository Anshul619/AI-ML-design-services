# Agent Skills
- Agents are increasingly capable, but often don’t have the context they need to do real work reliably. 
- [Skills](https://agentskills.io/home) solve this by giving agents access to procedural knowledge and company, team, and user-specific context they can load on demand. 
- Agents with access to a set of skills can extend their capabilities based on the task they’re working on.

# What are skills?
- [Agent Skills](https://agentskills.io/what-are-skills) are a lightweight, open format for extending AI agent capabilities with specialized knowledge and workflows.

````
my-skill/
├── SKILL.md          # Required: instructions + metadata
├── scripts/          # Optional: executable code
├── references/       # Optional: documentation
└── assets/           # Optional: templates, resources
````

# The SKILL.md file
- Every skill starts with a SKILL.md file containing YAML format and Markdown instructions:

````
---
name: pdf-processing
description: Extract text and tables from PDF files, fill forms, merge documents.
---

# PDF Processing

## When to use this skill
Use this skill when the user needs to work with PDF files...

## How to extract text
1. Use pdfplumber for text extraction...

## How to fill forms
...
````

# References
- [Mattpocock - Skills For Real Engineers](https://github.com/mattpocock/skills/tree/main)
- [The Agent Skills Directory](https://skills.sh/)
