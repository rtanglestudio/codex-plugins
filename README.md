# Product UI Architect for Codex

Product UI Architect is a Codex plugin for teams building SaaS products, dashboards, AI workflow tools, and modern marketing sites.

It helps Codex stop defaulting to generic AI-startup UI patterns such as floating cards, bento-box feature grids, detached pill navigation, and vague hero sections. Instead, it pushes the model toward calm, structured, task-first interfaces built around real workflows, content hierarchy, and product architecture.

## What it does

- guides Codex toward continuous surfaces instead of floating island layouts
- prefers tables, lists, master-detail views, and editorial sections where they fit the task better than cards
- reduces fake-premium styling such as excessive glow, blur, glass, and oversized radii
- reinforces accessibility, strong hierarchy, realistic density, and predictable actions
- helps marketing pages feel sharper and more product-specific
- helps logged-in apps feel like serious tools instead of widget soup

## Who it is for

- founders and product designers working with Codex on UI concepts
- frontend engineers generating or refining product surfaces with AI
- agencies building SaaS landing pages and application shells
- teams that want stronger default design taste in Codex outputs

## Typical use cases

- landing pages for B2B SaaS products
- logged-in app shells and admin workspaces
- dashboards that should prioritize action, not collage
- AI products that need structured workflow UI instead of prompt-box theater
- design reviews for generated React, Next.js, or static marketing pages

## Included plugin

### Product UI Architect

Path: [`plugins/product-ui-architect`](./plugins/product-ui-architect)

The plugin bundles a skill that can be invoked as `$product-ui-architect`.

## Install locally

1. Clone this repository into your local plugins directory:
   `git clone https://github.com/rtanglestudio/codex-plugins.git ~/plugins/codex-plugins`
2. Add or merge the marketplace entry from [`.agents/plugins/marketplace.json`](./.agents/plugins/marketplace.json) into your local `~/.agents/plugins/marketplace.json`.
3. Restart Codex so it picks up the new plugin catalog.

The included local marketplace path expects the repository to live at `~/plugins/codex-plugins`.

## How to use it

Example prompts:

- `Use $product-ui-architect to redesign this SaaS homepage without bento features.`
- `Use $product-ui-architect to turn this dashboard into a calmer operations workspace.`
- `Use $product-ui-architect to review this React app shell for generic AI-generated UI patterns.`

## Why it helps

Most AI-generated interfaces are visually busy, structurally weak, and too dependent on cards, glow, and superficial startup aesthetics. Product UI Architect adds a more opinionated design doctrine so Codex produces interfaces that are easier to ship, easier to use, and more specific to the product.

## Policy

- [Privacy Policy](./PRIVACY.md)
- [Terms of Service](./TERMS.md)
- [MIT License](./LICENSE)
