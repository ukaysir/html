# Festival Research Dashboard Design System

## Direction
- Visual target: Toss-like minimal Korean product page, not a dark dashboard and not festival-themed per-page art direction.
- Mood: clean, trusted, calm, spacious, highly readable.
- Core rule: every HTML page uses the same design tokens and Pretendard typography.

## Typography
- Font family: Pretendard only.
- Fallback: `-apple-system, BlinkMacSystemFont, system-ui, sans-serif` only for failed font loading.
- Heading weight: 800-900, tight letter spacing, short lines.
- Body weight: 400-600, generous line height.
- Numeric/stat text: 800-900 with Toss-blue emphasis.

## Color tokens
- Background: `#f8fafc` with very subtle vertical gradient.
- Surface: `#ffffff`.
- Primary text: `#191f28`.
- Secondary text: `#6b7684`.
- Tertiary text: `#8b95a1`.
- Primary blue: `#3182f6`.
- Blue hover: `#1b64da`.
- Success: `#00a76f`.
- Warning: `#f59f00`.
- Danger: `#f04452`.
- Border: `#e5e8eb`.

## Layout
- Page max width: 1120px.
- Desktop gutter: 24px minimum.
- Mobile gutter: 18px minimum.
- Header has large top whitespace and one clear headline.
- Main sections use open whitespace first, cards second.
- Avoid festival-specific background colors, ornamental gradients, and decorative blobs.

## Components
- Card: white background, 24-28px radius, 1px border, soft shadow.
- KPI card: same card style with blue numeric emphasis.
- Table: rounded white surface, sticky-looking header tone, clear row dividers.
- Link/button: Toss-blue, no underline by default, underline or darker blue on hover.
- Note/callout: white card with left blue border, not colored panels.

## Information hierarchy
- Every page starts with eyebrow, h1, lead, then evidence panels or KPI cards.
- Cause analysis sections use consistent card grids.
- Timeline sections use consistent date + text rows.
- Procurement sections use tables.
- Source sections are plain ordered lists for trust and scanability.

## Accessibility and performance
- Keep semantic HTML.
- Do not use icon emoji.
- Do not require JavaScript for reading.
- CSS must be shared from `assets/toss-report-theme.css` and linked after page-local styles so it wins.
- Do not run validation unless explicitly requested by the user.

## Accepted debt
- Existing pages contain heterogeneous local styles. The shared CSS intentionally overrides them instead of rewriting every page manually.
- Full visual QA is deferred because the user requested ongoing research/commit cadence and did not ask to run browser validation.
