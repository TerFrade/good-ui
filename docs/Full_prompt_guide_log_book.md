## Important Style Direction

The target style is **minimalist, polished, and practical**.

The logbook should feel inspired by:

* Refactoring UI principles
* Tailwind-style spacing systems
* clean product design
* calm hierarchy
* strong typography
* thoughtful whitespace
* useful structure

This is still a **physical print product**, not a web app.

Do not create:

* responsive layouts
* buttons
* hover states
* app components
* mobile screens
* web page cards

Translate good UI thinking into print:

* spacing systems become print spacing and field grouping
* visual hierarchy becomes cover/title/section hierarchy
* component consistency becomes reusable page templates
* Tailwind-style tokens become fixed print tokens for margins, line weights, typography, and repeated page modules
* UI clarity becomes handwriting usability and low-friction page flow

### ASCII / Wireframe Warning

Any ASCII diagrams, text blueprints, or block layouts in this document are **structural references only**.

They are not the final visual style.

Do not copy the ASCII look into the final design. Convert structural blueprints into refined print layouts with clean spacing, subtle lines, typography, and strong hierarchy.

\---

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

\---

## How To Use With Competitor Screenshots Only

When the user only uploads images and gives little explanation, follow this approach:

1. **Identify what is visible**

   * visible titles
   * niche indicators
   * cover styles
   * interior fields
   * repeated page structures
   * buyer-use clues
2. **Infer the niche**

   * state the likely niche
   * state confidence level
   * list what evidence supports the inference
3. **Research to fill gaps**

   * search for common niche expectations
   * research common buyer complaints
   * check common trim/page-count patterns when relevant
   * research terminology used by real buyers
4. **Do not over-copy**

   * competitor material is for analysis only
   * create a new product angle
   * create original cover and page structures
5. **Use this file**

   * physical print design rules come from `log-books-ai-design-document.md`
   * use minimalist style, not ASCII/blocky styling
6. **Produce build-ready outputs**

   * product concept
   * cover direction
   * interior page list
   * prompt pack for cover/interior generation
   * QA checklist

\---

## Physical KDP Working Assumptions — Verified

Everything in this section is confirmed directly against [KDP's official Trim Size, Bleed, and Margins page](https://kdp.amazon.com/en_US/help/topic/GVBQ3CMEQW3W2VL6), not carried forward from assumption. Re-verify against that page if it's been more than a few months since this doc was last checked — Amazon does update these occasionally.

### Trim Size

6×9in is the default recommendation for this product type — it supports 24–828 pages on black ink/white paper, which comfortably covers any logbook in the 100–150 page range this doc targets.

Useful trim alternatives (all valid 24–828 pages, black ink/white paper, "regular" pricing tier):

* `5 x 8 in`: compact and portable
* `5.5 x 8.5 in`: journal-like and balanced
* `6 x 9 in`: default recommendation
* `7 x 10 in`: **large trim** — better for detailed trackers, costs more to print
* `8.5 x 11 in`: **large trim** — workbook/tracker feel, only 24–590 pages supported, costs more to print

### Interior Margins — Official Minimums

The inside (gutter) margin scales up as the book gets thicker. Outside, top, and bottom margins stay fixed regardless of page count.

|Page count|Inside (gutter) margin|Outside/top/bottom (no bleed)|Outside/top/bottom (with bleed)|
|-|-|-|-|
|24–150|0.375in|0.25in|0.375in|
|151–300|0.5in|0.25in|0.375in|
|301–500|0.625in|0.25in|0.375in|
|501–700|0.75in|0.25in|0.375in|
|701–828|0.875in|0.25in|0.375in|

**Working defaults for a 24–150 page, no-bleed, 6×9in logbook** (confirmed safely above every minimum above, not just assumed):

* Inside/gutter: `0.45 in` (0.075in of margin above the 0.375in minimum)
* Outside: `0.35 in` (0.10in above the 0.25in minimum)
* Top: `0.40 in` (0.15in above the 0.25in minimum)
* Bottom: `0.45 in` (0.20in above the 0.25in minimum)

If a future project exceeds 150 pages, increase the gutter to at least 0.5in per the table above. Outside/top/bottom stay at 0.25in minimum regardless of page count — no need to increase those for a longer book.

### Bleed

* **Covers** always require bleed (0.125in on all outer edges), regardless of the interior's bleed setting.
* **Interior** bleed is only needed if any interior page has an image, background, or illustration reaching the trim edge. A guided logbook with margin-safe form fields does not need interior bleed — use **no bleed**.
* If interior bleed is ever needed, the math is **not symmetric like a cover** — the gutter/spine side never bleeds, only the outer three edges do:

  * Page width with bleed = trim width + 0.125in (outside edge only)
  * Page height with bleed = trim height + 0.25in (0.125in top + 0.125in bottom)

### Cover Technical Rules

The cover should be a single full-wrap PDF:

```txt
Back cover + spine + front cover
```

Full wrap width = bleed (0.125in) + back cover width + spine width + front cover width + bleed (0.125in).
Full wrap height = trim height + 0.25in (0.125in bleed top + bottom).

Spine width formula (white paper): `(page count × 0.002252) + 0.06 = spine width in inches`. Recalculate this any time the final page count changes — it's a hard dependency, not a rough estimate.

The cover must account for:

* trim size
* page count
* paper type
* ink type
* spine width
* bleed
* safe zones
* barcode area
* matte or glossy finish

Do not add spine text unless the page count comfortably supports it (KDP requires 79+ pages minimum for spine text to be an option at all). Below roughly 110–115 pages, a spine may be too narrow for text to stay comfortably legible — verify with a physical proof rather than trusting the math alone.

\---

## Print Design Philosophy

### 1\. Systematize Everything

Use a small set of repeated decisions:

* same trim size
* same margins
* same line weights
* same label sizes
* same heading hierarchy
* same field spacing
* same page header/footer style
* same cover/interior personality

Avoid random field heights, random margins, random fonts, and inconsistent spacing.

### 2\. Start Spacious

A logbook must be written in by hand. Start with more space than expected, then tighten only where needed.

### 3\. Build Hierarchy

Guide the eye with:

* type size
* weight
* whitespace
* contrast
* section dividers
* field grouping

Do not make every label bold, boxed, or equally loud.

### 4\. Avoid Ambiguous Spacing

Fields that belong together should be close. Separate sections should have clearly larger gaps.

### 5\. Avoid Too Many Borders

Do not create a page full of heavy boxes. Use light lines, whitespace, subtle dividers, and simple labels.

### 6\. Design For Handwriting

Default writing-space rules:

* single writing line: about `0.28-0.35 in` high
* compact writing line: about `0.24 in` high — use this only for reference/lookup tables (e.g. a quick index) where entries are a few words, not for primary writing fields
* notes lines: about `0.32-0.38 in` high
* checkbox: about `0.12-0.16 in`
* rating circle: about `0.16-0.22 in`
* table row: about `0.32-0.45 in`

### 7\. Verify Geometrically Before Finalizing

Hand-tracing the vertical math for a few representative pages is not sufficient — it's exactly how a real spacing bug slipped through undetected on a past project (see "Pre-Flight Geometry Audit" below). Before treating any interior as final, run every unique page type through the actual drawing code with an instrumented/recording canvas and check the real output, not a manual re-derivation of it.

\---

## Interior Design Tokens

### Typography

Use simple print-safe fonts.

Suggested directions to think of niche font styles:

* Professional: Garamond, Palatino, Baskerville-style serif
* Modern: Arial, Helvetica, Inter-style sans serif
* Warm journal: elegant serif heading + clean sans label font
* Technical logbook: clean sans serif with strong structure

Suggested interior sizes:

|Use|Size|Notes|
|-|-:|-|
|Page title|14-18 pt|clear but not huge|
|Section title|10-12 pt|semibold|
|Field label|7.5-9 pt|readable and quiet|
|Helper text|7-8 pt|use lightly|
|Page number|7-8 pt|subtle|

Rules:

* Do not use text below 7 pt.
* Embed fonts in exported PDFs. Note: a "Helvetica" (or other base-14) font reference may appear in a font-embedding check even when every visible glyph uses a properly embedded font — this is a harmless artifact of some PDF generation tools auto-registering the standard 14 fonts as available resources, not an actual embedding failure. Confirm by checking which fonts are actually used for visible text, not just which fonts are listed as resources.
* Use decorative fonts only for cover or large headings.
* Do not use hard-to-read fonts for functional labels.

### Line Weights

|Use|Weight|
|-|-:|
|faint writing lines|0.25 pt|
|normal writing lines|0.5 pt|
|section dividers|0.75 pt|
|rare emphasis|1 pt|

Greyscale defaults:

* Main text: `#222222`
* Secondary text: `#666666`
* Writing lines: `#D9D9D9`
* Dividers: `#B8B8B8`

### Print Spacing Scale

|Token|Size|Use|
|-|-:|-|
|XS|0.05 in|tiny label/line gap|
|SM|0.10 in|tight grouping|
|MD|0.16 in|normal field spacing|
|LG|0.24 in|section spacing|
|XL|0.35 in|major blocks|
|2XL|0.50 in|large breaks|

\---

## Print Component Patterns

These are reusable structural components validated across a full 132-page build — treat them as defaults for any future logbook using a running header/footer and checkbox fields.

### Running Header + Footer ("Chrome")

A consistent header/footer treatment repeated on every interior page reads as *systematic* rather than assembled page-by-page. Recommended structure:

* **Header:** book title (small caps, left) + page-specific label (right, e.g. section or entry name), both sitting **inside** the top margin — not above it. Position the header text roughly 0.15–0.20in below the top safe-margin boundary, with its hairline rule another 0.08–0.10in below the text. Do not place header text above the margin boundary even by a small amount — it reads as encroaching on the trim edge even when technically still inside KDP's hard minimum.
* **Footer:** page number, centered, with an optional small brand mark (e.g. a repeated icon) directly above it and thin hairline rules flanking both — sitting inside the bottom margin.
* **Right-aligned header text:** if using letter-spaced/tracked text, make sure the *actual* rendering routine (not just the width-calculation routine) applies the tracking — a mismatch between the two causes right-aligned text to fall short of the true margin edge, leaving an unintended gap. Test by confirming the rightmost character's true rendered edge lands exactly at the intended boundary.

### Header-to-First-Section Spacing

Where a page has both the running header (with its own rule) and a numbered section header (with its own rule) directly beneath it, leave **at least 0.25–0.30in** between the two rules. Anything tighter reads as a cluttered double-line directly under the header, even though both rules are individually correct. This is easy to miss on the most content-dense page types specifically, since those are the pages where the temptation to save vertical space is strongest — check those pages explicitly, not just the spacious front-matter pages.

### Checkbox Fields

* Size: `0.12–0.16in` per the handwriting-space token table — do not go smaller for the sake of fitting more per row.
* **Vertical alignment:** center the checkbox on the label text's cap-height band, not on the text baseline. A checkbox positioned relative to the baseline alone will visually float below its label. Concretely: if drawing a checkbox of height H next to text with baseline at y and font size S, position the checkbox's bottom edge at approximately `y - 0.02` to `y - 0.03` (in inches), not flush with the baseline itself.
* **Grid consistency:** if a section has two related checkbox rows (e.g. "Form:" and "Type:"), use the *same* column grid for both, or better, make each its own clean single row rather than an uneven multi-row grid. Mismatched grids between adjacent rows read as misaligned even when each row is internally consistent.

\---

## Recommended Page Types

A strong logbook should usually include more than one repeated generic page.

### 1\. Title Page

Include:

* book title
* owner name
* start date
* end date

### 2\. How To Use This Logbook

Include:

* 3-5 simple steps
* how often to fill it in
* how often to review it
* explanation of symbols, ratings, or sections

### 3\. Setup Or Goal Page

Include:

* user's goal
* starting point
* constraints
* what success looks like

### 4\. Repeating Log Entry Page

Include:

* date/session
* core tracking fields
* checklist or rating if useful
* main notes area
* observations
* next action or follow-up

### 5\. Review Page

Add review pages every 7, 14, 30, or 50 entries depending on the niche.

Include:

* wins
* repeated patterns
* what worked
* what needs adjustment
* next focus

### 6\. Notes Pages

Add a few pages at the back:

* lined
* dotted
* grid
* blank

\---

## Page-Parity Rule for Two-Page-Spread Designs

**Critical, and not covered anywhere in KDP's own documentation.** Any repeating entry format that splits content across a left page and a right page (e.g. "Product Profile" on the left, "Session \& Experience" on the right) depends entirely on those two pages landing on the correct physical sides — get this wrong and the two halves of every single entry will be split across the wrong facing pages for the entire book.

**The rule:** even page numbers are always left-hand (verso), odd page numbers are always right-hand (recto). A page only visually faces the *next* page number if it is even — an odd page faces the *previous* page instead. For a spread's left content to face its right content, the left half must land on an even page and the right half on the very next (odd) page.

**Practical check before finalizing any page sequence:** count every page that comes before the repeating spread section starts (title, how-to-use, legend, index, etc. — all of front matter).

* If that count is **odd**, the spread section starts on an even page and will pair correctly.
* If that count is **even**, the spread section starts on an odd page and will **not** pair correctly — fix this before treating the layout as final, not after.

**Fix if front matter comes out even:** add or remove exactly one page anywhere in front matter (split one reference section across an extra page, add a half-title, etc.) rather than restructuring the whole document. This same check applies to any other two-page unit meant to be seen together — review spreads, a favorites/summary spread — not just the main repeating entry.

**Verify by testing the real output, not just the arithmetic:** after building the file, extract the text of the first spread's two pages directly from the generated PDF and confirm page N is even and contains the "left" content while page N+1 is odd and contains the "right" content. Checking the actual rendered file catches transcription errors in the page-counting logic that pure arithmetic can miss.

\---

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

* Fast metadata goes at the top.
* Objective tracking fields come before reflection fields.
* The largest writing space should be for the most important user input.
* End with action, follow-up, or summary.
* Do not overload one page with too many prompts.
* Do not keep the final page blocky or ASCII-like.

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

* strong typography
* lots of negative space
* limited colour palette
* subtle icon or linework

#### Warm Guided Journal

* soft neutrals
* gentle serif/sans pairing
* calm emotional tone

#### Utility / Workshop

* practical grid
* strong labels
* functional, durable feeling

#### Bold Category Standout

* high contrast
* strong title block
* instantly readable in thumbnail

#### Illustrated Niche-Specific

* one strong relevant motif
* not clipart-heavy
* clear buyer signal

### If Cover Artwork Originates From AI Generation

If any part of the cover (illustration, motif, etc.) is produced by an AI image tool, two things follow:

1. **Disclose it.** KDP requires disclosure of AI-generated content (text, images, translations) during the publishing setup flow. This applies to the artwork even if the surrounding typography is rebuilt separately as real, non-AI-generated type.
2. **Don't trust the AI-rendered text.** Text baked into an AI-generated image is prone to warped letterforms, incorrect kerning, or subtle misspellings, and is raster-only at whatever resolution the source image was generated at — never final-quality. Extract the artwork/motif only, discard any AI-rendered text entirely, and rebuild all title/subtitle/cover copy as real, embedded type. If the artwork has a flat background, consider making that background transparent rather than color-matching a rectangle — even a near-perfect colour match (within 1/255 per channel) can render as a visible seam once composited, while a transparent cutout composited directly onto the real background guarantees no seam is possible regardless of the source image's exact pixel values.

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
- product concept
- physical design spec
- cover directions
- interior structure
- generation prompts
- risks and recommendations

### Step 1 - Competitor Analysis

Use when you want deep analysis before product design.

### Step 2 - Better Product Concept + Physical Design Spec

Use after competitor analysis.

### Step 3 - Interior Page Layout Plan

Use after the concept is clear.

### Step 4 - Cover Brief + Generation Prompts

Use after the concept, page count, and trim size are known.

### Step 5 - Final QA Review

Use after cover/interior drafts or PDFs exist.

---

# Prompt 0 - Master Orchestrator

Use this first when you want the AI to take competitor evidence and turn it into a complete original KDP logbook direction.

```txt
You are helping me create a physical logbook product for Amazon KDP.

This is a printed logbook, not a web app or mobile app.

A file named log-books-ai-design-document.md has been provided at the beginning of this session. Treat that file as the governing design document for this entire task. Do not ask me to paste it again.

I may provide very little context beyond competitor material such as:
- competitor cover images
- competitor interior images
- competitor titles or descriptions
- positive reviews
- negative reviews
- occasional ratings, page counts, trim sizes, or prices

Your job is to do the product thinking, research, competitor analysis, print-design planning, and prompt-generation work needed to create a better original logbook.

Important visual direction:
- The final product should feel minimalist, polished, and practical.
- Use Refactoring UI-style principles translated into print: strong hierarchy, consistent spacing, restrained colour, thoughtful whitespace, clear grouping, and useful structure.
- Use Tailwind-style design thinking as inspiration for systematic spacing, typography, and component consistency, but do not design a web app.
- ASCII diagrams or block layouts are only rough structural wireframes. Do not copy the ASCII look. Convert them into refined print layouts.

Research requirement:
Do additional research as needed. If the uploaded material is incomplete, infer what you can, research what matters, and clearly label assumptions.

Originality requirement:
Do not copy competitor covers, titles, layouts, wording, illustrations, or unique concepts. Use competitor material only to identify buyer expectations, visual clichés, functional gaps, review complaints, and product opportunities.

PHASE 1 - UNDERSTAND THE NICHE
- infer the niche and target buyer
- identify the real-world job this logbook helps with
- identify who would buy it and why
- identify whether it is more practical, emotional, professional, hobbyist, wellness, technical, or giftable
- label assumptions clearly

PHASE 2 - RESEARCH
Research what is needed to strengthen the product direction:
- common title/subtitle patterns in this niche
- common cover styles and visual clichés
- common trim sizes and page counts
- typical buyer expectations
- repeated review complaints in this product category
- useful fields or page types real users may need
- KDP-related production assumptions if relevant

PHASE 3 - COMPETITOR COVER ANALYSIS
Analyze the provided covers:
- design style
- colour palette and mood
- typography and hierarchy
- thumbnail readability
- buyer identity signal
- niche clichés
- what looks generic or overused
- what is missing visually
- what would stand out while still belonging to the niche

PHASE 4 - COMPETITOR INTERIOR ANALYSIS
Analyze the provided interiors:
- page types
- fields and sections
- writing space quality
- layout density
- prompt clarity
- field order and daily-use flow
- whether review/setup/reference pages exist
- usability problems
- what feels lazy, generic, cramped, or incomplete
- what real users still need

PHASE 5 - REVIEW MINING
From positive reviews, extract:
- what buyers love
- features they want preserved
- emotional language
- gift/use-case patterns
- quality signals

From negative reviews, extract:
- repeated complaints
- missing features
- layout frustrations
- unmet expectations
- quality issues
- signs the book feels generic or low effort

Group complaints by frequency and severity.

PHASE 6 - GAP MAP
Create:
- visual gap
- functional gap
- emotional gap
- usability gap
- positioning gap
- production-quality gap

PHASE 7 - BETTER PRODUCT CONCEPT
Create a superior original concept:
- working title direction
- subtitle direction
- target buyer
- one-line positioning
- emotional promise
- unique value proposition
- what to keep from competitors
- what to avoid completely

PHASE 8 - PHYSICAL DESIGN SPEC
Using log-books-ai-design-document.md, create:
- recommended trim size
- recommended page count
- black-and-white or colour interior recommendation
- bleed/no-bleed recommendation
- margin and gutter assumptions
- typography direction
- line-weight direction
- spacing direction
- page numbering direction
- page types
- repeating log page blueprint
- review/setup/reference pages

PHASE 9 - COVER DIRECTION
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

PHASE 10 - INTERIOR STRUCTURE
Create:
- full list of page types
- recommended page order
- repeated page count
- what each page includes
- why each page exists
- how each page solves buyer complaints or improves usability
- what pages should not be included because they add filler

PHASE 11 - GENERATION PROMPTS
Create prompts I can use with an image/design AI for:
1. front cover concept
2. full wraparound KDP cover brief
3. interior page layout concept
4. repeated log-entry page
5. final QA review

FINAL OUTPUT FORMAT
Return the answer in this order:
1. niche understanding
2. research summary
3. competitor cover analysis
4. competitor interior analysis
5. review mining summary
6. gap map
7. better product concept
8. physical design spec
9. cover directions
10. interior structure
11. generation prompts
12. final risks and recommendations

Be specific, decisive, and practical. Build something I can actually publish.
```

---

# Prompt 1 - Competitor Analysis + Gap Map

Use this when you want to deeply understand the market before deciding the product concept.

```txt
I am creating a physical logbook for Amazon KDP.

This is a printed logbook, not a web app or mobile app.

A file named log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

I have attached some or all of the following:
- competitor cover images
- competitor interior images
- competitor reviews
- competitor titles, descriptions, ratings, prices, trim sizes, or page counts

Use the attached material and do additional research where useful.

Important:
- Use competitor products only for analysis.
- Do not copy titles, covers, layouts, wording, illustrations, or unique design ideas.
- ASCII or text layout examples are structural only; the final design direction should be minimalist, and polished.

STEP 1 - INFER THE NICHE
- What niche does this appear to be?
- Who is the likely buyer?
- What job does the logbook help them do?
- What assumptions are you making?

STEP 2 - RESEARCH THE MARKET
Research what is needed to strengthen the analysis:
- common product claims
- common cover patterns
- common interior structures
- buyer expectations
- review complaints
- page count and trim-size patterns if relevant

STEP 3 - COVER ANALYSIS
For each competitor cover, assess:
- visual style
- colour palette
- typography hierarchy
- thumbnail readability
- buyer signal
- niche clichés
- what feels generic
- what feels strong
- what is missing visually

STEP 4 - INTERIOR ANALYSIS
For each competitor interior, assess:
- page types
- fields included
- layout density
- handwriting space
- flow and order of fields
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
- missing features
- layout frustrations
- unmet expectations
- quality concerns
- signs of generic or lazy design

STEP 6 - GAP MAP
Create:
- visual gap
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

# Prompt 2 - Better Product Concept + Physical Design Spec

Use this after Prompt 1.

```txt
Using the competitor analysis and gap map below, create a better original physical logbook concept for Amazon KDP.

This is a printed product, not a web app.

A file named log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

Design style requirement:
- minimalist
- polished
- practical
- clear hierarchy
- Refactoring UI-inspired spacing and visual discipline translated into print
- Tailwind-like design consistency translated into fixed print tokens
- no ASCII/blocky final aesthetic

COMPETITOR ANALYSIS AND GAP MAP:
Use the competitor analysis and gap map you produced earlier in this same conversation (Prompt 1's response). Do not ask me to repost it.

Create:

1. PRODUCT POSITIONING
- working title direction
- subtitle direction
- target buyer
- one-line positioning
- emotional promise
- unique value proposition

2. WHAT TO KEEP
- features buyers already like
- niche expectations that should remain

3. WHAT TO AVOID
- competitor clichés
- review complaints
- generic low-content patterns
- cramped or confusing layout choices

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
- what makes it different from competitors

6. INTERIOR DESIGN SYSTEM
- margin and gutter assumptions
- type scale direction
- line-weight direction
- spacing rhythm
- page numbering treatment
- section heading treatment
- handwriting-space rules

7. PAGE STRUCTURE
- all page types
- purpose of each page type
- fields on each page type
- how many times each page repeats
- what buyer complaint or use-case each page solves

8. REPEATING LOG PAGE BLUEPRINT
Provide a clear structural blueprint, but remember: any ASCII is only a wireframe. The final style should be clean and print-polished.

9. FINAL BUILD NOTES
- what to generate next
- risks to watch for
- QA checks before PDF export
```

---

# Prompt 3 - Interior Page Layout Plan

Use this when the concept and physical spec are clear.

```txt
Create a complete interior layout plan for this physical Amazon KDP logbook.

A file named log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

Use the product concept and design spec below:
Use the product concept and physical design spec you produced earlier in this same conversation (Prompt 2's response). Do not ask me to repost it.

Important style requirement:
- minimalist print layout
- clean spacing
- subtle lines
- refined typography
- enough handwriting space
- no heavy boxes unless functionally necessary
- no ASCII/blocky final aesthetic

Create:

1. INTERIOR FORMAT SUMMARY
- trim size
- page count
- bleed/no-bleed
- margin/gutter assumptions
- black-and-white or colour interior

2. FULL PAGE SEQUENCE
List the exact page sequence from page 1 to the final page.

3. UNIQUE PAGE TYPES
For each page type, specify:
- purpose
- fields
- field order
- approximate writing space
- line count or writing area size
- spacing notes
- whether it repeats
- repeat count

4. REPEATING LOG PAGE MASTER TEMPLATE
Specify:
- page header
- top metadata fields
- main tracking fields
- notes/reflection area
- checklist/rating area if needed
- follow-up/action area
- footer/page number treatment

5. REVIEW / SUMMARY PAGES
Specify where review pages appear and what they ask.

6. MODERN PRINT STYLE NOTES
Explain how to make the page feel minimal and polished, not generic or cramped.

7. INTERIOR QA CHECKLIST
Check margins, gutter, readability, handwriting space, line weights, repeated-page consistency, page count, and placeholder removal.
```

---

# Prompt 4 - KDP Cover Brief + Generation Prompts

Use this after the concept, interior structure, trim size, and page count are known.

```txt
Create a professional KDP cover brief and cover-generation prompts for this physical logbook.

A file named log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

Use the product concept and interior spec below:
Use the product concept and interior spec you produced earlier in this same conversation (Prompt 2 and/or Prompt 3's response). Do not ask me to repost it.

Important style requirement:
- modern minimalist
- strong Amazon thumbnail readability
- refined typography
- clear niche signal
- original, not derivative of competitors
- avoid generic Canva-template energy
- avoid copying competitor colours, composition, or motifs too closely

Create:

1. MARKET POSITIONING
- target buyer
- emotional promise
- what the cover must communicate in 2 seconds

2. FRONT COVER BRIEF
- title hierarchy
- subtitle placement
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
- what is inside
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
Check thumbnail readability, originality, safe areas, barcode area, hierarchy, and print-readiness.
```

---

# Prompt 5 - Final PDF / Screenshot QA Review

Use this after the cover or interior has been generated.

```txt
You are reviewing a finished or near-finished physical logbook for Amazon KDP.

I will provide screenshots, exported page images, or PDFs of the cover and interior.

A file named log-books-ai-design-document.md has been provided at the beginning of this session. Use it as the governing design document.

Use the product concept and design spec below as the product-specific standard:
Use the product concept and design spec produced earlier in this same conversation. Do not ask me to repost it. If this is a fresh conversation with no prior context, ask me for it once.

Review for:

1. MARKET FIT
- does the product clearly fit the niche?
- does it speak to the right buyer?
- does it solve the original competitor gaps?

2. COVER QUALITY
- is the title readable at Amazon thumbnail size?
- is the hierarchy strong?
- is the cover original but still niche-relevant?
- does it avoid competitor clichés?
- does it feel modern, minimalist, and polished?

3. INTERIOR USABILITY
- is there enough handwriting space?
- are fields useful and logically ordered?
- are there too many boxes or heavy borders?
- are labels readable?
- do repeated pages feel consistent?
- do setup/review pages add real value?

4. PRINT DESIGN QUALITY
- margins look safe
- gutter looks safe
- line weights are not too dark or too faint
- typography is readable
- page numbers are consistent
- no placeholder text remains
- no ASCII/blocky styling accidentally carried into the final design

5. KDP RISK CHECK
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
4. usability issues
5. KDP technical risks
6. exact fixes before upload
7. final recommendation: ready, almost ready, or needs redesign
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
- [ ] Fonts are embedded (verify programmatically - do not assume; base-14 fonts
      like Times/Helvetica are NOT embedded even though they render fine on screen).
- [ ] Any illustration/motif was sourced or generated as a separate image asset and
      composited in - never hand-coded as raw vector paths without visual verification.
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
- [ ] Cover feels modern, minimalist, and niche-relevant.
- [ ] Images are high resolution.
- [ ] Transparencies flattened.
- [ ] Fonts embedded.
- [ ] No template marks or guide text remain.

---

## Final Instruction

Use this system to create a **better physical logbook**, not a generic low-content notebook.

The final product should:

- look strong in Amazon search
- feel useful when written in
- solve buyer complaints found in competitor reviews
- use a consistent modern minimalist print design system
- avoid copying competitors
- avoid web-app thinking
- avoid ASCII/blocky final styling
- export cleanly as KDP-ready cover and interior PDFs
