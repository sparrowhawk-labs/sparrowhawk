# Sparrowhawk

A **canonical TALL-stack app framework** for Laravel.

> *"From apprentice to mage of the web."*

## Status

**Preview** — design in progress. This repository is the foundation for the Sparrowhawk framework and its ecosystem. APIs and structure are not yet stable.

## Vision

Sparrowhawk is what sits between *bare Laravel* and *Filament / Nova*: an opinionated app framework for the **TALL stack** (Tailwind, Alpine.js, Laravel, Livewire). It provides conventions, a project skeleton, integration glue, and a finite catalog of canonical web-app patterns — without inventing a new DSL on top of Laravel.

You keep writing **plain Livewire components, Alpine directives, Blade views, and Tailwind classes**. Sparrowhawk supplies the surrounding structure: how things are named, where they go, how they wire up, and what production-grade looks like for the patterns every web app eventually needs.

### Five pillars

1. **Conventions** — directory layout, naming, and service-provider composition rules
2. **Skeleton** — `composer create-project` yields a production-ready TALL-stack app
3. **Integration glue** — auth, permissions, billing, search, notifications, file upload, settings, audit log, i18n, a11y — wired together under one canonical convention
4. **Canonical pattern catalog** — a finite, co-tested set of web-app patterns that LLMs and humans both produce reliably
5. **Readability first** — minimal magic, explicit code, inspectable views; the generated code itself doubles as documentation

### What Sparrowhawk is *not*

- Not an admin-panel auto-generator (that's Filament's space; the Sparrowhawk-native visual builder is **Sparrowhawk Studio**, a hosted SaaS — see Ecosystem below)
- Not a UI component library (that's `pinion-ui`)
- Not framework-agnostic — Laravel-tight by design
- Not a new DSL to learn — Blade components are optional, view sources are copy-pasteable (shadcn/ui-style)
- Not specialised for any vertical (finance, healthcare, gaming) — focused on the generic patterns shared across web apps
- Not optimised for extreme scale (10⁵ RPS, CQRS, event sourcing) — that's outside scope

## Ecosystem

Sparrowhawk Labs ships two related-but-distinct brand systems under one roof:

- **Sparrowhawk** — the "wizard tools" axis: the framework itself plus the visual builder built on it
- **Pinion** — the plugin family: UI components, icons, and future companion plugins

### Open source

- **[`sparrowhawk-labs/sparrowhawk`](https://github.com/sparrowhawk-labs/sparrowhawk)** — the framework core (this repository)
- **[`sparrowhawk-labs/pinion-ui`](https://github.com/sparrowhawk-labs/pinion-ui)** — Blade UI components (Tailwind v4 + daisyUI v5 + Alpine.js, 11-preset Tune token system)
- **[`sparrowhawk-labs/pinion-icons`](https://github.com/sparrowhawk-labs/pinion-icons)** — unified icon system (`<x-i>` Blade tag, Solar / Fluent Emoji / Pixelarticons)
- **[`sparrowhawk-labs/pinion-ui-playground`](https://github.com/sparrowhawk-labs/pinion-ui-playground)** — showcase Laravel app demonstrating the UI catalog

### Commercial

- **Sparrowhawk Studio** — the Sparrowhawk-native visual builder, planned as a hosted SaaS. Drag-and-drop assembly that emits **canonical Sparrowhawk code** (plain Livewire / Alpine / Blade) — same patterns you'd hand-write, generated faster and stitched cleanly into a Sparrowhawk skeleton.

### Why two brands

The `pinion-*` series is the curated plugin family that ships alongside Sparrowhawk. `pinion` (= primary feather, 風切り羽) is the single wing-feather a sparrowhawk steers with — the metaphor keeps the plugin family rooted to the framework while letting each piece (UI, icons, future plugins) stand on its own as a usable Composer package.

Sparrowhawk and Sparrowhawk Studio share the framework name because they are the same conceptual thing seen from two angles: the OSS framework you write code against, and the SaaS workbench that helps you generate that code visually.

## Inspiration

The project draws its name from Ursula K. Le Guin's *Earthsea* — a story about a young wizard (Sparrowhawk) whose journey from apprentice to mage mirrors the path of a developer learning to wield powerful tools with care. The **true name** motif fits an open-source framework: name a thing well, and you can work with it.

## License

MIT. See [LICENSE](LICENSE).

## Sponsor

Crafted by [Yakaze Tech Studio](https://yakaze.com).
