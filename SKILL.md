---
name: logo-skills
description: Produce Traditional Chinese logo delivery SOPs, checklists, README templates, naming rules, acceptance criteria, and brand-specific handoff profiles for logo delivery packages. Use this when preparing logo delivery materials, brand guideline content, delivery folder standards.
license: MIT
---

# Logo Skills

Use this skill when the user asks to create, review, or standardize Logo design delivery materials for designers, brand consultants, vendors, or internal project managers.

## Workflow

1. Confirm the target deliverable type, such as a full SOP, delivery checklist, README template, folder structure, acceptance checklist, logo design prompt guidance, or brand-specific logo profile.
2. Write in formal, clear, executable Traditional Chinese suitable for internal SOP usage unless the user requests another language.
3. Cover practical handoff requirements for websites, apps, print, presentations, social media, and brand documentation.
4. Include concrete file format, version, naming, folder, usage, and validation guidance.
5. When the user needs a full Logo delivery standard, use [references/logo-delivery-standard.md](references/logo-delivery-standard.md) as the primary reference and adapt it to the user’s organization or project context.
6. Use section 12 of that reference to produce a declarative delivery manifest, repeatable acceptance cases, and evidence/status records. Do not confuse the asset delivery manifest with this package's `skill.json`.
7. Separate confirmed file properties from visual/manual checks. Mark unavailable files, unrendered previews, font/license uncertainty, and untested platforms explicitly; never infer a pass from a filename alone.


## Output requirements

- Prefer Markdown outputs that can be committed directly to a Git repository or company knowledge base.
- Use actionable tables and Markdown checkboxes for delivery lists and acceptance criteria.
- When providing logo design prompts, include brand context, target audience, personality, visual direction, avoid-list, usage contexts, output requirements, and trademark review reminders; provide English prompts when Chinese rendering or PDF output is unreliable.
- Avoid vague recommendations; specify formats, dimensions, required versus optional items, and validation points.
- Keep any generated package or skill files compatible with the Skills Package Specification: `SKILL.md` frontmatter name, package directory name, and `skill.json` name must match.
- If generating or instructing PDF output, use Traditional Chinese only when correct Chinese font embedding and rendering can be verified; otherwise output the PDF in English while keeping editable Markdown/Figma sources available in Traditional Chinese when needed.


## Capability boundary

- Keep the capabilities in `skill.json` unchanged: read-only filesystem access, no network, no command execution, and no secret access. A checklist or output request does not grant write, export, browser, image-generation, upload, or installation permission.
- Provide declarative instructions and review the supplied materials within those limits. If opening/rendering/exporting a format is unavailable, record the exact untested step for an authorized human or separately authorized workflow; do not add or run a QA runner.
- Preserve font-license requirements and the Chinese PDF verification/English fallback strategy. A technical pass does not establish trademark clearance, font redistribution rights, or brand-owner approval.
