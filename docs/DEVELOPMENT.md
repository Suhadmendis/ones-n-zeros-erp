# Development Guide

## Prerequisites

No installation step is currently required.

The project can be viewed directly in a browser, but using a local static server is usually better because browser behavior is closer to a deployed site.

## Local Preview

From the repository root:

```sh
python3 -m http.server 8000
```

Open:

```text
http://localhost:8000
```

## Common Entry Points

- `index.html` - primary dashboard
- `index2.html` - alternate dashboard
- `index3.html` - alternate dashboard
- `pages/` - application-style pages
- `forms/` - form examples
- `tables/` - table examples
- `widgets/` - dashboard widget examples

## Recommended Workflow

1. Create or switch to a feature branch.
2. Read `AGENTS.md` and relevant docs.
3. Identify the page or module being changed.
4. Make focused edits.
5. Preview the page in a browser.
6. Check responsive behavior.
7. Update Markdown documentation if the change affects conventions or structure.

## HTML Editing Notes

- Keep relative paths correct for the file location.
- Preserve required AdminLTE structure unless intentionally changing layout.
- Keep Bootstrap classes consistent with nearby examples.
- Prefer existing AdminLTE components before creating new patterns.
- Remove placeholder/demo text only when replacing it with product content.

## CSS Editing Notes

- Avoid broad changes to `css/adminlte.css` for one-page needs.
- Prefer page-level utility classes first.
- If custom project styling grows, create a dedicated project stylesheet and document it here.
- Do not edit minified CSS by hand.

## JavaScript Editing Notes

- Existing behavior is mostly AdminLTE and page-local scripts.
- Keep page-specific JavaScript near the page unless it becomes shared behavior.
- Do not edit minified JavaScript by hand.
- Avoid adding new dependencies without documenting why.

## Manual QA Checklist

For changed pages, verify:

- Page loads without missing local assets.
- CDN dependencies load when online.
- Sidebar toggle works.
- Dropdowns and collapses work.
- Icons render.
- Tables and forms remain usable.
- Layout works at desktop and mobile widths.
- Text does not overlap or overflow controls.

## Git Notes

Current development branch:

```text
dev
```

Do not commit changes unless explicitly asked.

