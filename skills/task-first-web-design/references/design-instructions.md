# AGENTS.md

Design instructions for Codex when generating SaaS products, modern web apps, dashboards, and marketing websites.

The purpose of this file is to stop default AI-looking layouts: floating islands, bento boxes, detached pill nav bars, random card walls, and generic "premium startup" compositions.

---

## 0) Prime directive

Design for the product's job, not for screenshot aesthetics.

Every layout must start from:
- the primary user task
- the content hierarchy
- the interaction model
- the brand personality
- the device context

Do not start from Dribbble-style composition patterns.
Do not default to floating cards.
Do not default to bento grids.
Do not use ornamental depth where structure should do the work.

---

## 1) Global design stance

Assume the best modern web apps feel:
- calm, sharp, and intentional
- dense enough to be useful
- brand-specific rather than template-like
- structured by alignment, hierarchy, and rhythm
- fast, legible, and obviously interactive

Aim for:
- strong information architecture
- clear task flows
- restrained but intentional visual identity
- functional motion
- accessibility by default

Avoid:
- "vibe-coded" generic startup pages
- over-rounded floating modules
- glassmorphism unless explicitly requested
- random gradient blobs
- decorative dashboards with no task logic
- giant empty padding that reduces usefulness
- hero sections that look expensive but explain nothing

---

## 2) Absolute bans unless explicitly requested

Do not generate any of the following by default:

1. **Floating island UI**
   - detached nav bars hovering over the page
   - content panels that float separately from the page frame
   - isolated rounded rectangles with shadow as the main organizing system

2. **Bento/grid-of-cards homepage patterns**
   - feature grids made of mixed-size boxes as the default SaaS layout
   - dashboard-like card mosaics for products that are not actually dashboard products
   - stacked card galleries where a clearer list, table, split layout, or editorial section would work better

3. **Fake-premium decoration**
   - excessive blur, frosted glass, glow, lens flares
   - shadow-heavy components used to create hierarchy that typography should create
   - oversized corner radii on every container

4. **Weak UX defaults**
   - carousels in the main hero
   - ambiguous icon-only controls without labels where labels are needed
   - forms split into multiple columns without a strong reason
   - data tables compressed inside narrow cards

5. **Overused AI aesthetics**
   - dark background + purple/blue glow + floating widgets
   - giant centered headline + tiny subcopy + random UI mockup on the right
   - same old testimonial cards, logo strip, pricing cards, FAQ accordion stack with no distinct structure

If a prompt is underspecified, choose a content-led editorial layout or a calm product shell, not floating islands.

---

## 3) Preferred layout archetypes

Choose one of these first. State it internally before designing.

### A. Editorial landing page
Use for marketing sites, studios, premium B2B, AI products with a point of view.

Characteristics:
- full-bleed sections
- strong typographic hierarchy
- deliberate rhythm between dense and open areas
- image/UI compositions integrated into the section, not floating above it
- concise copy with obvious scan paths
- product proof embedded into the story

Preferred structure:
- value proposition
- proof / product in context
- how it works
- differentiators
- deeper feature sections
- social proof
- CTA

### B. Product-first SaaS page
Use when the interface itself is the product.

Characteristics:
- the UI is the hero, but framed by a strong brand system
- page composition is continuous, not a pile of cards
- product screenshots appear as evidence, not decoration
- summary-first information architecture
- selective drill-down, not endless scrolling

Preferred structure:
- headline and 1-sentence value prop
- screenshot or workflow strip
- TL;DR product overview
- 3-5 core capabilities
- integration / automation / AI / governance section as needed
- proof / trust / CTA

### C. Calm app shell
Use for logged-in apps and internal tools.

Characteristics:
- docked navigation
- clear work surface
- subdued chrome
- predictable placement of actions
- compact controls
- density without noise

Preferred shell:
- left nav for product/location
- top bar for global actions/search/create/context
- main content area gets priority
- side panels only when contextually needed
- lists, tables, timelines, boards, or inspectors based on task

### D. Data-heavy workspace
Use for admin, operations, analytics, CRM, finance, infra, knowledge work.

Characteristics:
- tables/lists first
- filters and saved views visible
- summaries above data, not replacing data
- side detail panels for inspection
- charts support decisions; they do not replace the underlying records

Preferred structure:
- page title + scope
- filters/search/actions
- summary metrics
- primary table or list
- detail panel / drilldown
- secondary charts only where useful

---

## 4) Layout rules

### 4.1 Build continuous surfaces
Use shared planes, aligned sections, and docked edges.

Prefer:
- full-width wrappers
- split layouts
- inset content regions inside a larger surface
- clearly anchored sidebars and headers

Avoid:
- each section living in its own bubble
- detached nav pill floating in space
- cards as the page skeleton

### 4.2 Let hierarchy come from type and spacing
Use typography, alignment, grouping, and contrast to establish importance.
Shadows are secondary.

Prefer:
- large/small type contrast
- consistent spacing scale
- sentence-case headings
- stable baselines and gutters

Avoid:
- using ten cards to simulate information architecture
- every block looking equally important

### 4.3 Make the work area visually dominant
Navigation and support elements should recede. The task area should lead.

Prefer:
- quieter sidebars
- compact tabs
- restrained separators
- fewer icons, used intentionally

Avoid:
- bright chrome competing with content
- pills and chips everywhere
- decorative borders between every item

### 4.4 Prefer edge alignment over center-stacking
Most serious web apps and SaaS sites should be edge-aligned, not centered like a poster.

Prefer:
- left-aligned copy blocks
- asymmetric composition
- grid-based alignment
- anchored screenshots

Avoid:
- everything centered by default
- oversized empty space around key actions

---

## 5) Cards, lists, tables, and grids

### 5.1 Cards are not the default
Use cards only when the user is browsing heterogeneous content or comparing grouped modules.

Good uses:
- template galleries
- marketplaces
- media collections
- lightweight overview widgets

Bad uses:
- core CRUD workflows
- searchable entity management
- settings
- admin panels
- anything that needs scanning, sorting, ranking, or high information density

### 5.2 Prefer lists/tables for serious work
For productivity tools, lists and tables usually outperform card mosaics.

When the user needs to:
- scan many records
- compare values across rows
- sort/filter/search
- act on multiple items

Use:
- tables
- row lists
- master-detail views
- kanban only when status movement is primary

### 5.3 Don't put dense data in little boxes
Give tables and operational views room.
If content is cramped, widen the work area or move details into a side panel or dedicated page.

### 5.4 Use grid systems with discipline
A grid is for alignment and rhythm, not for creating a bento collage.

---

## 6) Navigation and product architecture

Navigation should feel predictable, adaptable, and task-aware.

Rules:
- top bar = universal/global actions
- side nav = product areas and movement within the product
- page header = local context, title, primary actions
- tabs = sibling views only
- breadcrumbs only when hierarchy truly matters

Use progressive disclosure:
- basic paths should feel obvious for new users
- power features should stay reachable without cluttering the default state

Never create navigation that looks more expressive than the content it leads to.

---

## 7) Motion rules

Motion is functional, not decorative.

Use motion to:
- explain state changes
- preserve spatial relationships
- support orientation
- soften latency
- reveal hierarchy

Do:
- keep transitions short and meaningful
- animate between related states
- use subtle fades, shifts, scale changes, and shared-element logic
- respect reduced-motion preferences

Do not:
- add animation just to feel premium
- use continuous ambient motion with no UX value
- auto-advance carousels in core product flows
- use parallax, spinning, or depth simulation by default

If motion is removed, the interface must still make sense.

---

## 8) Accessibility and interaction rules

Always design for accessibility from the start.

Required:
- visible keyboard focus
- strong contrast
- obvious hover/active/selected/disabled states
- semantic structure
- labels for important controls
- reduced-motion support
- interactive targets large enough to use comfortably

Focus styles:
- never remove outlines without replacing them with something stronger
- use a highly visible focus ring
- ensure sticky or floating UI does not obscure focus

Do not rely on color alone to communicate state.

---

## 9) Forms

Forms should feel simple, linear, and calm.

Rules:
- default to a single-column layout
- use top-aligned labels
- ask only for necessary information
- group related fields clearly
- make required/optional status obvious
- show validation near the field
- write helpful recovery messages

Avoid:
- two-column forms unless the inputs are short and naturally paired
- huge bordered card wrappers around each mini-section
- placeholder-only labeling

---

## 10) Empty states, loading states, and no-data moments

These states must guide the user.

Rules:
- explain why the area is empty
- tell the user what to do next
- offer the primary next action
- keep the tone calm and direct

Avoid:
- cute but useless illustrations with no instruction
- blank canvases that force guesswork

---

## 11) Visual language

### 11.1 Build a specific visual identity
Every design must have at least 3 signature choices that make it feel ownable.

Choose from:
- type system
- corner radius philosophy
- border language
- color system
- illustration style
- icon style
- screenshot framing style
- motion vocabulary
- background treatment

Do not generate generic "modern SaaS blue gradient" branding.

### 11.2 Use color as a system
Prefer a coherent palette over one loud accent color plus grayscale.

### 11.3 Use restraint in rounding and depth
Default:
- small to moderate radii
- light shadows only when needed
- borders and contrast before elevation

### 11.4 Typography should do heavy lifting
Prefer:
- crisp headline/body contrast
- disciplined line lengths
- concise copy
- clear subheads
- numbers styled for scanning when relevant

---

## 12) Marketing website instructions

When designing a homepage or landing page:

Do:
- open with a clear thesis
- show the product or outcome early
- create a scan-friendly summary path
- use section variety without breaking the overall plane
- include proof close to claims
- make CTAs obvious

Prefer:
- editorial sections
- split-screen hero layouts
- anchored product visuals
- comparison tables
- timeline/process sections
- customer proof integrated into the story

Avoid:
- 12 floating feature cards
- bento feature mosaics as the automatic solution
- giant empty hero space with vague copy
- stock "AI assistant" chat bubbles unless core to the product

---

## 13) Logged-in app instructions

When designing a product UI:

Do:
- define the primary unit of work first
- choose the right dominant view: list, table, board, calendar, document, canvas, inbox, timeline, map, inspector
- let navigation recede
- keep actions predictable
- use density intentionally
- expose shortcuts and batch actions where useful

Prefer:
- master-detail patterns
- resizable panels
- command/search bars
- filter bars
- saved views
- side inspectors
- inline edit where appropriate

Avoid:
- homepage-style marketing sections inside the app
- widget soup
- dashboard cards for everything
- floating panels disconnected from the app shell

---

## 14) Dashboard instructions

A dashboard is not a collage.

Use a dashboard only when the user truly needs an overview.
Otherwise go straight to the working view.

Dashboard rules:
- summary first, then drilldown
- every metric must lead somewhere useful
- charts need clear labels and time context
- avoid more than one visual emphasis level competing at once
- if users will act on records, show the records

Avoid:
- all-card dashboard walls
- decorative charts with no decision value
- tiny charts squeezed into pill-shaped boxes

---

## 15) AI product instructions

Do not reduce AI products to "prompt box + glowing orbs."

Prefer:
- visible system status
- clear handoff between user action and machine action
- provenance / citations / source context where relevant
- confidence and review states where relevant
- agent progress, checkpoints, and editable results
- embedded AI actions inside the real workflow

Avoid:
- chat as the only interaction pattern when a structured UI is better
- vague magic-language copy
- floating futuristic fragments disconnected from function

---

## 16) Self-check before finalizing any design

Before outputting code or mockups, verify all of the following:

### Layout
- Is the composition continuous rather than floating?
- Did I avoid default bento/card mosaics?
- Is the main work area clearly dominant?
- Is hierarchy created by structure rather than shadow?

### UX
- Is the primary task obvious in 5 seconds?
- Did I choose lists/tables instead of cards where scanning matters?
- Are actions predictable and placed consistently?
- Is the design useful at realistic content density?

### Brand
- Does this look specific to the product?
- Are there at least 3 ownable visual decisions?
- Does it avoid the generic AI-startup look?

### Accessibility
- Can a keyboard user see focus clearly?
- Are states obvious without color alone?
- Does motion have a purpose and respect reduced motion?
- Is the contrast good enough?

If any answer is "no", redesign before shipping.

---

## 17) Default fallback styles

If the prompt is vague, use one of these defaults.

### Default for B2B SaaS marketing
- editorial layout
- full-bleed sections
- left-aligned typography
- product screenshot integrated into the grid
- concise copy
- light or near-white base with restrained accent system
- almost no shadows
- no floating nav pill
- no bento features

### Default for logged-in SaaS app
- calm docked shell
- subdued sidebar
- compact top bar
- table/list first
- subtle borders
- modest radius
- high legibility
- one primary action per view
- inspector panel for details

### Default for AI workflow product
- task-oriented workspace
- structured inputs and outputs
- agent status and checkpoints
- citations or source grounding when relevant
- motion only for transitions and progress
- no sci-fi ornament unless the brand explicitly asks for it

---

## 18) One-sentence rule

**When in doubt, design a calm, brand-specific, task-first interface with continuous surfaces and strong hierarchy, not a floating island bento collage.**
