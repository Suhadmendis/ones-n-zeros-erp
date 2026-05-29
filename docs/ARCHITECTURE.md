# Architecture

## Overview

This repository is currently a static frontend project. It does not contain a backend, build system, router, package manager, or component framework.

Pages are plain HTML documents that reference local AdminLTE assets and external CDN dependencies.

## Runtime Model

The app can run as static files:

```text
Browser
  |-- HTML pages
  |-- Local CSS from css/
  |-- Local JS from js/
  |-- Local images from assets/
  `-- CDN libraries from cdn.jsdelivr.net
```

## Page Structure

Most full application pages follow the AdminLTE layout pattern:

```text
app-wrapper
|-- app-header
|-- app-sidebar
|-- app-main
`-- app-footer
```

Relative paths vary depending on folder depth:

- Root pages use `./css/...`, `./js/...`, `./assets/...`
- One-level pages use `../css/...`, `../js/...`, `../assets/...`
- Two-level docs pages use `../../css/...`, `../../js/...`, `../../assets/...`

Be careful when moving or copying HTML between folders.

## Important Directories

- `assets/` contains static images and logo assets.
- `css/` contains AdminLTE CSS outputs and source maps.
- `js/` contains AdminLTE JavaScript outputs and source maps.
- `docs/` contains upstream AdminLTE documentation and project Markdown files.
- `examples/` contains authentication-style examples.
- `forms/` contains form examples.
- `layout/` contains layout variants.
- `pages/` contains application-style pages.
- `tables/` contains table examples.
- `UI/` contains UI component examples.
- `widgets/` contains dashboard widget examples.

## Dependencies

Observed dependencies include:

- AdminLTE 4.0.0
- Bootstrap 5.3
- Bootstrap Icons
- OverlayScrollbars
- ApexCharts
- jsVectorMap
- SortableJS
- Source Sans 3 font

Most third-party dependencies are loaded through CDN links in each HTML file.

## Asset Policy

Treat these files as generated or vendor distribution assets unless intentionally updating AdminLTE itself:

- `css/*.min.css`
- `css/*.map`
- `js/*.min.js`
- `js/*.map`

For product-level screen changes, edit HTML first. Add custom project CSS or JavaScript only when a repeated pattern needs it.

## Future Architecture Options

Possible future directions:

- Keep as static prototype for design and workflow validation.
- Add a lightweight static build pipeline.
- Convert repeated HTML into templates or components.
- Integrate with an API backend.
- Migrate to a frontend framework.

Any major architecture change should be documented before implementation.
