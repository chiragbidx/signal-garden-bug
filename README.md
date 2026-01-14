# 🐼 Panda Template Manifest – Creative Startup Template

> **This document defines how AI must understand and operate on the Creative Startup template inside Panda.**  
> It is the single source of truth for AI-driven code suggestions.

---

## 1. Template Metadata (DO NOT MODIFY STRUCTURE)

```md
# Panda Template Manifest

template_name: "Creative Startup"
template_id: "panda-creative-startup-001"
template_version: "1.0.0"
template_type: "marketing-landing"
layout_style: "creative-modern"
technology_stack: ["HTML5", "CSS3"]
responsive: true
dark_mode: false
rtl_supported: false

author: "Panda Templates"
last_updated: "2026-01-04"
```

---

## 2. Template Intent & Design Philosophy

```md
## Template Intent

This template is designed for:
- Startups
- Creative studios
- Early-stage SaaS products
- Founder-led companies

Primary goals:
- Bold first impression
- Story-driven layout
- Lead capture and conversion
```

### Design Rules

```md
## Design Rules

- Modern creative aesthetic
- Visual storytelling with imagery
- Balanced text-to-image ratio
- Smooth visual flow between sections
```

⚠️ **AI DESIGN RULE**  
Do NOT introduce heavy animations or experimental layouts unless explicitly requested.

---

## 3. File & Folder Structure (SOURCE OF TRUTH)

```md
## File Structure

/
├── index.html                     # Primary landing page
├── creative-startup/
│   ├── css/
│   │   └── style.css              # Core styles (READ-ONLY by default)
│   ├── standard-blog.html
│   ├── single-blog.html
│   └── standalone.html
├── vendor/                        # Third-party libraries (READ-ONLY)
├── assets/                        # Images & icons
```

### File Rules

```md
- Do NOT edit vendor files
- Do NOT rename folders
- Do NOT move HTML files
- Do NOT inline CSS
```

---

## 4. Change Control Rules (CRITICAL – AI ENFORCED)

### styles.css (STRICT)

```md
- style.css is READ-ONLY by default
- The AI MUST NOT modify CSS unless the user explicitly requests styling changes
- Vendor CSS must NEVER be edited
```

---

### Images (STRICT)

```md
Images are READ-ONLY by default.

Image changes are allowed ONLY if the user explicitly:
- Mentions the image (filename, path, section, or alt text), OR
- Provides a direct image URL

Otherwise, image modifications are NOT allowed.
```

---

### Sections (STRICT)

```md
ALL sections across index.html and standalone.html are IMMUTABLE by default.

The AI MUST NOT:
- Remove sections
- Add new sections
- Reorder sections
- Merge sections

Allowed ONLY if user explicitly names the section or file.
```

---

## 5. Default AI Assumptions

```md
Unless explicitly stated:

- HTML structure remains unchanged
- CSS remains unchanged
- Images remain unchanged
- All sections remain present
- Only TEXT CONTENT is editable
```

---

## 6. Sections Overview (AI NAVIGATION MAP)

```md
1. Header / Navigation
2. Hero
3. About / Vision
4. Services / What We Do
5. Feature Highlights
6. Portfolio / Work
7. Testimonials
8. Blog Preview
9. Call To Action
10. Footer
```

---

## 7. Section-Level Contracts

```md
## Section: Hero

section_id: "hero"
html_container_id: "hero-section"
css_scope_prefix: ".hero"

Purpose:
- Establish brand message
- Capture attention

Editable Content:
- Headline
- Subheadline
- CTA text

Non-Editable:
- Layout
- Animations
- Class names
```

---

## 8. Section Integrity Contract

```md
Sections are IMMUTABLE by default.

AI MAY:
- Edit text content
- Update copy within defined limits

AI MUST NOT:
- Alter structure
- Rename classes or IDs
- Remove containers
```

---

## 9. CSS Architecture Rules

```md
- Section-scoped styles
- No new frameworks
- No !important usage
- Mobile-first approach
```

---

## 10. Typography System

```md
Fonts and weights are defined in style.css
AI must NOT change typography unless explicitly requested
```

---

## 11. Color System

```md
All colors are defined in style.css
AI must NOT introduce new colors unless explicitly approved
```

---

## 12. AI Code Suggestion Modes

### Full Code Suggestion

```md
- Return full file content
- Use ONLY for large or structural changes
```

### Diff-Based Partial Suggestion

```md
- Return minimal diffs
- Preferred for small content edits
```

---

## 13. Mode Conflict Resolution

```md
Priority Order:
1. Explicit user instruction
2. Diff-based suggestion (default)
3. Full code suggestion
```

---

## 14. Change Permission Matrix

```md
| Change Type       | Default | Explicit |
|------------------|---------|----------|
| Text             | ✅      | ❌       |
| CSS              | ❌      | ✅       |
| Images           | ❌      | ✅       |
| Sections         | ❌      | ✅       |
| Vendor files     | ❌      | ❌       |
| New files        | ❌      | ✅       |
| JavaScript       | ❌      | ✅       |
```

---

## 15. AI Hard Stop Conditions

```md
The AI MUST STOP if:
- CSS change is implied but not requested
- Image change is implied without image reference or URL
- Section change is implied without section name
- Vendor files are targeted
```

---

## 16. Version Notes

```md
v1.0.0
- Initial Creative Startup template
- Multi-page structure
- Vendor-managed assets
```

---

## 17. AI FINAL DIRECTIVE

```md
This manifest is the highest authority.

If conflicts arise:
→ Follow this document
→ Ask for clarification
→ Do NOT assume
```
