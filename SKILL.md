---
name: logo-skills
description: Produce Traditional Chinese logo delivery SOPs, checklists, README templates, naming rules, acceptance criteria, and brand-specific handoff profiles for logo delivery packages. Use this when preparing logo delivery materials, brand guideline content, delivery folder standards, or HRDA Plus logo/profile documentation.
license: MIT
---

# Logo Skills

Use this skill when the user asks to create, review, or standardize Logo design delivery materials for designers, brand consultants, vendors, or internal project managers.

## Workflow

1. Confirm the target deliverable type, such as a full SOP, delivery checklist, README template, folder structure, acceptance checklist, logo design prompt guidance, or brand-specific logo profile.
2. Write in formal, clear, executable Traditional Chinese suitable for internal SOP usage unless the user requests another language.
3. Cover practical handoff requirements for websites, apps, print, presentations, social media, and brand documentation.
4. Include concrete file format, version, naming, folder, usage, and validation guidance.
5. When the user needs a full Logo delivery standard, use `references/logo-delivery-standard.md` as the primary reference and adapt it to the user’s organization or project context.
6. When the user mentions HRDA, HRDA+, HRDA PLUS, or Human Resource Digital Assistant, use `references/hrda-plus-brand-profile.md` as the product-specific reference and preserve the HR / DA / PLUS semantic distinction.

## Output requirements

- Prefer Markdown outputs that can be committed directly to a Git repository or company knowledge base.
- Use actionable tables and Markdown checkboxes for delivery lists and acceptance criteria.
- When providing logo design prompts, include brand context, target audience, personality, visual direction, avoid-list, usage contexts, output requirements, and trademark review reminders; provide English prompts when Chinese rendering or PDF output is unreliable.
- Avoid vague recommendations; specify formats, dimensions, required versus optional items, and validation points.
- Keep any generated package or skill files compatible with the Skills Package Specification: `SKILL.md` frontmatter name, package directory name, and `skill.json` name must match.
- If generating or instructing PDF output, use Traditional Chinese only when correct Chinese font embedding and rendering can be verified; otherwise output the PDF in English while keeping editable Markdown/Figma sources available in Traditional Chinese when needed.

## HRDA+ specific requirements

When producing HRDA+ delivery content:

- Treat `HRDA+` and `HRDA PLUS` as the product name.
- Treat `Human Resource Digital Assistant` as the required English tagline.
- Preserve the color logic: HR in gray, DA in orange, PLUS / + as the upgraded AI product marker.
- Include the four product feature groups: 非同步雲端錄影面試、系統內建專業面試題目、語音轉文字精準快速、AI 影像觀察分析。
- Use `hrda-plus` as the canonical file naming prefix.
- Include a clear note that color values extracted from raster artwork are approximate unless verified from the original vector design file or official color tokens.
