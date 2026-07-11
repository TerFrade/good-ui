## Important Style Direction

The target style is **minimalist, polished, and practical**.

The logbook should feel inspired by:

- Refactoring UI principles
- Tailwind-style spacing systems
- clean product design
- calm hierarchy
- strong typography
- thoughtful whitespace
- useful structure

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
- visual hierarchy becomes cover/title/section hierarchy
- component consistency becomes reusable page templates
- Tailwind-style tokens become fixed print tokens for margins, line weights, typography, and repeated page modules
- UI clarity becomes handwriting usability and low-friction page flow

### ASCII / Wireframe Warning

Any ASCII diagrams, text blueprints, or block layouts in this document are **structural references only**.

They are not the final visual style.

Do not copy the ASCII look into the final design. Convert structural blueprints into refined print layouts with clean spacing, subtle lines, typography, and strong hierarchy.

---

## Core Working Rule

If the user provides mostly competitor evidence, the AI must still:

1. infer the niche and target buyer
2. analyze covers, interiors, and reviews
3. do additional research where useful
4. identify visual, functional, emotional, usability, positioning, and production gaps
5. create a better original logbook concept
6. use this file as the governing physical print guide
7. propose a modern minimalist cover direction
8. propose a practical interior structure
9. create prompts for generating the cover and interior
10. review the final result against usability and KDP-readiness

Do not stop because the input is incomplete. Make reasonable inferences and clearly label them.

Do not copy competitor covers, titles, layouts, wording, illustrations, or unique concepts.

---

## How To Use With Competitor Screenshots Only

When the user only uploads images and gives little explanation, follow this approach:

1. **Identify what is visible**
   - visible titles
   - niche indicators
   - cover styles
   - interior fields
   - repeated page structures
   - buyer-use clues

2. **Infer the niche**
   - state the likely niche
   - state confidence level
   - list what evidence supports the inference

3. **Research to fill gaps**
   - search for common niche expectations
   - research common buyer complaints
   - check common trim/page-count patterns when relevant
   - research terminology used by real buyers

4. **Do not over-copy**
   - competitor material is for analysis only
   - create a new product angle
   - create original cover and page structures

5. **Use this file**
   - physical print design rules come from `log-books-ai-design-document.md`
   - use minimalist style, not ASCII/blocky styling

6. **Produce build-ready outputs**
   - product concept
   - cover direction
   - interior page list
   - prompt pack for cover/interior generation
   - QA checklist

---

## Physical KDP Working Assumptions

Always verify final specs in KDP before upload. Use these as sensible working assumptions.

### Common Logbook Format

Default interior recommendation:

- Trim size: `6 x 9 in`
- Interior: black ink on white paper
- Interior style: no bleed unless artwork or background reaches the edge
- Page count: commonly `100-120 pages`, adjusted by niche
- Cover: full wraparound PDF with bleed
- Interior: separate manuscript PDF

Useful trim alternatives:

- `5 x 8 in`: compact and portable
- `5.5 x 8.5 in`: journal-like and balanced
- `7 x 10 in`: better for detailed trackers
- `8.5 x 11 in`: workbook/tracker feel

### Interior Margin Defaults

For a `6 x 9 in`, no-bleed, 100-120 page logbook:

- Inside/gutter: `0.45 in` working value
- Outside: `0.35 in`
- Top: `0.40 in`
- Bottom: `0.45 in`

For page counts above 150, increase the gutter.

Never place important text, boxes, page numbers, or icons close to the trim edge.

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

## Print Design Philosophy

### 1. Systematize Everything

Use a small set of repeated decisions:

- same trim size
- same margins
- same line weights
- same label sizes
- same heading hierarchy
- same field spacing
- same page header/footer style
- same cover/interior personality

Avoid random field heights, random margins, random fonts, and inconsistent spacing.

### 2. Start Spacious

A logbook must be written in by hand. Start with more space than expected, then tighten only where needed.

### 3. Build Hierarchy

Guide the eye with:

- type size
- weight
- whitespace
- contrast
- section dividers
- field grouping

Do not make every label bold, boxed, or equally loud.

### 4. Avoid Ambiguous Spacing

Fields that belong together should be close. Separate sections should have clearly larger gaps.

### 5. Avoid Too Many Borders

Do not create a page full of heavy boxes. Use light lines, whitespace, subtle dividers, and simple labels.

### 6. Design For Handwriting

Default writing-space rules:

- single writing line: about `0.28-0.35 in` high
- compact writing line: about `0.24 in` high
- notes lines: about `0.32-0.38 in` high
- checkbox: about `0.12-0.16 in`
- rating circle: about `0.16-0.22 in`
- table row: about `0.32-0.45 in`

---

## Interior Design Tokens

### Typography

Use simple print-safe fonts.

Suggested directions to think of niche font styles:

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

### Print Spacing Scale

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

### 1. Title Page

Include:

- book title
- owner name
- start date
- end date

### 2. How To Use This Logbook

Include:

- 3-5 simple steps
- how often to fill it in
- how often to review it
- explanation of symbols, ratings, or sections

### 3. Setup Or Goal Page

Include:

- user's goal
- starting point
- constraints
- what success looks like

### 4. Repeating Log Entry Page

Include:

- date/session
- core tracking fields
- checklist or rating if useful
- main notes area
- observations
- next action or follow-up

### 5. Review Page

Add review pages every 7, 14, 30, or 50 entries depending on the niche.

Include:

- wins
- repeated patterns
- what worked
- what needs adjustment
- next focus

### 6. Notes Pages

Add a few pages at the back:

- lined
- dotted
- grid
- blank

---

## Repeating Log Entry Structural Blueprint

This is a wireframe only. Convert it into a refined print layout.

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
- Do not keep the final page blocky or ASCII-like.

---

## Page-Parity Rule for Two-Page-Spread Designs

**Critical, and not covered anywhere in KDP's own documentation.** Any repeating entry format that splits content across a left page and a right page (e.g. "Product Profile" on the left, "Session \& Experience" on the right) depends entirely on those two pages landing on the correct physical sides — get this wrong and the two halves of every single entry will be split across the wrong facing pages for the entire book.

**The rule:** even page numbers are always left-hand (verso), odd page numbers are always right-hand (recto). A page only visually faces the *next* page number if it is even — an odd page faces the *previous* page instead. For a spread's left content to face its right content, the left half must land on an even page and the right half on the very next (odd) page.

**Practical check before finalizing any page sequence:** count every page that comes before the repeating spread section starts (title, how-to-use, legend, index, etc. — all of front matter).

* If that count is **odd**, the spread section starts on an even page and will pair correctly.
* If that count is **even**, the spread section starts on an odd page and will **not** pair correctly — fix this before treating the layout as final, not after.

**Fix if front matter comes out even:** add or remove exactly one page anywhere in front matter (split one reference section across an extra page, add a half-title, etc.) rather than restructuring the whole document. This same check applies to any other two-page unit meant to be seen together — review spreads, a favorites/summary spread — not just the main repeating entry.

**Verify by testing the real output, not just the arithmetic:** after building the file, extract the text of the first spread's two pages directly from the generated PDF and confirm page N is even and contains the "left" content while page N+1 is odd and contains the "right" content. Checking the actual rendered file catches transcription errors in the page-counting logic that pure arithmetic can miss.

\---

## Pre-Flight Geometry Audit

Before treating any interior as final, build a lightweight instrumented canvas that mimics the real drawing API (setFont, drawString, line, rect, circle, etc.) but records geometry instead of rendering, then run **every unique page-drawing function** through it — not just a visual spot-check of a few pages. This was the single most effective QA step across the whole project; several real defects were only caught this way, and one (a header sitting too close to the trim edge) was initially "fixed" based on hand-calculated math that turned out to still miss a related, undetected issue nearby.

At minimum, check for each page type:

* **Content floor/ceiling:** does anything drawn fall outside the safe content box, excluding the intentional header/footer chrome?
* **Line clustering:** are any two horizontal rules closer together than roughly 0.19–0.20in anywhere on the page? (This catches double-divider clutter automatically, including in places not otherwise being reviewed.)
* **Consistency across page types:** is the header-to-first-content gap the same on every page type that has one, not just the ones that happened to get checked by hand?

Hand-tracing the arithmetic for one or two representative pages is a useful sanity check during development, but is not a substitute for this — it only verifies what you thought to check, and real bugs tend to hide exactly in what wasn't thought to check.

\---

## Cover Design System

The cover must sell the book in Amazon search results.

### Thumbnail Priorities

1. Title is readable.
2. Niche is obvious.
3. Buyer identity is clear.
4. Mood is different from competitors.
5. Design looks professional.

### Front Cover Hierarchy

Recommended order:

1. Main title
2. Niche/use-case subtitle
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

#### Utility / Workshop

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

### If Cover Artwork Originates From AI Generation

If any part of the cover (illustration, motif, etc.) is produced by an AI image tool, two things follow:

1. **Disclose it.** KDP requires disclosure of AI-generated content (text, images, translations) during the publishing setup flow. This applies to the artwork even if the surrounding typography is rebuilt separately as real, non-AI-generated type.
2. **Don't trust the AI-rendered text.** Text baked into an AI-generated image is prone to warped letterforms, incorrect kerning, or subtle misspellings, and is raster-only at whatever resolution the source image was generated at — never final-quality. Extract the artwork/motif only, discard any AI-rendered text entirely, and rebuild all title/subtitle/cover copy as real, embedded type. If the artwork has a flat background, consider making that background transparent rather than color-matching a rectangle — even a near-perfect colour match (within 1/255 per channel) can render as a visible seam once composited, while a transparent cutout composited directly onto the real background guarantees no seam is possible regardless of the source image's exact pixel values.

---
