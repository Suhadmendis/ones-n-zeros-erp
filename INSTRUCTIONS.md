# Instructions

Use this file as the quick-start instruction sheet for working on Ones n Zeros ERP.

## Before You Start

1. Confirm you are in the repository root:

   ```sh
   pwd
   ```

   Expected path:

   ```text
   /Users/akilamendis/PROJECTS/Ones n Zeros/Commont-ERP/ones-n-zeros-erp
   ```

2. Confirm you are on the development branch:

   ```sh
   git status --short --branch
   ```

   Expected branch:

   ```text
   dev
   ```

3. Read these files before making changes:

   ```text
   README.md
   AGENTS.md
   docs/PROJECT_BRIEF.md
   docs/ARCHITECTURE.md
   docs/DEVELOPMENT.md
   docs/ROADMAP.md
   ```

## Project Type

This is currently a static AdminLTE 4 frontend project.

Do not assume there is:

- A package manager
- A build step
- A frontend framework
- A backend
- A database
- A test runner

## How To Preview

Open `index.html` directly, or run a static server from the repository root:

```sh
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Development Rules

- Keep changes focused.
- Prefer existing AdminLTE and Bootstrap patterns.
- Preserve relative asset paths.
- Do not edit minified files or source maps by hand.
- Do not introduce new dependencies without approval.
- Do not delete demo pages unless explicitly requested.
- Do not remove license or attribution comments from vendor files.
- Update documentation when changing structure, workflow, or conventions.

## Recommended Edit Targets

For normal ERP screen work, edit:

- `*.html`
- Project-owned Markdown files
- New project-owned CSS or JavaScript files, if needed

Avoid editing unless there is a clear reason:

- `css/adminlte.css`
- `js/adminlte.js`

Do not manually edit:

- `*.min.css`
- `*.min.js`
- `*.map`

## Product Direction

Convert the AdminLTE demo into an ERP interface for Ones n Zeros.

Near-term priorities:

1. Branding
2. Navigation
3. ERP dashboard
4. Core module screens
5. Documentation cleanup

## Verification

Before finishing a change, verify:

- The changed page loads.
- CSS and JavaScript assets resolve.
- Sidebar toggle works.
- Dropdowns and collapsible controls work.
- Icons render.
- Layout works on desktop and mobile widths.
- Text does not overlap or overflow.

## Git Rules

- Work on `dev` unless instructed otherwise.
- Do not commit unless asked.
- Do not revert user changes.
- Keep local/generated files ignored.
