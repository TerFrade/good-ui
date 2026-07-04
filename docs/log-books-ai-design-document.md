# Log Books UI Design Document + AI Prompt Pack

## Purpose

This document defines a practical design system and AI instruction pack for building **Log Books**: structured records for daily work, development notes, deployments, PR reviews, incidents, meetings, learning notes, and personal reflections.

Use this file when asking an AI coding assistant to create or refactor Log Book screens. It gives the assistant concrete decisions for sizing, fonts, colours, spacing, layout, hierarchy, component structure, accessibility, and implementation checks.

The goal is to avoid vague instructions like:

> Make the log books UI look good.

Instead, use instructions like:

> Build the Log Books UI using the design tokens, component contracts, spacing rules, typography scale, states, and acceptance checklist from this design document.

---

## Source Design Principles

This repo summarizes ideas from **Refactoring UI**. The Log Books feature should apply these principles directly:

1. **Systematize everything**: avoid one-off values; use predefined colours, spacing, typography, shadows, radius, widths, and states.
2. **Start with too much space**: begin with generous spacing, then tighten only where the UI needs density.
3. **Use visual hierarchy**: guide the eye with weight, contrast, spacing, and colour instead of only font size.
4. **Use fixed widths**: constrain sidebars, forms, and reading columns so content remains comfortable.
5. **Use contextual line-height**: long text needs enough line-height, while large headings can be tighter.
6. **Balance weight and contrast**: muted text can use slightly stronger weight; strong text should not always be huge.
7. **Avoid ambiguous spacing**: spacing should clearly show which items belong together.
8. **Avoid too many borders**: prefer background, spacing, and subtle shadows over border-heavy layouts.
9. **Avoid too-long lines**: long-form text should sit in readable columns.
10. **Design empty states properly**: Log Books depend on user-created content, so empty states are part of the core UX.
11. **Think mobile first**: start with a small mobile canvas and progressively enhance for desktop.

---

## Product Definition

A **Log Book** is a structured journal/work-record area where users can create, review, filter, and maintain entries.

A good Log Book helps the user answer:

- What happened?
- When did it happen?
- What category does it belong to?
- What is the current status?
- What should I do next?
- What context should an AI assistant remember from this entry?

The UI should feel:

- calm
- spacious
- focused
- professional
- developer-friendly
- easy to scan under pressure
- trustworthy enough for important work notes

Avoid:

- dense admin-dashboard clutter
- random spacing values
- every element fighting for attention
- excessive borders
- tiny unreadable metadata
- paragraphs stretching across the full screen
- too many bright colours in one section

---

## Core User Flows

### Flow 1: Create First Log Book

1. User lands on empty Log Books page.
2. Empty state explains what Log Books are.
3. User chooses `Create log book` or selects a template.
4. User fills in title, description, category, and optional default template.
5. New Log Book appears as a card.

### Flow 2: Create Log Entry

1. User opens a Log Book.
2. User selects `New entry`.
3. User chooses a template or blank entry.
4. User fills in title, summary, tags, status, body, action items, and AI context.
5. User saves as draft or publishes/completes entry.

### Flow 3: Review Existing Logs

1. User searches or filters entries.
2. User scans entry list.
3. User opens an entry.
4. User reads summary first, then details.
5. User copies useful AI context or follows up on action items.

### Flow 4: Ask AI From a Log

1. User opens a log entry.
2. User uses the `AI context` block.
3. User copies or sends a clean prompt based on the entry.
4. AI receives structured context instead of messy notes.

---

## Design Tokens

### Typography

Preferred font stack:

```css
font-family: Inter, Satoshi, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
```

Use this scale:

| Token | Size | Line height | Weight | Letter spacing | Use |
|---|---:|---:|---:|---:|---|
| `display` | 40px | 48px | 700 | -0.035em | Rare hero/header moments |
| `h1` | 32px | 40px | 700 | -0.03em | Page titles |
| `h2` | 24px | 32px | 650 | -0.025em | Section titles |
| `h3` | 20px | 28px | 650 | -0.02em | Card titles / entry titles |
| `body-lg` | 18px | 30px | 400 | -0.01em | Important readable text |
| `body` | 16px | 28px | 400 | 0 | Long-form log content |
| `body-sm` | 14px | 22px | 400 | 0 | Metadata / helper text |
| `caption` | 12px | 18px | 600 | 0.04em | All-caps labels / badges |

Rules:

- Use tighter tracking for larger headings.
- Use looser tracking for all-caps labels.
- Do not make secondary metadata smaller than 12px.
- Long-form log body should usually be `16px / 28px`.
- Prefer stronger weight and better contrast before increasing font size.

---

### Colours

Use a neutral-first palette with one primary colour and functional accents.

```ts
export const logBookColors = {
  background: "#F8FAFC",
  backgroundSubtle: "#F1F5F9",
  surface: "#FFFFFF",
  surfaceMuted: "#F8FAFC",
  surfaceElevated: "#FFFFFF",

  textStrong: "#0F172A",
  text: "#334155",
  textMuted: "#64748B",
  textSubtle: "#94A3B8",
  textInverse: "#FFFFFF",

  borderSubtle: "#E2E8F0",
  borderStrong: "#CBD5E1",

  primary: "#2563EB",
  primaryHover: "#1D4ED8",
  primarySoft: "#DBEAFE",
  primarySoftText: "#1E40AF",

  success: "#16A34A",
  successSoft: "#DCFCE7",
  successText: "#166534",

  warning: "#D97706",
  warningSoft: "#FEF3C7",
  warningText: "#92400E",

  danger: "#DC2626",
  dangerSoft: "#FEE2E2",
  dangerText: "#991B1B",

  info: "#0284C7",
  infoSoft: "#E0F2FE",
  infoText: "#075985"
};
```

Colour rules:

- Use `textStrong` only for titles and high-priority content.
- Use `text` for normal body copy.
- Use `textMuted` for metadata and secondary descriptions.
- Use `primary` only for primary actions, selected states, important links, and focus states.
- Use accent colours only for meaningful status or category communication.
- Do not create rainbow tag chaos. Tags should be neutral by default.

---

### Spacing

Use this spacing scale only:

| Token | Pixels | Use |
|---|---:|---|
| `1` | 4px | Icon/text gap, micro spacing |
| `2` | 8px | Tight related spacing |
| `3` | 12px | Badge gaps, compact form gaps |
| `4` | 16px | Default control spacing |
| `5` | 20px | Small card padding |
| `6` | 24px | Default card padding |
| `8` | 32px | Section spacing |
| `10` | 40px | Large section spacing |
| `12` | 48px | Page block spacing |
| `16` | 64px | Large layout separation |
| `20` | 80px | Rare large spacing |

Spacing rules:

- Page padding mobile: `16px`
- Page padding tablet: `24px`
- Page padding desktop: `32px`
- Card padding mobile: `20px`
- Card padding desktop: `24px` to `32px`
- Gap between label and input: `6px` to `8px`
- Gap between form fields: `20px` to `24px`
- Gap between sections inside a card: `24px`
- Gap between major page sections: `40px`
- Use larger spacing between unrelated groups than related items.

Bad:

```tsx
<div className="mt-[19px] gap-[13px] p-[27px]" />
```

Good:

```tsx
<div className="mt-6 gap-4 p-6" />
```

---

### Radius

```ts
export const radii = {
  sm: "8px",
  md: "12px",
  lg: "16px",
  xl: "20px",
  "2xl": "24px",
  full: "9999px"
};
```

Rules:

- Buttons: `12px`
- Inputs/selects: `12px`
- Cards: `20px` or `24px`
- Badges/tags: `9999px`
- Large panels/modals: `24px`

---

### Shadows

```ts
export const shadows = {
  xs: "0 1px 2px rgba(15, 23, 42, 0.05)",
  sm: "0 1px 3px rgba(15, 23, 42, 0.08), 0 1px 2px rgba(15, 23, 42, 0.06)",
  md: "0 8px 24px rgba(15, 23, 42, 0.08)",
  lg: "0 20px 50px rgba(15, 23, 42, 0.12)"
};
```

Rules:

- Default cards: `xs` or subtle border.
- Dropdowns/popovers: `md`.
- Modals/dialogs: `lg`.
- Do not apply heavy shadows to every card.

---

### Widths

Use fixed readable widths where appropriate:

| Area | Width |
|---|---:|
| App shell max width | 1280px |
| Main content max width | 1120px |
| Reading column max width | 720px |
| Form column max width | 760px |
| Sidebar width | 280px |
| Inspector panel width | 360px |
| Empty state max width | 520px |

Rules:

- Long-form body text should stay between `680px` and `760px` max width.
- Do not let paragraphs span the full desktop viewport.
- Sidebars should not shrink until text wraps awkwardly.

---

## Layout System

### Desktop Shell

```txt
┌─────────────────────────────────────────────────────────────┐
│ Top Bar: breadcrumb, search, create button                   │
├───────────────┬────────────────────────────┬────────────────┤
│ Sidebar       │ Main Content               │ Inspector      │
│ 280px fixed   │ readable column             │ 360px optional │
└───────────────┴────────────────────────────┴────────────────┘
```

### Mobile Shell

```txt
┌──────────────────────┐
│ Top Bar              │
├──────────────────────┤
│ Log Book List        │
├──────────────────────┤
│ Selected Entry       │
└──────────────────────┘
```

### Page Container Example

```tsx
<main className="min-h-screen bg-slate-50 px-4 py-6 sm:px-6 lg:px-8 lg:py-8">
  <div className="mx-auto max-w-7xl">
    {/* content */}
  </div>
</main>
```

---

## Core Components

### `LogBooksPage`

Purpose: Main overview page for all log books.

Must include:

- Page header
- Subtitle/explanation
- Primary `Create log book` action
- Search/filter row when content exists
- Log book cards/grid
- Recent entries section
- Empty state when no log books exist

Spacing:

- Header title/subtitle gap: `8px`
- Header bottom margin: `32px`
- Header/action gap: `24px`
- Filter row margin bottom: `24px`
- Card grid gap: `20px` to `24px`

Responsive:

- Mobile: stack header actions, full-width primary button, one-column cards.
- Desktop: header title/action can sit horizontally, 2-3 column card grid.

---

### `LogBookCard`

Purpose: Shows a single log book summary.

Content:

- Icon/category marker
- Title
- Description
- Entry count
- Last updated date
- Optional pinned badge
- Optional status summary

Recommended dimensions:

- Desktop min height: `180px`
- Padding: `24px`
- Radius: `24px`
- Internal gap: `16px`

Suggested Tailwind shape:

```tsx
className="rounded-3xl border border-slate-200 bg-white p-6 shadow-xs transition hover:-translate-y-0.5 hover:shadow-md"
```

Rules:

- Title: `20px`, semibold, strong text.
- Description: `14px`, `22px` to `24px` line height, muted text, max 2 lines in grid.
- Metadata: `13px` to `14px`, muted text.
- Icon container: `40px x 40px`, rounded `14px`, soft background.
- The whole card may be clickable, but do not also make every inner element visually dominant.

---

### `LogEntryList`

Purpose: Scannable list of entries.

Each row should include:

- Date/time
- Entry title
- One-line summary
- Tags
- Status
- Optional linked project/context
- Actions menu

Desktop row:

```txt
[date] [title + summary + tags] [status] [actions]
```

Mobile row:

```txt
[title]
[summary]
[tags]
[date + status]
```

Rules:

- Row padding: `16px` to `20px`.
- Row gap: `12px`.
- Use either subtle row dividers or separate card rows; do not over-border everything.
- Active row: soft primary background plus optional left accent line.
- Hover row: subtle background, not a dramatic colour change.

---

### `LogEntryDetail`

Purpose: Reading view for one entry.

Structure:

1. Entry title
2. Summary paragraph
3. Metadata strip
4. Main body sections
5. Action items
6. AI context block
7. Related links/attachments

Recommended section order:

```txt
Title
Summary
Metadata chips
---
Context
What happened
Decisions made
Action items
AI context
Related links
```

Typography:

- Title: `32px / 40px`, bold, tight tracking.
- Summary: `18px / 30px`, muted but readable.
- Body: `16px / 28px`, normal text.
- Section headings: `14px`, semibold, muted, optional uppercase with tracking.

Rules:

- Body content max width: `680px` to `760px`.
- Do not stretch long content across the full screen.
- Make summary scannable before detailed body content.

---

### `LogEntryEditor`

Purpose: Create/edit form for entries.

Fields:

- Title
- Log book/category
- Date/time
- Status
- Tags
- Summary
- Body sections
- Action items
- AI context/prompt notes

Layout rules:

- Single-column form by default.
- Two-column layout only for short metadata fields on tablet/desktop.
- Inputs: `44px` to `48px` high.
- Textareas: start at `120px` to `180px` high.
- Label-to-field gap: `6px` to `8px`.
- Field group gap: `20px` to `24px`.
- Form max width: `760px`.

Input style example:

```tsx
className="h-11 rounded-xl border border-slate-300 bg-white px-3 text-sm text-slate-900 shadow-xs outline-none transition placeholder:text-slate-400 focus:border-blue-500 focus:ring-4 focus:ring-blue-100"
```

---

### `StatusBadge`

Statuses:

- Draft
- Active
- Waiting
- Blocked
- Done
- Archived

Sizing:

- Height: `24px` or `28px`
- Horizontal padding: `10px`
- Radius: full
- Font: `12px`, medium

Colours:

| Status | Background | Text |
|---|---|---|
| Draft | `#F1F5F9` | `#475569` |
| Active | `#DBEAFE` | `#1E40AF` |
| Waiting | `#FEF3C7` | `#92400E` |
| Blocked | `#FEE2E2` | `#991B1B` |
| Done | `#DCFCE7` | `#166534` |
| Archived | `#F8FAFC` | `#64748B` |

---

### `TagPill`

Purpose: Display tags without overpowering the UI.

Suggested style:

```tsx
className="inline-flex h-7 items-center rounded-full bg-slate-100 px-3 text-xs font-medium text-slate-600"
```

Rules:

- Tags are neutral by default.
- Use colour only for meaningful categories.
- Do not use many competing bright colours in a small area.

---

### `EmptyState`

Purpose: Guide users when there are no log books or no entries.

Required content:

- Icon or simple illustration
- Friendly title
- Short explanation
- Primary action
- Optional secondary action
- Optional template suggestions

Sizing:

- Container max width: `520px`
- Padding: `24px` mobile, `40px` desktop
- Icon size: `48px`
- Title: `20px` or `24px`
- Description: `14px` to `16px`, max width `420px`

Example copy:

```txt
No log entries yet
Capture your first work note, incident, learning, or decision so future-you and your AI assistant have clean context.
```

Important:

- Hide tabs, filters, and sorting controls if there is no content yet.
- The empty state should prioritize creating the first useful entry.

---

## Log Book Templates

### Daily Work Log

Fields:

- Date
- Focus area
- Tasks completed
- Blockers
- Decisions
- Follow-ups
- AI context

### Development Log

Fields:

- Feature/task
- Branch/PR
- Problem solved
- Implementation notes
- Edge cases
- Tests added
- Risks
- Follow-ups

### Deployment Log

Fields:

- Environment
- Version/branch
- Deployment steps
- Verification steps
- Rollback plan
- Issues found
- Sign-off

### PR Review Log

Fields:

- PR link
- Area reviewed
- Concerns
- Suggestions
- Tests checked
- Decision
- Follow-up comments

### Incident Log

Fields:

- Incident summary
- Impact
- Timeline
- Root cause
- Mitigation
- Follow-up actions
- Lessons learned

### Learning Log

Fields:

- Topic
- Source/book/video/course
- Main idea
- Examples
- How I can apply this
- Questions
- Next practice step

---

## Interaction States

Every interactive component must define:

- Default
- Hover
- Focus-visible
- Active/pressed
- Selected/current
- Disabled
- Loading
- Error
- Empty

### Primary Button

```tsx
className="inline-flex h-11 items-center justify-center rounded-xl bg-blue-600 px-4 text-sm font-semibold text-white shadow-sm transition hover:bg-blue-700 focus-visible:outline-none focus-visible:ring-4 focus-visible:ring-blue-100 disabled:cursor-not-allowed disabled:opacity-50"
```

### Secondary Button

```tsx
className="inline-flex h-11 items-center justify-center rounded-xl border border-slate-300 bg-white px-4 text-sm font-semibold text-slate-700 shadow-xs transition hover:bg-slate-50 focus-visible:outline-none focus-visible:ring-4 focus-visible:ring-slate-100 disabled:cursor-not-allowed disabled:opacity-50"
```

### Tertiary Button

```tsx
className="inline-flex h-10 items-center justify-center rounded-xl px-3 text-sm font-medium text-slate-600 transition hover:bg-slate-100 hover:text-slate-900 focus-visible:outline-none focus-visible:ring-4 focus-visible:ring-slate-100"
```

### Destructive Button

Rules:

- Destructive actions should be visually subtle by default.
- Use strong red styling only in confirmation flows where the destructive action is the main decision.
- Always require confirmation for deleting log books or entries.

---

## Responsive Behaviour

### Mobile: `<640px`

- Single column.
- Full-width primary action.
- Hide inspector panel behind drawer or separate route.
- Search and filters stack vertically.
- Cards are full width.
- Entry detail body fills available container but remains readable.
- Sticky bottom create action is allowed for frequent logging.

### Tablet: `640px - 1024px`

- Two-column card grid where useful.
- Sidebar may collapse.
- Filters may wrap.
- Editor metadata can use two columns.

### Desktop: `>1024px`

- Sidebar visible when useful.
- Main content constrained.
- Optional inspector panel.
- Card grid can use 2 to 3 columns.
- Long-form content remains constrained.

---

## Accessibility Requirements

- All interactive elements must be keyboard reachable.
- Use visible focus states.
- Inputs must have labels.
- Icon-only buttons must have accessible names.
- Error messages must be close to the relevant field.
- Do not rely on colour alone for status.
- Destructive actions must have confirmation.
- Loading states should not cause major layout shift.
- Text contrast should meet WCAG AA.

---

## Recommended TypeScript Models

```ts
export type LogBookCategory =
  | "work"
  | "development"
  | "deployment"
  | "review"
  | "incident"
  | "learning"
  | "personal";

export type LogBook = {
  id: string;
  title: string;
  description?: string;
  category: LogBookCategory;
  entryCount: number;
  lastUpdatedAt?: string;
  pinned?: boolean;
};

export type LogEntryStatus =
  | "draft"
  | "active"
  | "waiting"
  | "blocked"
  | "done"
  | "archived";

export type LogEntry = {
  id: string;
  logBookId: string;
  title: string;
  summary?: string;
  body?: string;
  status: LogEntryStatus;
  tags: string[];
  createdAt: string;
  updatedAt?: string;
  occurredAt?: string;
  aiContext?: string;
  actionItems?: Array<{
    id: string;
    title: string;
    done: boolean;
  }>;
};
```

---

## AI Prompt Pack

### Prompt 1: Create the Full Log Books Feature

```txt
You are a senior product designer and frontend engineer. Build a polished Log Books feature using the design document below as strict requirements.

Goal:
Create a clean, calm, professional Log Books UI where users can create, browse, filter, read, and edit structured log entries.

Hard requirements:
- Use the provided design tokens for typography, colours, spacing, radius, shadows, and layout widths.
- Build mobile first.
- Use reusable components, not one giant page.
- Include LogBooksPage, LogBookCard, LogEntryList, LogEntryDetail, LogEntryEditor, StatusBadge, TagPill, EmptyState, and FilterBar.
- Include default, hover, focus, loading, disabled, empty, and error states where relevant.
- Use realistic sample data.
- Keep long-form text max width around 680px to 760px.
- Use clear hierarchy with weight, contrast, colour, and spacing instead of only large font sizes.
- Avoid excessive borders.
- Include accessible labels, keyboard focus states, and aria-labels for icon-only buttons.

Before coding:
1. Briefly summarize the component structure.
2. List the files you will create/change.
3. Confirm the design tokens you will use.

Then implement the feature.

Design document:
[PASTE THIS DOCUMENT HERE]
```

### Prompt 2: Refactor an Existing Log Books UI

```txt
You are refactoring an existing Log Books UI to match a polished Refactoring UI-inspired design system.

Review the current implementation and improve it using these rules:
- Replace random one-off spacing with the spacing scale from the design document.
- Improve hierarchy using font weight, contrast, muted metadata, and spacing.
- Increase breathing room where the UI feels cramped.
- Reduce unnecessary borders and use background, spacing, and subtle shadows instead.
- Constrain long-form content to readable widths.
- Make empty states intentional and useful.
- Ensure mobile layout works first, then enhance desktop.
- Keep existing business logic intact unless it conflicts with usability.

Output format:
1. Issues found in the current UI.
2. Design changes you will make.
3. Component/file changes.
4. Implementation.
5. Final checklist against the design document.

Design document:
[PASTE THIS DOCUMENT HERE]
```

### Prompt 3: Generate Only the Component Library

```txt
Create only the reusable component library for Log Books. Do not build the full page yet.

Components required:
- Button variants: primary, secondary, tertiary, destructive
- StatusBadge
- TagPill
- LogBookCard
- LogEntryRow
- EmptyState
- Field, Textarea, Select styling
- SectionHeader
- MetadataStrip

Requirements:
- Use exact tokens from the design document.
- Include TypeScript props.
- Include accessible labels and focus states.
- Include sample usage for each component.
- Do not use random colours or arbitrary pixel values.
- Keep components composable and easy to reuse.

Design document:
[PASTE THIS DOCUMENT HERE]
```

### Prompt 4: Create a Log Entry Editor Form

```txt
Build a Log Entry Editor form using the provided design system.

Fields:
- Title
- Log book/category
- Date/time
- Status
- Tags
- Summary
- Body sections
- Action items
- AI context

Rules:
- Single-column form by default.
- Use two columns only for short metadata fields on tablet/desktop.
- Inputs should be 44px to 48px high.
- Textareas should start at 120px to 180px high.
- Labels should be 6px to 8px from their field.
- Field groups should have 20px to 24px vertical gaps.
- Include validation error states.
- Include save, cancel, and save draft actions.
- Use a clear button hierarchy.

Design document:
[PASTE THIS DOCUMENT HERE]
```

### Prompt 5: Create the Empty State and First-Use Flow

```txt
Design and implement the first-use empty state for Log Books.

Requirements:
- No pointless filters or tabs before content exists.
- Include a friendly title, short explanation, primary action, and optional template suggestions.
- Make it visually polished but not playful.
- Use max width around 520px.
- Use 24px padding on mobile and 40px padding on desktop.
- Include template cards for Daily Work Log, Development Log, Deployment Log, PR Review Log, Incident Log, and Learning Log.
- Ensure the primary action is obvious.

Design document:
[PASTE THIS DOCUMENT HERE]
```

### Prompt 6: AI Review Prompt After Implementation

```txt
Review the implemented Log Books UI against this design document.

Check specifically for:
- Random arbitrary spacing or colour values
- Weak visual hierarchy
- Cramped areas
- Too many borders
- Long unreadable text lines
- Missing empty states
- Missing loading/error/disabled states
- Poor mobile behaviour
- Inconsistent typography
- Missing accessibility labels/focus states
- Destructive actions that are too visually aggressive outside confirmation flows

Output:
1. Pass/fail summary.
2. Exact issues found.
3. Suggested fixes.
4. Priority order.
5. Code-level recommendations.

Design document:
[PASTE THIS DOCUMENT HERE]
```

---

## Implementation Acceptance Checklist

### Visual Design

- [ ] Uses the defined colour tokens.
- [ ] Uses the defined spacing scale.
- [ ] Uses the defined typography scale.
- [ ] Uses consistent radius values.
- [ ] Uses shadows sparingly.
- [ ] Avoids unnecessary borders.
- [ ] Has clear visual hierarchy.
- [ ] Has enough breathing room.

### Layout

- [ ] Mobile layout works first.
- [ ] Desktop layout uses fixed readable widths.
- [ ] Long-form content does not exceed 760px width.
- [ ] Sidebar does not shrink below a usable width.
- [ ] Inspector panel is optional and not required on mobile.

### Components

- [ ] `LogBooksPage` exists.
- [ ] `LogBookCard` exists.
- [ ] `LogEntryList` exists.
- [ ] `LogEntryDetail` exists.
- [ ] `LogEntryEditor` exists.
- [ ] `StatusBadge` exists.
- [ ] `TagPill` exists.
- [ ] `EmptyState` exists.
- [ ] `FilterBar` exists.

### States

- [ ] Empty state exists.
- [ ] Loading state exists.
- [ ] Error state exists.
- [ ] Disabled state exists.
- [ ] Hover state exists.
- [ ] Focus-visible state exists.
- [ ] Active/selected state exists.

### Accessibility

- [ ] Inputs have labels.
- [ ] Icon buttons have accessible names.
- [ ] Keyboard navigation works.
- [ ] Focus states are visible.
- [ ] Colour is not the only status indicator.
- [ ] Destructive actions have confirmation.

### AI Context

- [ ] Each log entry has an optional AI context field.
- [ ] Templates guide users to capture useful future context.
- [ ] Log summaries are concise and scannable.
- [ ] Action items are clearly separated from notes.

---

## Final Instruction to AI Builders

Do not optimize for novelty. Optimize for clarity, repeatability, hierarchy, and calm usability.

The best Log Books UI should feel like a reliable workbench: structured enough to guide the user, spacious enough to think clearly, and polished enough that the user trusts it with important notes.
