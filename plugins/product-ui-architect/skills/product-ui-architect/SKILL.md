---
name: product-ui-architect
description: Design guardrails for SaaS products, modern web apps, dashboards, AI workflow tools, and marketing websites that should feel calm, task-first, and brand-specific instead of generic AI-startup UI. Use when designing or implementing frontend layouts, landing pages, app shells, dashboards, or product screens and the goal is to avoid floating-island nav, bento/card mosaics, fake-premium glass, vague hero sections, or widget soup.
---

# Product UI Architect

## Overview

Use this skill to turn vague "make it modern" requests into layouts driven by user tasks, content hierarchy, and product structure.

Choose an explicit layout archetype before writing code. Prefer alignment, hierarchy, and density over decorative cards and glow.

## Workflow

1. Identify the primary user task, core content objects, top actions, brand personality, and device context.
2. Choose one layout archetype and keep the page or screen consistent with it.
3. Build continuous surfaces with docked edges, aligned sections, and a dominant work area.
4. Choose the right working view for the job: table, list, board, calendar, document, timeline, map, inspector, or editorial section flow.
5. Apply a specific visual system with at least three ownable decisions such as typography, radius, border language, color system, screenshot framing, or motion vocabulary.
6. Run the final self-check before shipping code or mockups.

## Archetype Selection

Choose one of these first:

- Editorial landing page: Use for marketing sites, studios, premium B2B, and products with a strong point of view.
- Product-first SaaS page: Use when the product UI itself is the proof and the interface should appear early.
- Calm app shell: Use for logged-in apps and internal tools with docked navigation and a dominant work surface.
- Data-heavy workspace: Use for admin, operations, CRM, analytics, finance, and knowledge work where records matter more than widgets.

## Hard Rules

- Start from the product job, not from screenshot aesthetics.
- Prefer continuous surfaces over floating islands and detached pill navigation.
- Prefer edge alignment over center-stacked poster layouts.
- Use typography, spacing, and grouping for hierarchy before shadows and effects.
- Use lists and tables for scanning, sorting, ranking, filtering, and batch action workflows.
- Default forms to single-column, top-aligned labels, and nearby validation.
- Use motion only for orientation, state change, progress, and latency softening.
- Make keyboard focus, contrast, labels, and non-color state cues obvious.

## Non-Default Bans

Do not generate these unless the user explicitly asks for them:

- Floating island UI, detached nav pills, and content bubbles as the page skeleton.
- Bento feature mosaics or random card walls as the default SaaS layout.
- Fake-premium decoration such as heavy blur, glass, glow, and oversized radii.
- Weak UX defaults such as carousels in the main hero, icon-only controls without labels, multi-column forms without need, or data tables inside narrow cards.
- Generic AI-product tropes such as purple glow, vague magic-language copy, or prompt-box-plus-orbs compositions.

## Product-Specific Guidance

- Marketing pages: Lead with a clear thesis, show the product or outcome early, integrate proof near claims, and prefer editorial sections or split layouts over card galleries.
- Logged-in apps: Define the primary unit of work first, let navigation recede, keep actions predictable, and prefer master-detail, filters, saved views, inspectors, and inline edit where appropriate.
- Dashboards: Use only when an overview is genuinely needed. Summary metrics should lead to drilldown, and record views should remain accessible.
- AI products: Show system status, checkpoints, provenance, citations, and editable outputs. Do not force chat as the only interaction pattern when a structured UI fits better.

## Reference

Read `references/design-instructions.md` when the task needs the full rule set, the original wording, or detailed guidance for marketing pages, app shells, dashboards, AI products, forms, motion, and self-check criteria.

## Final Self-Check

Confirm all of the following before finalizing:

- The composition is continuous rather than floating.
- The primary task is obvious within a few seconds.
- The main work area is visually dominant.
- Lists or tables are used where scanning matters.
- The design has at least three ownable visual decisions.
- Focus, contrast, state cues, and reduced-motion behavior are covered.
