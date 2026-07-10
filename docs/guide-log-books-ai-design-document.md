# Guide + Logbook Hybrid KDP Design Document + Prompt System

## Purpose

This document is the governing design system for creating **physical guide + logbook hybrid books for Amazon KDP**.

A guide + logbook hybrid is not only a notebook, and it is not only an informational book. It teaches the reader enough to take action, then gives them structured pages to apply, track, reflect, and improve.

Use this file at the beginning of an AI session when creating any guide + logbook hybrid, regardless of niche.

Examples of possible niches:

- dog training guide + logbook
- puppy care guide + tracker
- bearded dragon care guide + logbook
- plant care guide + journal
- garden planning guide + logbook
- fitness guide + workout log
- meal planning guide + food log
- budgeting guide + spending tracker
- study guide + revision tracker
- sleep guide + sleep log
- skincare guide + routine tracker
- cannabis education guide + strain/session journal
- wine, cigar, coffee, or tea guide + tasting journal
- travel planning guide + trip log
- hobby guide + practice log

Do not get stuck on any one competitor niche. If competitor examples are dog-related, pet-related, fitness-related, or anything else, use them only to understand **hybrid structure**, **buyer expectations**, and **market gaps**. The output must be adaptable to any guide + logbook niche.

---

## How To Use This File In An AI Session

At the beginning of a new AI session, upload or provide this file:

`guide-log-books-ai-design-document.md`

Then use the prompts in this document.

The prompts reference this file by name. Do not replace those references with pasted text. The AI should understand that `guide-log-books-ai-design-document.md` is already loaded in the session and must be used as the governing design document.

Recommended starting message:

```txt
I have provided a file named guide-log-books-ai-design-document.md. Treat it as the governing design document for this session. Use it for all physical Amazon KDP guide + logbook hybrid design, competitor analysis, cover direction, guide structure, logbook structure, prompt generation, and QA review.
```

---

## Important Style Direction

The target style is **minimalist, modern, polished, practical, and easy to use**.

The guide + logbook hybrid should feel inspired by:

- Refactoring UI principles
- Tailwind-style spacing systems
- clean product design
- calm hierarchy
- strong typography
- useful whitespace
- consistent reusable page systems
- printed workbook clarity

This is still a **physical print product**, not a web app.

Do not create:

- responsive layouts
- buttons
- hover states
- app components
- mobile screens
- web page cards

Translate good UI thinking into print:

- spacing systems become print spacing and field grouping
- visual hierarchy becomes chapter/page/section hierarchy
- component consistency becomes reusable guide modules, worksheet modules, and log-entry modules
- Tailwind-style tokens become fixed print tokens for margins, type scale, line weights, spacing, callouts, and repeated page modules
- UI clarity becomes reader comprehension, handwriting usability, and low-friction action flow

### ASCII / Wireframe Warning

Any ASCII diagrams, text blueprints, or block layouts in this document are **structural references only**.

They are not the final visual style.

Do not copy the ASCII look into the final design. Convert structural blueprints into refined print layouts with clean spacing, subtle lines, modern typography, and strong hierarchy.

---

## What Makes A Good Guide + Logbook Hybrid

A strong hybrid book should do three jobs:

1. **Teach** - give the reader simple, useful guidance.
2. **Apply** - help the reader turn the guidance into action.
3. **Track** - give the reader repeatable pages to record progress, results, observations, and next steps.

The guide content should not feel like filler. The logbook pages should not feel like generic lined pages.

Every guide page should help the reader make better decisions.
Every worksheet/log page should help the reader apply or measure something from the guide.

---

## Core Working Rule

If the user provides mostly competitor evidence, the AI must still:

1. infer the niche and target buyer
2. identify whether the market expects more guide content, more tracking content, or a balanced hybrid
3. analyze competitor covers, guide pages, log pages, worksheets, and reviews
4. do additional research where useful
5. identify visual, functional, educational, emotional, usability, positioning, and production gaps
6. create a better original guide + logbook concept
7. use this file as the governing physical print guide
8. propose a modern minimalist cover direction
9. propose a practical guide structure and logbook structure
10. create prompts for generating the cover and interior
11. review the final result against usefulness, usability, and KDP-readiness

Do not stop because the input is incomplete. Make reasonable inferences and clearly label them.

Do not copy competitor covers, titles, layouts, wording, illustrations, lesson structure, worksheets, or unique concepts.

---

## Competitor Inspiration Boundary

Competitors are used for:

- understanding buyer expectations
- finding repeated page types
- finding cover clichés
- spotting missing guide content
- spotting weak tracking/logbook pages
- finding review complaints
- identifying opportunities

Competitors are not used for copying:

- titles
- subtitles
- covers
- page layouts
- lesson wording
- icons/illustrations
- unique frameworks
- exact field names
- exact guide structure

If competitor examples are from one niche, extract only the transferable patterns.

Example transferable patterns:

- step-by-step beginner guide
- quick-start checklist
- weekly tracker
- symptom/progress log
- training/session log
- reflection page
- troubleshooting page
- goal-setting worksheet
- review spread
- resource/reference page

Example non-transferable details:

- dog-specific commands
- pet-specific terminology
- niche-specific illustrations
- exact competitor fields
- competitor product names

---

## How To Use With Competitor Screenshots Only

When the user uploads only competitor screenshots and gives little explanation, follow this process:

1. **Identify what is visible**
   - visible titles and subtitles
   - niche indicators
   - cover styles
   - guide sections
   - worksheet sections
   - log-entry fields
   - review/checklist pages
   - buyer-use clues

2. **Infer the niche and hybrid type**
   - likely niche
   - likely buyer
   - confidence level
   - guide-heavy, log-heavy, or balanced hybrid
   - evidence supporting the inference

3. **Research to fill gaps**
   - common beginner questions
   - common mistakes in the niche
   - common buyer complaints
   - common field/page expectations
   - common trim/page-count patterns when useful
   - terminology used by real buyers

4. **Extract transferable structure**
   - what type of guide pages competitors use
   - what type of log pages competitors use
   - what review pages or checklists are useful
   - what page flow makes sense

5. **Do not over-copy**
   - competitor material is for analysis only
   - create a new product angle
   - create original cover and page structures

6. **Produce build-ready outputs**
   - product concept
   - guide structure
   - logbook structure
   - cover direction
   - interior page plan
   - generation prompts
   - QA checklist

---

## Physical KDP Working Assumptions

Always verify final specs in KDP before upload. Use these as sensible working assumptions.

### Common Hybrid Format

Default interior recommendation:

- Trim size: `6 x 9 in`
- Interior: black ink on white paper
- Interior style: no bleed unless artwork or background reaches the edge
- Page count: commonly `120-180 pages`, adjusted by niche and guide depth
- Cover: full wraparound PDF with bleed
- Interior: separate manuscript PDF

The hybrid format usually needs more pages than a pure logbook because it includes educational guide content, worksheets, and repeated log pages.

Useful trim alternatives:

- `5 x 8 in`: compact pocket guide + short log
- `5.5 x 8.5 in`: journal-like and balanced
- `6 x 9 in`: default for most guide + logbook hybrids
- `7 x 10 in`: better for detailed worksheets and trackers
- `8.5 x 11 in`: workbook/training-manual feel

### Paperback vs Hardcover

Default recommendation:

- **Paperback first** for most guide + logbook hybrids.
- **Hardcover only** when the niche benefits from giftability, keepsake value, premium positioning, or long-term archival use.

Paperback is better for testing, pricing, and most functional guide + tracker products.

Hardcover can work for premium journals, keepsake trackers, baby/pet milestone books, luxury hobby journals, or giftable guides.

### Interior Margin Defaults

For a `6 x 9 in`, no-bleed, 120-180 page hybrid:

- Inside/gutter: `0.50 in` working value
- Outside: `0.35-0.40 in`
- Top: `0.40-0.45 in`
- Bottom: `0.45-0.50 in`

For page counts above 180, increase the gutter.

Never place important text, boxes, page numbers, icons, or worksheet fields close to the trim edge.

### Cover Technical Rules

The cover should be a single full-wrap PDF:

```txt
Back cover + spine + front cover
```

The cover must account for:

- trim size
- page count
- paper type
- ink type
- spine width
- bleed
- safe zones
- barcode area
- matte or glossy finish

Do not add spine text unless the page count supports it. If uncertain, omit spine text or verify in KDP's cover calculator/template generator.

---

## Hybrid Content Ratio Models

Choose a ratio based on the niche and buyer expectation.

### 1. Guide-Heavy Hybrid

Best for beginner education or complex topics.

Suggested ratio:

- 60-70% guide content
- 20-30% worksheets
- 10-20% logs/trackers

Useful for:

- beginner training guides
- care guides
- educational hobby guides
- step-by-step programs
- wellness guides

### 2. Balanced Hybrid

Best default for most KDP guide + logbooks.

Suggested ratio:

- 35-45% guide content
- 20-30% worksheets/checklists
- 30-40% log/tracker pages

Useful for:

- pet care/training
- fitness programs
- study systems
- gardening journals
- budgeting systems
- routine-based guides

### 3. Log-Heavy Hybrid

Best when the buyer mainly wants tracking but needs a short guide to use it well.

Suggested ratio:

- 10-25% guide content
- 10-20% worksheets/reference pages
- 60-75% log/tracker pages

Useful for:

- daily trackers
- session logs
- symptom logs
- food logs
- workout logs
- tasting journals

---

## Print Design Philosophy

### 1. Teach, Then Apply

Guide content should lead into action.

Good flow:

```txt
Concept -> Example -> Checklist -> Worksheet -> Log Entry -> Review
```

Avoid long passive reading sections with no practical follow-through.

### 2. Keep Guide Pages Skimmable

Guide pages should use:

- short sections
- clear headings
- callout boxes
- numbered steps
- quick-start summaries
- mistake warnings
- simple examples
- action prompts

Avoid dense textbook pages.

### 3. Start Spacious

A guide + logbook hybrid must be readable and writable.

Give guide text breathing room.
Give worksheets and log pages enough handwriting space.

### 4. Use Reusable Page Modules

Build pages from consistent modules:

- chapter intro block
- quick tip block
- warning block
- checklist block
- worksheet block
- log-entry block
- reflection block
- review block

### 5. Avoid Too Many Borders

Do not create heavy boxed pages. Use light lines, whitespace, subtle dividers, and clean grouping.

### 6. Make The Hybrid Feel Intentional

The reader should never feel like the book is half random guide pages and half generic blank pages.

Each log page should connect to the guide system.

---

## Interior Design Tokens

### Typography

Use simple print-safe fonts.

Suggested directions:

- Professional: Garamond, Palatino, Baskerville-style serif
- Modern: Arial, Helvetica, Inter-style sans serif
- Warm guided journal: elegant serif heading + clean sans label font
- Technical guide: clean sans serif with strong structure
- Premium hobby guide: restrained serif + minimal sans labels

Suggested interior sizes:

| Use | Size | Notes |
|---|---:|---|
| Chapter title | 16-22 pt | use sparingly |
| Page title | 14-18 pt | clear but not huge |
| Section title | 10-12 pt | semibold |
| Body text | 8.5-10 pt | readable and compact |
| Field label | 7.5-9 pt | readable and quiet |
| Helper text | 7-8 pt | use lightly |
| Page number | 7-8 pt | subtle |

Rules:

- Do not use text below 7 pt.
- Embed fonts in exported PDFs.
- Use decorative fonts only for cover or large headings.
- Do not use hard-to-read fonts for functional labels.

### Line Weights

| Use | Weight |
|---|---:|
| faint writing lines | 0.25 pt |
| normal writing lines | 0.5 pt |
| section dividers | 0.75 pt |
| rare emphasis | 1 pt |

Greyscale defaults:

- Main text: `#222222`
- Secondary text: `#666666`
- Writing lines: `#D9D9D9`
- Dividers: `#B8B8B8`
- Callout background: very light grey, around `#F3F3F3` if printing quality supports it

### Print Spacing Scale

| Token | Size | Use |
|---|---:|---|
| XS | 0.05 in | tiny label/line gap |
| SM | 0.10 in | tight grouping |
| MD | 0.16 in | normal field spacing |
| LG | 0.24 in | section spacing |
| XL | 0.35 in | major blocks |
| 2XL | 0.50 in | chapter/page breaks |

---

## Recommended Page Types

A strong hybrid should combine educational, action, and tracking pages.

### 1. Title Page

Include:

- book title
- owner name
- start date
- end date

### 2. How To Use This Book

Include:

- how to read the guide sections
- when to use the worksheets
- how often to fill in logs
- how often to review progress
- explanation of symbols, ratings, and repeated sections

### 3. Quick Start Page

A one-page fast path for readers who want to begin immediately.

Include:

- 3-7 starting steps
- what to complete first
- where to begin logging
- what to review after the first week/session

### 4. Foundation Guide Pages

Short educational pages that explain the core concepts.

Use:

- short paragraphs
- bullets
- examples
- warning callouts
- quick tips
- action prompts

### 5. Checklist Pages

Useful for readiness, setup, preparation, maintenance, or review.

### 6. Worksheet Pages

A worksheet helps the reader apply guide content.

Possible worksheets:

- goal setting
- baseline assessment
- plan builder
- routine builder
- decision tree
- troubleshooting worksheet
- progress review
- habit/routine planner

### 7. Reference Pages

Reference pages should be useful at a glance.

Examples:

- glossary
- measurement guide
- symptom/issue guide
- routine examples
- rating scale explanation
- milestone guide
- troubleshooting table

### 8. Repeating Log Entry Pages

Include if the niche benefits from tracking.

Possible fields:

- date/session
- context
- objective fields
- rating/checklist
- main notes
- outcome
- next action

### 9. Review Pages

Add review pages after meaningful intervals:

- weekly
- monthly
- every 7 entries
- every 14 entries
- every 30 entries
- after each program phase

Include:

- wins
- patterns
- what worked
- what needs adjustment
- next focus

### 10. Notes Pages

Add a small number of useful notes pages at the back.

Avoid padding the book with too many blank pages.

---

## Hybrid Page Flow Patterns

### Beginner Program Flow

```txt
Intro -> Quick Start -> Foundation Lessons -> Worksheets -> Logs -> Reviews -> Reference
```

### Tracker With Short Guide Flow

```txt
Intro -> Quick Guide -> Setup Worksheet -> Repeating Logs -> Reviews -> Notes
```

### Phase-Based Program Flow

```txt
Intro -> Phase 1 Guide -> Phase 1 Worksheets -> Phase 1 Logs -> Phase 1 Review -> Phase 2...
```

### Reference-First Flow

```txt
Intro -> Reference Guide -> Decision Tables -> Logs -> Reviews -> Troubleshooting
```

These are structural flows only. Do not copy the blocky appearance into final design.

---

## Repeating Log Entry Structural Blueprint

This is a wireframe only. Convert it into a refined modern print layout.

```txt
[LOG ENTRY TITLE]

Date: ____________       Session/Context: ____________

Before / Setup:
Field 1: _______________     Field 2: _______________

Action / Observation:
Field 3: _______________     Field 4: _______________

Checklist / rating:
[ ] Item     [ ] Item     Rating: ○ ○ ○ ○ ○

Main notes:
____________________________________________________
____________________________________________________
____________________________________________________

Outcome:
____________________________________________________

Next action:
____________________________________________________
```

Rules:

- Fast metadata goes at the top.
- Setup/context comes before outcome.
- The largest writing space should be for the most important user input.
- End with action, follow-up, or summary.
- Do not overload one page with too many prompts.
- Do not keep the final page blocky or ASCII-like.

---

## Guide Page Structural Blueprint

This is a wireframe only.

```txt
[CHAPTER / GUIDE TOPIC]

Short explanation:
2-4 short paragraphs or bullet blocks.

Key idea:
[short highlighted callout]

Common mistakes:
- Mistake 1
- Mistake 2
- Mistake 3

Try this:
1. Step one
2. Step two
3. Step three

Apply it:
Go to the related worksheet/log page and record your starting point.
```

Rules:

- Keep guide pages short and actionable.
- Avoid long textbook blocks.
- Every guide page should connect to an action, worksheet, checklist, or log page.

---

## Cover Design System

The cover must communicate both guide value and logbook utility.

### Thumbnail Priorities

1. Title is readable.
2. Niche is obvious.
3. Buyer understands it is both a guide and a logbook.
4. Mood is different from competitors.
5. Design looks professional.

### Front Cover Hierarchy

Recommended order:

1. Main title
2. Hybrid signal: `Guide + Logbook`, `Guide & Tracker`, `Field Guide + Journal`, `Workbook + Log`, etc.
3. Benefit or positioning line
4. Visual motif
5. Author or brand name

### Cover Style Directions

Pick one clear direction.

#### Premium Minimal

- strong typography
- lots of negative space
- limited colour palette
- subtle icon or linework

#### Warm Guided Journal

- soft neutrals
- gentle serif/sans pairing
- calm emotional tone

#### Practical Field Guide

- organized reference feel
- subtle labels or specimen/diagram influence
- useful but polished

#### Utility / Workbook

- practical grid
- strong labels
- functional, durable feeling

#### Bold Category Standout

- high contrast
- strong title block
- instantly readable in thumbnail

#### Illustrated Niche-Specific

- one strong relevant motif
- not clipart-heavy
- clear buyer signal

---

## Recommended Workflow

### Step 0 - Master Orchestrator

Use first when starting from competitor screenshots/reviews and you want the AI to run the whole strategy process.

Output:

- niche understanding
- research summary
- competitor analysis
- review mining
- gap map
- hybrid concept
- physical design spec
- guide structure
- logbook structure
- cover directions
- generation prompts
- risks and recommendations

### Step 1 - Competitor Analysis

Use when you want deep analysis before product design.

### Step 2 - Hybrid Product Concept + Physical Design Spec

Use after competitor analysis.

### Step 3 - Guide + Interior Page Layout Plan

Use after the concept is clear.

### Step 4 - Cover Brief + Generation Prompts

Use after the concept, page count, and trim size are known.

### Step 5 - Final QA Review

Use after cover/interior drafts or PDFs exist.

---

# Prompt 0 - Master Orchestrator

Use this first when you want the AI to take competitor evidence and turn it into a complete original KDP guide + logbook hybrid direction.

```txt
You are helping me create a physical guide + logbook hybrid product for Amazon KDP.

This is a printed guide + logbook hybrid, not a web app or mobile app.

A file named guide-log-books-ai-design-document.md has been provided at the beginning of this session. Treat that file as the governing design document for this entire task. Do not ask me to paste it again.

I may provide very little context beyond competitor material such as:
- competitor cover images
- competitor interior images
- competitor guide pages
- competitor worksheet pages
- competitor log pages
- competitor titles or descriptions
- positive reviews
- negative reviews
- occasional ratings, page counts, trim sizes, or prices

Your job is to do the product thinking, research, competitor analysis, educational structure planning, print-design planning, and prompt-generation work needed to create a better original guide + logbook hybrid.

Important visual direction:
- The final product should feel modern, minimalist, polished, and practical.
- Use Refactoring UI-style principles translated into print: strong hierarchy, consistent spacing, restrained colour, thoughtful whitespace, clear grouping, and useful structure.
- Use Tailwind-style design thinking as inspiration for systematic spacing, typography, and component consistency, but do not design a web app.
- ASCII diagrams or block layouts are only rough structural wireframes. Do not copy the ASCII look. Convert them into refined print layouts.

Research requirement:
Do additional research as needed. If the uploaded material is incomplete, infer what you can, research what matters, and clearly label assumptions.

Originality requirement:
Do not copy competitor covers, titles, layouts, wording, illustrations, guide frameworks, worksheets, or unique concepts. Use competitor material only to identify buyer expectations, visual clichés, educational gaps, functional gaps, review complaints, and product opportunities.

PHASE 1 - UNDERSTAND THE NICHE
- infer the niche and target buyer
- identify the real-world job this guide + logbook helps with
- identify who would buy it and why
- identify whether it should be guide-heavy, log-heavy, or balanced
- identify whether it is more practical, emotional, professional, hobbyist, wellness, technical, or giftable
- label assumptions clearly

PHASE 2 - RESEARCH
Research what is needed to strengthen the product direction:
- common beginner questions in this niche
- common mistakes or pain points
- common title/subtitle patterns
- common cover styles and visual clichés
- common trim sizes and page counts
- typical buyer expectations
- repeated review complaints in this product category
- useful guide sections, worksheets, checklists, reference pages, and log fields
- KDP-related production assumptions if relevant

PHASE 3 - COMPETITOR COVER ANALYSIS
Analyze the provided covers:
- design style
- colour palette and mood
- typography and hierarchy
- thumbnail readability
- whether the cover clearly signals guide + logbook value
- buyer identity signal
- niche clichés
- what looks generic or overused
- what is missing visually
- what would stand out while still belonging to the niche

PHASE 4 - COMPETITOR INTERIOR ANALYSIS
Analyze the provided interiors:
- guide sections
- worksheet pages
- checklist pages
- reference pages
- log entry pages
- page flow
- writing space quality
- layout density
- prompt clarity
- usability problems
- what feels lazy, generic, cramped, or incomplete
- what real users still need

PHASE 5 - REVIEW MINING
From positive reviews, extract:
- what buyers love
- features they want preserved
- guide content they value
- log/tracker content they value
- emotional language
- gift/use-case patterns
- quality signals

From negative reviews, extract:
- repeated complaints
- missing guide content
- missing logbook fields
- layout frustrations
- unmet expectations
- quality issues
- signs the book feels generic or low effort

Group complaints by frequency and severity.

PHASE 6 - GAP MAP
Create:
- visual gap
- educational gap
- functional gap
- emotional gap
- usability gap
- positioning gap
- production-quality gap

PHASE 7 - BETTER HYBRID CONCEPT
Create a superior original concept:
- working title direction
- subtitle direction
- target buyer
- one-line positioning
- emotional promise
- unique value proposition
- recommended guide/logbook ratio
- what to keep from competitors
- what to avoid completely

PHASE 8 - PHYSICAL DESIGN SPEC
Using guide-log-books-ai-design-document.md, create:
- recommended trim size
- recommended page count
- black-and-white or colour interior recommendation
- bleed/no-bleed recommendation
- paperback/hardcover recommendation
- margin and gutter assumptions
- typography direction
- line-weight direction
- spacing direction
- page numbering direction
- guide page types
- worksheet page types
- repeating log page blueprint
- review/reference pages

PHASE 9 - GUIDE STRUCTURE
Create:
- guide chapters or sections
- purpose of each guide section
- key lessons or concepts
- quick-start page
- common mistakes page if useful
- reference pages if useful
- how each guide section connects to a worksheet or log page

PHASE 10 - LOGBOOK STRUCTURE
Create:
- full list of logbook page types
- recommended page order
- repeated page count
- what each page includes
- why each page exists
- how each page solves buyer complaints or improves usability
- what pages should not be included because they add filler

PHASE 11 - COVER DIRECTION
Create:
- 2 to 3 original cover directions
- recommended strongest direction
- front cover hierarchy
- back cover content direction
- spine guidance
- thumbnail strategy
- colour palette
- typography direction
- motif/illustration/photo direction

PHASE 12 - GENERATION PROMPTS
Create prompts I can use with an image/design AI for:
1. front cover concept
2. full wraparound KDP cover brief
3. guide page layout concept
4. worksheet page layout concept
5. repeated log-entry page
6. final QA review

FINAL OUTPUT FORMAT
Return the answer in this order:
1. niche understanding
2. research summary
3. competitor cover analysis
4. competitor interior analysis
5. review mining summary
6. gap map
7. better hybrid concept
8. physical design spec
9. guide structure
10. logbook structure
11. cover directions
12. generation prompts
13. final risks and recommendations

Be specific, decisive, and practical. Build something I can actually publish.
```

---

# Prompt 1 - Competitor Analysis + Hybrid Gap Map

Use this when you want to deeply understand the market before deciding the product concept.

```txt
I am creating a physical guide + logbook hybrid for Amazon KDP.

This is a printed guide + logbook hybrid, not a web app or mobile app.

A file named guide-log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

I have attached some or all of the following:
- competitor cover images
- competitor interior images
- competitor guide pages
- competitor worksheet pages
- competitor log pages
- competitor reviews
- competitor titles, descriptions, ratings, prices, trim sizes, or page counts

Use the attached material and do additional research where useful.

Important:
- Use competitor products only for analysis.
- Do not copy titles, covers, layouts, wording, illustrations, frameworks, worksheets, or unique design ideas.
- If examples are from a specific niche, extract transferable hybrid patterns instead of copying niche-specific content.
- ASCII or text layout examples are structural only; the final design direction should be modern, minimalist, and polished.

STEP 1 - INFER THE NICHE
- What niche does this appear to be?
- Who is the likely buyer?
- What job does the guide + logbook help them do?
- Should the product be guide-heavy, log-heavy, or balanced?
- What assumptions are you making?

STEP 2 - RESEARCH THE MARKET
Research what is needed to strengthen the analysis:
- common beginner questions
- common mistakes
- common product claims
- common cover patterns
- common guide structures
- common worksheet/log structures
- buyer expectations
- review complaints
- page count and trim-size patterns if relevant

STEP 3 - COVER ANALYSIS
For each competitor cover, assess:
- visual style
- colour palette
- typography hierarchy
- thumbnail readability
- guide + logbook signal
- buyer signal
- niche clichés
- what feels generic
- what feels strong
- what is missing visually

STEP 4 - INTERIOR ANALYSIS
For each competitor interior, assess:
- guide pages
- worksheet pages
- log pages
- checklists
- reference pages
- field usefulness
- layout density
- handwriting space
- flow and order
- instruction quality
- missing sections
- usability problems
- whether it feels useful or like filler

STEP 5 - REVIEW MINING
From positive reviews:
- what buyers love
- what must be preserved
- repeated praise
- emotional language

From negative reviews:
- repeated complaints
- missing guide content
- missing worksheet/log fields
- layout frustrations
- unmet expectations
- quality concerns
- signs of generic or lazy design

STEP 6 - GAP MAP
Create:
- visual gap
- educational gap
- functional gap
- emotional gap
- usability gap
- positioning gap
- production-quality gap

STEP 7 - OPPORTUNITY SUMMARY
Give me the biggest product opportunities in priority order.

Be specific and decisive.
```

---

# Prompt 2 - Better Hybrid Product Concept + Physical Design Spec

Use this after Prompt 1.

```txt
Using the competitor analysis and gap map below, create a better original physical guide + logbook hybrid concept for Amazon KDP.

This is a printed product, not a web app.

A file named guide-log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

Design style requirement:
- modern minimalist
- polished
- practical
- clear hierarchy
- skimmable guide sections
- useful worksheets/log pages
- Refactoring UI-inspired spacing and visual discipline translated into print
- Tailwind-like design consistency translated into fixed print tokens
- no ASCII/blocky final aesthetic

COMPETITOR ANALYSIS AND GAP MAP:
[PASTE OUTPUT FROM PROMPT 1]

Create:

1. PRODUCT POSITIONING
- working title direction
- subtitle direction
- target buyer
- one-line positioning
- emotional promise
- unique value proposition
- guide-heavy, log-heavy, or balanced hybrid recommendation

2. WHAT TO KEEP
- features buyers already like
- guide expectations that should remain
- logbook expectations that should remain

3. WHAT TO AVOID
- competitor clichés
- review complaints
- generic low-content patterns
- dense textbook-style guide pages
- cramped or confusing worksheet/log layouts

4. PHYSICAL FORMAT
- trim size recommendation
- page count recommendation
- black-and-white or colour interior
- bleed/no-bleed interior
- paperback/hardcover assumption
- matte/gloss cover recommendation

5. COVER DIRECTION
- visual style
- colour palette
- typography direction
- motif/illustration/photo direction
- thumbnail strategy
- how to communicate guide + logbook clearly
- what makes it different from competitors

6. INTERIOR DESIGN SYSTEM
- margin and gutter assumptions
- type scale direction
- line-weight direction
- spacing rhythm
- callout treatment
- worksheet treatment
- log-entry treatment
- page numbering treatment
- section heading treatment
- handwriting-space rules

7. GUIDE STRUCTURE
- guide chapters/sections
- purpose of each section
- key lessons
- quick-start content
- reference/checklist content
- how each section connects to action

8. LOGBOOK STRUCTURE
- all log/worksheet/review page types
- purpose of each page type
- fields on each page type
- how many times each page repeats
- what buyer complaint or use-case each page solves

9. REPEATING PAGE BLUEPRINTS
Provide structural blueprints for:
- guide page
- worksheet page
- log entry page
- review page

Remember: any ASCII is only a wireframe. The final style should be clean, modern, and print-polished.

10. FINAL BUILD NOTES
- what to generate next
- risks to watch for
- QA checks before PDF export
```

---

# Prompt 3 - Guide + Logbook Interior Page Layout Plan

Use this when the concept and physical spec are clear.

```txt
Create a complete interior layout plan for this physical Amazon KDP guide + logbook hybrid.

A file named guide-log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

Use the product concept and design spec below:
[PASTE OUTPUT FROM PROMPT 2]

Important style requirement:
- modern minimalist print layout
- clean spacing
- subtle lines
- refined typography
- skimmable guide content
- enough handwriting space
- no heavy boxes unless functionally necessary
- no ASCII/blocky final aesthetic

Create:

1. INTERIOR FORMAT SUMMARY
- trim size
- page count
- guide/logbook ratio
- bleed/no-bleed
- margin/gutter assumptions
- black-and-white or colour interior

2. FULL PAGE SEQUENCE
List the exact page sequence from page 1 to the final page.

3. GUIDE PAGE TYPES
For each guide page type, specify:
- purpose
- section heading
- body text density
- callouts
- checklists
- examples
- action prompt
- related worksheet/log page

4. WORKSHEET PAGE TYPES
For each worksheet type, specify:
- purpose
- fields
- field order
- writing space
- connection to guide content

5. LOG PAGE TYPES
For each log page type, specify:
- purpose
- fields
- field order
- approximate writing space
- line count or writing area size
- spacing notes
- repeat count

6. REVIEW / SUMMARY PAGES
Specify where review pages appear and what they ask.

7. REFERENCE PAGES
Specify any glossary, troubleshooting, quick-reference, measurement, routine, or example pages.

8. MODERN PRINT STYLE NOTES
Explain how to make the book feel minimal and polished, not generic, cramped, or textbook-heavy.

9. INTERIOR QA CHECKLIST
Check margins, gutter, readability, handwriting space, line weights, repeated-page consistency, guide/log flow, page count, and placeholder removal.
```

---

# Prompt 4 - KDP Cover Brief + Generation Prompts

Use this after the concept, interior structure, trim size, and page count are known.

```txt
Create a professional KDP cover brief and cover-generation prompts for this physical guide + logbook hybrid.

A file named guide-log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

Use the product concept and interior spec below:
[PASTE OUTPUT FROM PROMPT 2 OR 3]

Important style requirement:
- modern minimalist
- strong Amazon thumbnail readability
- refined typography
- clear niche signal
- clear guide + logbook signal
- original, not derivative of competitors
- avoid generic Canva-template energy
- avoid copying competitor colours, composition, or motifs too closely

Create:

1. MARKET POSITIONING
- target buyer
- emotional promise
- what the cover must communicate in 2 seconds
- how to signal both guide value and logbook utility

2. FRONT COVER BRIEF
- title hierarchy
- subtitle placement
- guide + logbook signal placement
- author/brand placement
- motif or image direction
- composition
- typography direction
- colour palette
- texture or pattern guidance
- thumbnail readability rules

3. BACK COVER BRIEF
- headline direction
- short sales copy direction
- bullet benefit direction
- who it is for
- what guide content is inside
- what logbook/tracker content is inside
- barcode safe-area reminder

4. SPINE GUIDANCE
- whether spine text should be included
- title/author placement guidance
- warning if page count may be too low for spine text

5. THREE COVER DIRECTIONS
For each direction include:
- name
- mood
- layout
- colours
- typography
- motif
- why it stands out

6. IMAGE/DESIGN AI PROMPTS
Create:
- safe market-fit prompt
- differentiated modern prompt
- bold standout prompt
- negative prompt / avoid list

7. COVER QA CHECKLIST
Check thumbnail readability, guide + logbook clarity, originality, safe areas, barcode area, hierarchy, and print-readiness.
```

---

# Prompt 5 - Final PDF / Screenshot QA Review

Use this after the cover or interior has been generated.

```txt
You are reviewing a finished or near-finished physical guide + logbook hybrid for Amazon KDP.

I will provide screenshots, exported page images, or PDFs of the cover and interior.

A file named guide-log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

Use the product concept and design spec below as the product-specific standard:
[PASTE PRODUCT CONCEPT / DESIGN SPEC]

Review for:

1. MARKET FIT
- does the product clearly fit the niche?
- does it speak to the right buyer?
- does it solve the original competitor gaps?
- is the guide/logbook balance right?

2. COVER QUALITY
- is the title readable at Amazon thumbnail size?
- is the hierarchy strong?
- does the cover clearly signal guide + logbook value?
- is the cover original but still niche-relevant?
- does it avoid competitor clichés?
- does it feel modern, minimalist, and polished?

3. GUIDE CONTENT QUALITY
- is the guide content useful and actionable?
- is it skimmable?
- does it avoid dense textbook blocks?
- does each guide section connect to an action, worksheet, or log page?
- are callouts/checklists helpful rather than filler?

4. LOGBOOK / WORKSHEET USABILITY
- is there enough handwriting space?
- are fields useful and logically ordered?
- are there too many boxes or heavy borders?
- are labels readable?
- do repeated pages feel consistent?
- do setup/review/reference pages add real value?

5. PRINT DESIGN QUALITY
- margins look safe
- gutter looks safe
- line weights are not too dark or too faint
- typography is readable
- page numbers are consistent
- no placeholder text remains
- no ASCII/blocky styling accidentally carried into the final design

6. KDP RISK CHECK
- trim size consistency
- bleed/safe area concerns
- barcode area concern
- spine text concern
- image resolution concern
- font embedding concern

Output:
1. pass/fail summary
2. highest-risk issues
3. design polish issues
4. guide-content issues
5. worksheet/log usability issues
6. KDP technical risks
7. exact fixes before upload
8. final recommendation: ready, almost ready, or needs redesign
```

---

## Final QA Checklist

### Guide Content

- [ ] Guide pages are useful, not filler.
- [ ] Guide pages are skimmable.
- [ ] Dense textbook blocks are avoided.
- [ ] Each guide section leads to an action, worksheet, checklist, or log page.
- [ ] Reference pages are useful at a glance.
- [ ] The guide/logbook ratio matches the niche.

### Worksheets + Logs

- [ ] Fields are useful and specific.
- [ ] Writing spaces are large enough for real handwriting.
- [ ] Page flow is logical.
- [ ] Review pages add value.
- [ ] Repeated pages are consistent.
- [ ] No generic filler pages dominate the book.

### Interior Print Design

- [ ] Correct trim size.
- [ ] Fixed-size print pages, not app screens.
- [ ] Margins and gutter are safe.
- [ ] Important content is away from trim edge.
- [ ] Field labels are readable.
- [ ] Line weights are consistent.
- [ ] Fonts are embedded.
- [ ] No placeholder text remains.
- [ ] No copied competitor wording or layout remains.
- [ ] No ASCII/blocky styling remains in final design.

### Cover

- [ ] Single wraparound PDF: back + spine + front.
- [ ] Correct KDP template size for trim, paper, ink, and page count.
- [ ] Bleed included where needed.
- [ ] Text inside safe areas.
- [ ] Barcode area clear.
- [ ] No spine text if page count is too low.
- [ ] Title readable at Amazon thumbnail size.
- [ ] Cover clearly signals guide + logbook value.
- [ ] Cover feels modern, minimalist, and niche-relevant.
- [ ] Images are high resolution.
- [ ] Transparencies flattened.
- [ ] Fonts embedded.
- [ ] No template marks or guide text remain.

---

## Final Instruction

Use this system to create a **better physical guide + logbook hybrid**, not a generic low-content notebook and not a dense textbook.

The final product should:

- teach enough to be useful
- help the reader take action
- provide structured pages for tracking and reflection
- look strong in Amazon search
- feel useful when written in
- solve buyer complaints found in competitor reviews
- use a consistent modern minimalist print design system
- avoid copying competitors
- avoid web-app thinking
- avoid ASCII/blocky final styling
- export cleanly as KDP-ready cover and interior PDFs
