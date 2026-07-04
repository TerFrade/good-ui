# Log Books KDP Prompt System v2

## Purpose

This document is a polished prompt system for creating **physical log books for Amazon KDP** using AI.

It is designed for the actual workflow where the user may provide mostly:

- competitor cover screenshots
- competitor interior screenshots
- competitor review screenshots or review text
- product titles, subtitles, descriptions, ratings, prices, page counts, or trim sizes when available

The AI must then research, analyze, design, and guide the creation of a better original physical logbook.

Use this document together with:

`docs/log-books-ai-design-document.md`

That companion document is the physical print design guide. This v2 document is the prompt and workflow system.

---

## Important Style Direction

The target style is **modern, minimalist, polished, and practical**.

The logbook should feel inspired by:

- Refactoring UI principles
- Tailwind-style spacing systems
- clean modern product design
- calm hierarchy
- strong typography
- thoughtful whitespace
- useful structure

However, this is **not a web app**. Do not create buttons, cards, hover states, responsive screens, or app-style components unless using them only as conceptual inspiration.

Translate good UI thinking into print:

- spacing systems become print spacing and field grouping
- visual hierarchy becomes cover/title/section hierarchy
- component consistency becomes reusable page templates
- Tailwind-style tokens become fixed print tokens for margins, line weights, typography, and repeated page modules
- UI clarity becomes handwriting usability and low-friction page flow

### ASCII / Wireframe Warning

Any ASCII diagrams, text blueprints, or block layouts in these prompts are **structural references only**.

They are not the final visual style.

The AI must not copy the ASCII look into the final design. The final output should use a modern minimalist print design style with clean spacing, subtle lines, refined typography, and strong visual hierarchy.

---

## Core Rule

If the user provides mostly competitor evidence, the AI must still:

1. infer the niche and target buyer
2. analyze covers, interiors, and reviews
3. do additional research where useful
4. identify visual, functional, emotional, usability, positioning, and production gaps
5. create a better original logbook concept
6. use `docs/log-books-ai-design-document.md` as the governing physical print guide
7. propose a modern minimalist cover direction
8. propose a practical interior structure
9. create prompts for generating the cover and interior
10. review the final result against usability and KDP-readiness

Do not stop because the input is incomplete. Make reasonable inferences and clearly label them.

---

## How To Use With Competitor Screenshots Only

When the user only uploads images and gives little explanation, the AI should follow this approach:

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

5. **Use the design guide**
   - physical print design rules come from `docs/log-books-ai-design-document.md`
   - use modern minimalist style, not ASCII/blocky styling

6. **Produce build-ready outputs**
   - product concept
   - cover direction
   - interior page list
   - prompt pack for cover/interior generation
   - QA checklist

---

## Recommended Workflow

### Step 0 - Master Orchestrator

Use when starting from competitor screenshots/reviews and you want the AI to run the whole strategy process.

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

Output:

- cover market analysis
- interior market analysis
- positive review patterns
- negative review opportunities
- gap map

### Step 2 - Better Product Concept + Physical Design Spec

Use after competitor analysis.

Output:

- concept name direction
- positioning
- target buyer
- cover direction
- interior structure
- trim/page-count recommendation
- print design system

### Step 3 - Interior Page Layout Plan

Use after the concept is clear.

Output:

- full page sequence
- repeated page template
- unique pages
- review pages
- notes/reference pages
- layout rules
- production checklist

### Step 4 - Cover Brief + Generation Prompts

Use after the concept and page count are known.

Output:

- cover strategy
- front cover brief
- back cover copy direction
- spine guidance
- thumbnail strategy
- image/design AI prompts

### Step 5 - Final QA Review

Use after cover/interior drafts or PDFs exist.

Output:

- pass/fail summary
- highest-risk issues
- design polish issues
- usability issues
- KDP technical risks
- exact fixes before upload

---

# Prompt 0 - Master Orchestrator

Use this first when you want the AI to take competitor evidence and turn it into a complete original KDP logbook direction.

```txt
You are helping me create a physical logbook product for Amazon KDP.

This is a printed logbook, not a web app or mobile app.

I may provide very little context beyond competitor material such as:
- competitor cover images
- competitor interior images
- competitor titles or descriptions
- positive reviews
- negative reviews
- occasional ratings, page counts, trim sizes, or prices

Your job is to do the product thinking, research, competitor analysis, print-design planning, and prompt-generation work needed to create a better original logbook.

Use this physical print design guide as the governing design framework:
[PASTE OR ATTACH docs/log-books-ai-design-document.md]

Important visual direction:
- The final product should feel modern, minimalist, polished, and practical.
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
Using the physical design guide, create:
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

I have attached some or all of the following:
- competitor cover images
- competitor interior images
- competitor reviews
- competitor titles, descriptions, ratings, prices, trim sizes, or page counts

Use the attached material and do additional research where useful.

Use this physical design guide as context:
[PASTE OR ATTACH docs/log-books-ai-design-document.md]

Important:
- Use competitor products only for analysis.
- Do not copy titles, covers, layouts, wording, illustrations, or unique design ideas.
- ASCII or text layout examples are structural only; the final design direction should be modern, minimalist, and polished.

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

Use this physical design guide as the governing framework:
[PASTE OR ATTACH docs/log-books-ai-design-document.md]

Design style requirement:
- modern minimalist
- polished
- practical
- clear hierarchy
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
Provide a clear structural blueprint, but remember: any ASCII is only a wireframe. The final style should be clean, modern, and print-polished.

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

Use the product concept and design spec below:
[PASTE OUTPUT FROM PROMPT 2]

Use the physical design guide:
[PASTE OR ATTACH docs/log-books-ai-design-document.md]

Important style requirement:
- modern minimalist print layout
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

Use the product concept and interior spec below:
[PASTE OUTPUT FROM PROMPT 2 OR 3]

Use the physical design guide:
[PASTE OR ATTACH docs/log-books-ai-design-document.md]

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

Use the product concept, design spec, and physical design guide as the standard:
[PASTE PRODUCT CONCEPT / DESIGN SPEC]
[PASTE OR ATTACH docs/log-books-ai-design-document.md]

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
