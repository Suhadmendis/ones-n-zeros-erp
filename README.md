# Ones n Zeros ERP

Static AdminLTE-based ERP interface scaffold for Ones n Zeros.

This repository currently contains a customized working copy of the AdminLTE 4 static distribution. It is intended to become an ERP frontend, with pages, layouts, widgets, tables, forms, and documentation available as starting points for future product development.

## Current State

- Static HTML, CSS, JavaScript, and image assets.
- No package manager or build pipeline is configured yet.
- AdminLTE 4 assets are checked into `css/` and `js/`.
- Most pages still contain upstream AdminLTE demo content and should be treated as scaffolding.
- External runtime dependencies are loaded from CDNs inside the HTML files.

## Preview

Open `index.html` directly in a browser, or serve the folder with any static HTTP server.

Example:

```sh
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Repository Map

```text
.
|-- index.html              # Main dashboard demo page
|-- index2.html             # Alternate dashboard demo page
|-- index3.html             # Alternate dashboard demo page
|-- assets/                 # Images, logos, avatars, product images
|-- css/                    # AdminLTE CSS, RTL CSS, minified builds, maps
|-- js/                     # AdminLTE JavaScript, minified builds, maps
|-- docs/                   # AdminLTE docs plus project documentation
|-- examples/               # Login, register, lockscreen examples
|-- forms/                  # Form layout, elements, validation, wizard pages
|-- layout/                 # Layout variants and sidebar/header examples
|-- mailbox/                # Mailbox example pages
|-- pages/                  # ERP-adjacent pages and app demos
|-- tables/                 # Table examples
|-- UI/                     # UI components and timeline examples
`-- widgets/                # Card, info box, and small box examples
```

## Key Technologies

- AdminLTE 4.0.0
- Bootstrap 5.3
- Bootstrap Icons
- Vanilla JavaScript
- OverlayScrollbars
- ApexCharts
- jsVectorMap
- SortableJS

## Development Direction

The next development phase should convert the generic AdminLTE demo into a coherent ERP product interface:

1. Apply Ones n Zeros branding across titles, navigation, logos, footer, and metadata.
2. Decide the ERP module structure before deeply editing pages.
3. Convert useful demo pages into real product screens.
4. Remove unused upstream demo pages only after confirming they are not needed as references.
5. Introduce a build system only when it solves a real development problem.

## AI Agent Instructions

AI agents should read `AGENTS.md` before changing the repository.

For project context, also read:

- `docs/PROJECT_BRIEF.md`
- `docs/ARCHITECTURE.md`
- `docs/DEVELOPMENT.md`
- `docs/ROADMAP.md`
