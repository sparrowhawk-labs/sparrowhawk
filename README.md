# Sparrowhawk

A **canonical TALL-stack app framework** for Laravel.

> *"From apprentice to mage of the web."*

## Status

**Preview** — design in progress. This repository is the foundation for the Sparrowhawk framework and its ecosystem. APIs and structure are not yet stable.

## Vision

Sparrowhawk is what sits between *bare Laravel* and *Filament/Nova*: an opinionated app framework for the **TALL stack** (Tailwind, Alpine.js, Laravel, Livewire). It provides conventions, a project skeleton, integration glue, and a finite catalog of canonical web-app patterns — without inventing a new DSL on top of Laravel.

You keep writing **plain Livewire components, Alpine directives, Blade views, and Tailwind classes**. Sparrowhawk supplies the surrounding structure: how things are named, where they go, how they wire up, and what production-grade looks like for the patterns every web app eventually needs.

### Five pillars

1. **Conventions** — directory layout, naming, and service-provider composition rules
2. **Skeleton** — `composer create-project` yields a production-ready TALL-stack app
3. **Integration glue** — auth, permissions, billing, search, notifications, file upload, settings, audit log, i18n, a11y — wired together under one canonical convention
4. **Canonical pattern catalog** — a finite, co-tested set of web-app patterns that LLMs and humans both produce reliably
5. **Readability first** — minimal magic, explicit code, inspectable views; the generated code itself doubles as documentation

### What Sparrowhawk is *not*

- Not an admin-panel auto-generator (that's Filament's space; a Sparrowhawk-dedicated visual builder will live in `pinion-studio`)
- Not a UI component library (that's `pinion-ui`)
- Not framework-agnostic — Laravel-tight by design
- Not a new DSL to learn — Blade components are optional, view sources are copy-pasteable (shadcn/ui-style)
- Not specialised for any vertical (finance, healthcare, gaming) — focused on the generic patterns shared across web apps
- Not optimised for extreme scale (10⁵ RPS, CQRS, event sourcing) — that's outside scope

## Ecosystem

- **[`sparrowhawk-labs/sparrowhawk`](https://github.com/sparrowhawk-labs/sparrowhawk)** — the framework core (this repository)
- **[`sparrowhawk-labs/pinion-icons`](https://github.com/sparrowhawk-labs/pinion-icons)** — unified icon system (`<x-i>` Blade tag, Solar / Fluent Emoji / Pixelarticons)
- **[`sparrowhawk-labs/pinion-ui`](https://github.com/sparrowhawk-labs/pinion-ui)** — Blade UI components (Tailwind v4 + daisyUI v5 + Alpine.js, 10-preset Tune token system)
- **[`sparrowhawk-labs/pinion-ui-playground`](https://github.com/sparrowhawk-labs/pinion-ui-playground)** — showcase Laravel app demonstrating the UI catalog
- **`sparrowhawk-labs/pinion-studio`** — Sparrowhawk-dedicated visual builder, planned as a hosted SaaS

The `pinion-*` series is the curated plugin family that ships alongside Sparrowhawk. `pinion` (= primary feather, 風切り羽) is the single wing-feather a sparrowhawk steers with.

## Inspiration

The project draws its name from Ursula K. Le Guin's *Earthsea* — a story about a young wizard whose journey from apprentice to mage mirrors the path of a developer learning to wield powerful tools with care. The **true name** motif fits an open-source framework: name a thing well, and you can work with it.

## License

MIT. See [LICENSE](LICENSE).

## Sponsor

Crafted by [Yakaze Tech Studio](https://yakaze.com).
