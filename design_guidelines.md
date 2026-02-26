# thelaziest.dev --- Branding Design Guidelines (v1)

Lean. Monochrome. High leverage. No decoration.

------------------------------------------------------------------------

# 1. Brand Core

## Positioning

A developer blog about building high-leverage software with minimal
effort.\
Systems over hustle. Automation over repetition. Shipping over
polishing.

## Audience

Senior engineers, indie hackers, infra-focused builders.

## Personality

-   Sharp
-   Minimal
-   Opinionated
-   Dry
-   High signal / low noise

## Optional Tagline

> Maximum leverage. Minimum effort.

------------------------------------------------------------------------

# 2. Visual Identity

## Design Principles

-   Dark-first
-   Monospace-forward
-   No gradients
-   No decorative illustrations
-   No shadows unless functional
-   Aggressive whitespace

## Logo Direction

-   Pure wordmark: `thelaziest.dev`
-   Monospace typography
-   One accent color only
-   Must work in pure black & white

symbol: `//` or `_` used sparingly

------------------------------------------------------------------------

# 3. Color System

## Dark Mode (Canonical)

  Role               Hex
  ------------------ -----------
  Background         `#0B0F14`
  Elevated Surface   `#11161C`
  Border             `#1C232B`
  Primary Text       `#F5F7FA`
  Secondary Text     `#9BA6B2`
  Code Block BG      `#0F141A`

Dark mode is the default brand experience.

------------------------------------------------------------------------

## Light Mode (Secondary)

  Role               Hex
  ------------------ -----------
  Background         `#FAFBFC`
  Elevated Surface   `#F1F3F5`
  Border             `#E2E8F0`
  Primary Text       `#0F1720`
  Secondary Text     `#5B6672`
  Code Block BG      `#F6F8FA`

Light mode should feel like technical documentation.

------------------------------------------------------------------------

## Accent Color (Choose One Only)

### Recommended

Terminal Green: `#00FF88`

### Alternatives

-   Electric Blue: `#3A86FF`
-   Muted Amber: `#FFB703`

### Accent Usage Rules

Use for: - Links - Inline code highlights - Active navigation state -
Buttons (outline or solid) - Minimal separators (`//`)

Never: - Multiple accents on one page - Gradient usage - Large
background floods

------------------------------------------------------------------------

# 4. Typography System (CDN-Based)

## Fonts

### Headings + Code

JetBrains Mono (Google Fonts CDN)

### Body

Inter (Google Fonts CDN)

## Fallback Stack

### Sans

system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple
Color Emoji", "Segoe UI Emoji"

### Monospace

ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation
Mono", "Courier New", monospace

## Type Scale

  Element   Size       Line Height
  --------- ---------- -------------
  H1        40px       1.1
  H2        28px       1.2
  H3        20px       1.3
  Body      16--18px   1.6

Rules: - Monospace headings - Monospace for all code - No ultra-light
weights - Max reading width: 65--75ch

------------------------------------------------------------------------

# 5. Layout System

## Structure

-   Single-column layout
-   Max width: 720px
-   Centered
-   No sidebar

## Spacing System

Base unit: 8px

-   Section spacing: 48--64px
-   Paragraph spacing: 16--20px
-   Code block spacing: 24px

Whitespace is part of the identity.

------------------------------------------------------------------------

# 6. Navigation

Minimal top bar:

-   thelaziest.dev
-   Articles
-   About
-   Now
-   RSS

No dropdowns. No nested navigation.

------------------------------------------------------------------------

# 7. UI Components

## Links

-   Accent color
-   No underline by default
-   Underline on hover
-   Fast transition (\<150ms)

## Buttons

-   Rectangular
-   No pill radius
-   2px border
-   Accent outline or accent solid
-   No drop shadows

------------------------------------------------------------------------

# 8. Code Blocks

-   Same monospace as headings
-   Slightly smaller than body (14--15px)
-   Darker than page background
-   Subtle border
-   No heavy syntax themes

Code must look like a tool, not decoration.

------------------------------------------------------------------------

# 9. Imagery Rules

Allowed: - Terminal screenshots - Minimal diagrams - Geometric line
graphics - Black background visuals

Not allowed: - Stock photos - SaaS vector illustrations - Gradient
blobs - Decorative hero banners

Most posts should not have header images.

------------------------------------------------------------------------

# 10. Micro-Brand Elements

Consistent identity cues:

-   `//` as section separator
-   Muted aphorisms
-   Footer line:

> Built lazily. Shipped aggressively.

------------------------------------------------------------------------

# 11. Accessibility

-   Minimum contrast ratio 4.5:1
-   Avoid pure white on pure black
-   Avoid thin font weights in dark mode
-   Large clickable areas

------------------------------------------------------------------------

# 12. Implementation Constraint

Keep styling simple: - Under 300 lines of CSS - No UI framework
required - No animation beyond hover states - Static site friendly

Consistency \> cleverness.
