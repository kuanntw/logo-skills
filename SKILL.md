---
name: logo-skills
description: Produce Traditional Chinese logo delivery SOPs, checklists, README templates, naming rules, and acceptance criteria for brand identity handoff packages.
license: MIT
---

# Logo Skills

Use this skill when the user asks to create, review, or standardize Logo design delivery materials for designers, brand consultants, vendors, or internal project managers.

## Workflow

1. Confirm the target deliverable type, such as a full SOP, delivery checklist, README template, folder structure, acceptance checklist, or logo design prompt guidance.
2. Write in formal, clear, executable Traditional Chinese suitable for internal SOP usage unless the user requests another language.
3. Cover practical handoff requirements for websites, apps, print, presentations, social media, and brand documentation.
4. Include concrete file format, version, naming, folder, usage, and validation guidance.
5. When the user needs a full Logo delivery standard, use `logo-delivery-standard.md` as the primary reference and adapt it to the user’s organization or project context.

## Output requirements

- Prefer Markdown outputs that can be committed directly to a Git repository or company knowledge base.
- Use actionable tables and Markdown checkboxes for delivery lists and acceptance criteria.
- When providing logo design prompts, include brand context, target audience, personality, visual direction, avoid-list, usage contexts, output requirements, and trademark review reminders; provide English prompts when Chinese rendering or PDF output is unreliable.
- Avoid vague recommendations; specify formats, dimensions, required versus optional items, and validation points.
- Keep any generated package or skill files compatible with the Skills Package Specification: `SKILL.md` frontmatter name, package directory name, and `skill.json` name must match.
- If generating or instructing PDF output, use Traditional Chinese only when correct Chinese font embedding and rendering can be verified; otherwise output the PDF in English while keeping editable Markdown/Figma sources available in Traditional Chinese when needed.
