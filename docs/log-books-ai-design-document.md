# Physical Log Book Design Document + AI Prompt Pack for Amazon KDP

## Purpose

This document is for creating **physical log books** for Amazon KDP, not web apps or mobile apps.

Use it when prompting AI tools to create:

- competitor analysis reports
- stronger logbook concepts
- cover design briefs
- interior layout plans
- print-ready manuscript PDF instructions
- KDP cover PDF instructions
- final QA checklists before upload

The goal is to produce a physical logbook that is useful, original, visually competitive, and ready to turn into a KDP paperback or hardcover PDF.

---

## Core Principle

A KDP logbook is a **printed product**, not a UI screen.

Do not ask AI for:

- responsive layouts
- buttons
- hover states
- app components
- mobile screens
- web page cards

Ask AI for:

- fixed trim-size pages
- safe print margins
- gutter spacing
- cover bleed
- back/spine/front cover layout
- page templates
- handwriting space
- repeated log entry pages
- review pages
- print-safe typography
- PDF export checks

---

## Refactoring UI Principles Translated to Print

### 1. Systematize everything

Use a small set of repeated design decisions:

- same trim size
- same margins
- same line weights
- same label sizes
- same heading hierarchy
- same field spacing
- same page header/footer style
- same cover/interior personality

Avoid random field heights, random margins, random fonts, and inconsistent page spacing.

### 2. Start spacious

A logbook must be written in by hand. Start with more space than you think you need, then tighten only when the page feels too empty.

### 3. Build hierarchy

Guide the eye with:

- type size
- weight
- whitespace
- contrast
- section dividers
- field grouping

Do not make every label bold, boxed, or equally loud.

### 4. Avoid ambiguous spacing

Fields that belong together should be close. Separate sections should have clearly larger gaps.

### 5. Avoid too many borders

Do not create a page full of heavy boxes. Use light lines, whitespace, subtle dividers, and simple labels.

### 6. Design for handwriting

This is a physical product. The user needs enough room to write comfortably.

Default writing-space rules:

- single writing line: about `0.28-0.35 in` high
- compact writing line: about `0.24 in` high
- notes lines: about `0.32-0.38 in` high
- checkbox: about `0.12-0.16 in`
- rating circle: about `0.16-0.22 in`
- table row: about `0.32-0.45 in`

---

## Default KDP Working Specs

Always verify final values in KDP before publishing, but these are useful working defaults.

### Interior

Recommended default for many logbooks:

- Trim size: `6 x 9 in`
- Interior: black ink on white paper
- Interior bleed: no bleed unless artwork or background reaches the page edge
- Page count: often `100-120 pages`, adjusted by niche
- File: print-ready manuscript PDF

Useful alternatives:

- `5 x 8 in`: portable, compact
- `5.5 x 8.5 in`: journal-like
- `7 x 10 in`: more writing room
- `8.5 x 11 in`: workbook/tracker style

### Interior margins for a 100-120 page no-bleed book

Use safe working margins, not bare minimums:

- Inside/gutter: `0.45 in`
- Outside: `0.35 in`
- Top: `0.40 in`
- Bottom: `0.45 in`

For page counts above 150, increase the gutter.

### Cover

The cover must be a single full-wrap PDF:

```txt
Back cover + spine + front cover
```

Cover must account for:

- trim size
- page count
- paper type
- ink type
- spine width
- bleed
- safe zones
- barcode area
- matte or glossy finish

Do not add spine text unless the page count supports it. If unsure, leave the spine blank or verify in KDP's cover calculator/template generator.

---

## Interior Design Tokens

### Typography

Use simple print-safe fonts. Suggested directions:

- Professional: Garamond, Palatino, Baskerville-style serif
- Modern: Arial, Helvetica, Inter-style sans serif
- Warm journal: elegant serif heading + clean sans label font
- Technical logbook: clean sans serif with strong structure

Suggested interior sizes:

| Use | Size | Notes |
|---|---:|---|
| Page title | 14-18 pt | clear but not huge |
| Section title | 10-12 pt | semibold |
| Field label | 7.5-9 pt | readable and quiet |
| Helper text | 7-8 pt | use lightly |
| Page number | 7-8 pt | subtle |

Rules:

- Do not use text below 7 pt.
- Embed fonts in exported PDFs.
- Use decorative fonts only for cover or large headings.
- Do not use hard-to-read fonts for functional labels.

### Line weights

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

### Print spacing scale

| Token | Size | Use |
|---|---:|---|
| XS | 0.05 in | tiny label/line gap |
| SM | 0.10 in | tight grouping |
| MD | 0.16 in | normal field spacing |
| LG | 0.24 in | section spacing |
| XL | 0.35 in | major blocks |
| 2XL | 0.50 in | large breaks |

---

## Recommended Page Types

A strong logbook should usually include more than one repeated generic page.

### 1. Title page

Include:

- book title
- owner name
- start date
- end date

### 2. How to use this logbook

Include:

- 3-5 simple steps
- how often to fill it in
- how often to review it
- explanation of symbols, ratings, or sections

### 3. Setup or goal page

Include:

- user's goal
- starting point
- constraints
- what success looks like

### 4. Repeating log entry page

Include:

- date/session
- core tracking fields
- checklist or rating if useful
- main notes area
- observations
- next action or follow-up

### 5. Review page

Add review pages every 7, 14, 30, or 50 entries depending on the niche.

Include:

- wins
- repeated patterns
- what worked
- what needs adjustment
- next focus

### 6. Notes pages

Add a few pages at the back:

- lined
- dotted
- grid
- blank

---

## Repeating Log Entry Blueprint

Use this as a default starting point:

```txt
[PAGE TITLE / ENTRY TYPE]

Date: ____________       Time/Session: ____________

Primary fields:
Field 1: _______________     Field 2: _______________
Field 3: _______________     Field 4: _______________

Checklist / rating:
[ ] Item     [ ] Item     Rating: ○ ○ ○ ○ ○

Main notes:
____________________________________________________
____________________________________________________
____________________________________________________
____________________________________________________

Observations:
____________________________________________________
____________________________________________________

Next action / follow-up:
____________________________________________________
```

Rules:

- Fast metadata goes at the top.
- Objective tracking fields come before reflection fields.
- The largest writing space should be for the most important user input.
- End with action, follow-up, or summary.
- Do not overload one page with too many prompts.

---

## Cover Design System

The cover must sell the book in Amazon search results.

### Cover must work at thumbnail size

Priorities:

1. Title is readable.
2. Niche is obvious.
3. Buyer identity is clear.
4. Mood is different from competitors.
5. Design looks professional.

### Front cover hierarchy

Recommended order:

1. Main title
2. Niche/use-case subtitle
3. Benefit or positioning line
4. Visual motif
5. Author or brand name

### Cover style directions

Pick one clear direction.

#### Premium minimal

- strong typography
- lots of negative space
- limited colour palette
- subtle icon or linework

#### Warm guided journal

- soft neutrals
- gentle serif/sans pairing
- calm emotional tone

#### Utility/workshop

- practical grid
- strong labels
- functional, durable feeling

#### Bold category standout

- high contrast
- strong title block
- instantly readable in thumbnail

#### Illustrated niche-specific

- one strong relevant motif
- not clipart-heavy
- clear buyer signal

---

## Competitor Analysis Workflow

Collect:

- competitor cover images
- competitor interior screenshots
- titles and subtitles
- descriptions
- ratings
- positive reviews
- negative reviews
- known page counts, trim sizes, prices, and formats if available

Important rule:

Use competitors to understand the market. Do not copy their titles, covers, wording, layouts, illustrations, or unique concepts.

Analyze:

1. Cover patterns
2. Interior patterns
3. Positive review patterns
4. Negative review complaints
5. Visual gaps
6. Functional gaps
7. Emotional gaps
8. Usability gaps
9. Positioning gaps
10. Production-quality gaps

---

## Prompt 1: Competitor Analysis and Better Product Concept

```txt
I am creating a physical logbook for Amazon KDP in this niche:

[NICHE NAME]

This is a printed paperback or hardcover logbook, not a web app or mobile app.

I have attached:
- competitor cover images
- competitor interior page images
- competitor titles and subtitles
- competitor descriptions
- ratings
- positive reviews
- negative reviews
- any known page counts, trim sizes, prices, and formats

Your job is to analyze the market and design a better original logbook concept.

Do not copy any competitor's exact title, cover, layout, wording, illustration, or unique design. Use competitors only to identify buyer expectations, clichés, gaps, and opportunities.

STEP 1 — COMPETITOR COVER ANALYSIS

For each cover, assess:
- design style
- colour palette and mood
- typography choices and hierarchy
- thumbnail readability on Amazon
- who the cover visually speaks to
- what buyer identity it signals
- what all covers have in common
- visual clichés of this niche
- what feels missing from the visual market
- what would stand out while still clearly belonging to the niche

STEP 2 — COMPETITOR INTERIOR ANALYSIS

For each interior, assess:
- page types included
- fields and sections included
- layout density
- handwriting space quality
- field order and user flow
- whether instructions are clear
- whether review/summary pages exist
- what all interiors have in common
- functional clichés of this niche
- missing fields or sections a real user would want
- usability problems such as poor flow, clutter, wasted space, missing context, illogical order, or too little writing space

STEP 3 — REVIEW MINING

From positive reviews, extract:
- what buyers genuinely love and want preserved
- features or details repeatedly praised
- emotional language buyers use
- what the logbook means to them
- who they bought it for and why

From negative reviews, extract:
- repeated complaints
- missing features buyers wished existed
- layout or usability frustrations
- quality concerns
- anything that made buyers feel the product was lazy, generic, or incomplete
- unmet expectations

Organize complaints by frequency and severity.

STEP 4 — GAP MAP

Create a clear gap map:
- VISUAL GAP
- FUNCTIONAL GAP
- EMOTIONAL GAP
- USABILITY GAP
- POSITIONING GAP
- PRODUCTION GAP

STEP 5 — BETTER PRODUCT CONCEPT

Create a superior original product concept.

Include:

CONCEPT NAME AND POSITIONING
- working title
- subtitle direction
- one-line positioning statement
- target buyer
- emotional promise

COVER DIRECTION
- visual approach
- colour palette
- mood
- typography direction
- image, illustration, or motif direction
- thumbnail strategy
- what signal it sends to the buyer
- what to avoid copying from competitors

INTERIOR STRUCTURE
- recommended trim size
- recommended page count
- list of all page types
- for each page type: what it includes, why it exists, and how it improves on competitors
- repeating log entry page structure
- review/summary pages
- notes/reference pages
- layout feel: spacious vs dense, minimal vs guided
- unique pages or features no competitor currently offers

WHAT TO KEEP FROM COMPETITORS
- things the market already does well and buyers expect

WHAT TO COMPLETELY AVOID
- choices buyers dislike
- generic patterns
- confusing fields
- cramped layouts
- cover clichés

UNIQUE VALUE PROPOSITION
- one paragraph explaining why a buyer who has seen every other logbook in this niche would choose this one

Be specific and decisive. Give me a product concept I can build from directly.
```

---

## Prompt 2: Physical Logbook Design Specification

```txt
You are a senior print designer specializing in Amazon KDP logbooks.

Using the product concept below, create a full physical logbook design specification.

This is for a print-ready PDF, not a web app.

PRODUCT CONCEPT:
[PASTE PRODUCT CONCEPT]

Create a design specification with:

1. BOOK FORMAT
- trim size
- page count
- binding assumption
- black-and-white or colour interior
- bleed or no-bleed interior
- paper recommendation
- cover finish recommendation

2. DESIGN PERSONALITY
- 5-8 words describing the visual personality
- what the book should feel like in the buyer's hands
- what it must avoid

3. COVER SPEC
- front cover hierarchy
- back cover content
- spine guidance
- barcode safe area reminder
- colour palette
- typography direction
- image, illustration, or icon direction
- thumbnail readability rules
- 3 alternative cover concepts

4. INTERIOR SYSTEM
- margins and safe zones
- typography scale
- line weights
- greyscale palette
- spacing scale
- page header/footer treatment
- page numbering style
- section divider style

5. PAGE-BY-PAGE STRUCTURE
For every unique page type, specify:
- page purpose
- exact fields
- order of fields
- approximate field size
- writing line count
- spacing notes
- whether the page repeats
- how many times it repeats

6. REPEATING LOG PAGE BLUEPRINT
Give an exact layout blueprint in text form, including approximate vertical space allocation.

7. PRINT QA CHECKLIST
Include checks for margins, gutter, trim size, bleed, font embedding, line thickness, readability, page count, barcode area, cover PDF, and interior PDF.

Be concrete. Avoid vague advice.
```

---

## Prompt 3: Interior Page Layout Generator

```txt
You are designing the interior pages for a physical Amazon KDP logbook.

Use this design spec:
[PASTE DESIGN SPEC]

Create the complete interior page layout plan.

Requirements:
- Use fixed print dimensions, not responsive layout.
- Use inches or points for spacing.
- Keep all content inside safe margins.
- Use generous handwriting space.
- Avoid heavy borders and clutter.
- Use consistent typography, line weights, and spacing.
- Design for black-and-white print unless the spec says otherwise.
- Include page numbers if appropriate.

Output:
1. Full page sequence from page 1 to final page.
2. For each unique page type, provide a precise layout blueprint.
3. For repeated pages, define the master template and repeat count.
4. Provide suggested text for instructions and prompts.
5. Provide a QA checklist for the finished PDF.

Also include a compact table with page type, page count, repeats, purpose, and notes.
```

---

## Prompt 4: KDP Cover Brief Generator

```txt
You are creating a professional KDP paperback cover brief for a physical logbook.

Use this product concept and interior spec:
[PASTE PRODUCT CONCEPT AND INTERIOR SPEC]

Create a cover brief that a designer or image-generation AI can follow.

Include:

1. MARKET POSITIONING
- target buyer
- emotional promise
- what the cover must communicate in 2 seconds

2. FRONT COVER
- title hierarchy
- subtitle placement
- author/brand placement
- visual motif
- composition
- typography direction
- colour palette
- texture or pattern guidance
- thumbnail readability rules

3. BACK COVER
- headline
- short sales copy
- bullet benefits
- who it is for
- what is inside
- barcode safe area reminder

4. SPINE
- whether spine text should be included based on page count
- title/author placement guidance
- warning if page count is below KDP spine text minimum

5. TECHNICAL NOTES
- single full-wrap cover PDF
- include bleed
- keep text inside safe area
- leave barcode area clear unless own barcode is supplied
- use high-resolution images
- flatten transparencies
- embed fonts

6. THREE DISTINCT COVER DIRECTIONS
For each direction include name, mood, layout, colours, typography, motif, and why it would stand out.

Do not copy competitor designs. Create an original direction based on the market gap.
```

---

## Prompt 5: Finished PDF Review

```txt
You are reviewing a finished physical logbook PDF for Amazon KDP.

I will provide screenshots or exported page images from the cover and interior.

Review against this design spec:
[PASTE DESIGN SPEC]

Check:
- Does the cover communicate the niche clearly at thumbnail size?
- Is the title readable and well positioned?
- Does the cover avoid competitor clichés while still fitting the niche?
- Is the interior spacious enough for handwriting?
- Are margins and gutters safe?
- Are field labels readable?
- Are lines too dark, too light, too thick, or too thin?
- Is the page flow logical?
- Are review/summary pages useful?
- Is the barcode area clear?
- Are there any likely KDP rejection risks?

Output:
1. Pass/fail summary
2. Highest-risk issues
3. Design polish issues
4. Usability issues
5. KDP technical risks
6. Exact fixes to make before upload
```

---

## Final QA Checklist

### Interior

- [ ] Correct trim size.
- [ ] Fixed-size print pages, not app screens.
- [ ] Margins and gutter are safe.
- [ ] Important content is away from trim edge.
- [ ] Field labels are readable.
- [ ] Writing spaces are large enough for real handwriting.
- [ ] Line weights are consistent.
- [ ] Repeated pages are consistent.
- [ ] Review pages add real value.
- [ ] Fonts are embedded.
- [ ] No placeholder text remains.
- [ ] No copied competitor wording or layout remains.

### Cover

- [ ] Single wraparound PDF: back + spine + front.
- [ ] Correct KDP template size for trim, paper, ink, and page count.
- [ ] Bleed included.
- [ ] Text inside safe areas.
- [ ] Barcode area clear.
- [ ] No spine text if page count is too low.
- [ ] Title readable at Amazon thumbnail size.
- [ ] Images are high resolution.
- [ ] Transparencies flattened.
- [ ] Fonts embedded.
- [ ] No template marks or guide text remain.

## Final Instruction

Design the logbook as a real printed tool. It should look strong in Amazon search, feel useful when written in, solve buyer complaints found in competitor reviews, and export cleanly as KDP-ready PDFs.
