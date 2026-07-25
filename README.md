# Atlas

Atlas is a browser-to-Figma reconstruction engine for turning structured live websites into editable design systems.

This is the public product showcase for Atlas. The implementation repository is private.

## What Atlas does

Atlas opens a public webpage in a real browser, captures its rendered structure and visual reference, reconstructs the interface as editable Figma layers, and validates the result against the original browser render.

It is designed for structured interfaces such as:

- healthcare and operations dashboards;
- admin panels and internal tools;
- SaaS products and portals;
- content-heavy product pages;
- multi-page web applications with tabs and UI states.

Atlas can discover same-site pages and tab-like states, preserve editable text and controls, translate compatible icons and SVGs into vectors, and withhold incomplete or visually inaccurate captures.

## Current release: v0.4.0

The current milestone introduces a laptop-safe website workflow:

- one target processed at a time;
- bounded local crawls;
- safe stopping after the current capture;
- editable reconstruction with geometry-safe Auto Layout;
- browser-to-Figma visual validation;
- failure retention for later diagnosis.

Local runs are intentionally limited to small chunks while durable cloud scheduling is being developed.

## What this repository contains

- [Product overview](docs/product-overview.md)
- [Architecture](docs/architecture.md)
- [Roadmap](docs/roadmap.md)
- [Public limitations](docs/limitations.md)

The repository contains no Atlas source code, conversion payloads, private application data, credentials, or customer website captures.

## Status

Atlas is an active private development project. The public repository documents the direction and capabilities without exposing the implementation.

## License

The showcase documentation is released under the MIT License. Atlas implementation code is not included and remains proprietary.
