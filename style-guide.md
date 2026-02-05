# cooldad.computer Style Guide
**Version 1.0** | Jekyll Theme Console Base

---

## 1. Brand Overview

### Brand Personality
cooldad.computer is a portfolio for whimsical, purpose-built coding projects that balance technical sophistication with playful irreverence. The brand voice is:
- **Technically competent** but not pompous
- **Self-aware** with a sense of humor
- **Accessible** without being dumbed down
- **Warm** despite the terminal aesthetic

Think: "A senior engineer who builds silly things on weekends and isn't afraid to explain the journey."

### Target Audience
- Fellow engineers who appreciate clever one-off projects
- Technical recruiters looking for creative problem-solving
- Anyone who enjoys the intersection of craft and whimsy

### Design Principles
1. **Let content shine** - The design supports, never overwhelms
2. **Embrace constraints** - Terminal aesthetic is a feature, not a limitation
3. **Warmth through color** - Use the brown/teal palette to soften the monospace starkness
4. **Intentional playfulness** - Quirky content deserves a confident presentation

---

## 2. Color System

### Primary Colors

**Brand Brown (Primary Background)**
- Hex: `#6B4A3A`
- RGB: `rgb(107, 74, 58)`
- Usage: Logo background, accent elements, hover states
- Personality: Warm, grounded, approachable

**Brand Teal (Primary Accent)**
- Hex: `#CFEFF2`
- RGB: `rgb(207, 239, 242)`
- Usage: Logo text, interactive elements, highlights
- Personality: Cool, technical, confident

### Terminal Theme Colors (Console Base)

**Background**
- Dark Mode: `#1a1a1a` (near-black)
- Light Alternative: `#f8f9fa` (off-white, for accessibility)

**Text Colors**
- Primary Text (Dark): `#CFEFF2` (brand teal - high contrast on dark)
- Secondary Text (Dark): `#b5c9cc` (muted teal)
- Muted Text (Dark): `#8a9b9e` (subtle teal-gray)

**Interactive Colors**
- Link Default: `#CFEFF2` (brand teal)
- Link Hover: `#6B4A3A` (brand brown - inverted)
- Link Visited: `#9dc4c8` (muted teal)
- Link Active: `#e8f4f6` (bright teal)

### Semantic Colors

**Success/Complete**
- Color: `#7ac683` (soft green)
- Usage: Completed projects, success messages

**Warning/In Progress**
- Color: `#e5c07b` (warm yellow)
- Usage: Work-in-progress indicators

**Error/Experimental**
- Color: `#e06c75` (soft red)
- Usage: Experimental projects, error states

### Neutral Palette

**Grays (for borders, dividers)**
- Lightest: `#3a3a3a`
- Mid: `#2a2a2a`
- Darkest: `#1a1a1a`

### Color Contrast Ratios
- Brand Teal (#CFEFF2) on Dark BG (#1a1a1a): **15.2:1** ✓ WCAG AAA
- Brand Brown (#6B4A3A) on Light BG (#f8f9fa): **4.8:1** ✓ WCAG AA
- Brand Teal on Brand Brown: **8.9:1** ✓ WCAG AAA

---

## 3. Typography

### Font Families

**Primary Font: Libre Baskerville**
- Usage: Headings, logo, emphasis
- Weights: 400 (regular), 700 (bold)
- Character: Classic, serif, confident
- Rationale: Provides warmth and personality against monospace code

**Secondary Font: Monospace (System)**
- Fallback Stack: `'Courier New', Courier, 'Lucida Console', monospace`
- Usage: Body text, code, terminal elements
- Weights: 400 (regular)
- Character: Technical, authentic, readable
- Rationale: Maintains terminal aesthetic, excellent for code

### Type Scale

**Headings**
- H1: 2.5rem / 40px (Libre Baskerville, 400)
  - Line height: 1.2
  - Usage: Page titles only
  
- H2: 2rem / 32px (Libre Baskerville, 400)
  - Line height: 1.3
  - Usage: Major sections
  
- H3: 1.5rem / 24px (Libre Baskerville, 400)
  - Line height: 1.4
  - Usage: Project titles, subsections
  
- H4: 1.25rem / 20px (Monospace, 400)
  - Line height: 1.5
  - Usage: Minor headings, labels
  
- H5: 1.125rem / 18px (Monospace, 400)
  - Line height: 1.5
  - Usage: Metadata, tags

**Body Text**
- Body Regular: 1rem / 16px (Monospace, 400)
  - Line height: 1.6
  - Usage: Paragraphs, descriptions
  
- Body Small: 0.875rem / 14px (Monospace, 400)
  - Line height: 1.6
  - Usage: Captions, footnotes, metadata
  
- Body Tiny: 0.75rem / 12px (Monospace, 400)
  - Line height: 1.5
  - Usage: Timestamps, micro-copy

### Font Weights & Styles
- Regular (400): Default for all text
- Bold (700): Only for Libre Baskerville in rare emphasis
- Italic: Available but use sparingly (monospace italics can be hard to read)

### Typography Hierarchy Rules
1. **Headings use Libre Baskerville** to break up monospace monotony
2. **Body text uses monospace** to maintain terminal authenticity
3. **Never use more than 2 hierarchy levels on a single screen**
4. **Line length: max 75 characters** for optimal readability

---

## 4. Layout & Spacing

### Grid System
- Container max-width: **800px** (optimized for reading code)
- Gutters: **2rem / 32px** on desktop
- Gutters: **1rem / 16px** on mobile

### Spacing Scale (8px base)
```
xs:  0.5rem /  8px  - Tight spacing (inline elements)
sm:  1rem   / 16px  - Default spacing (paragraphs)
md:  1.5rem / 24px  - Section breathing room
lg:  2rem   / 32px  - Major sections
xl:  3rem   / 48px  - Page sections
xxl: 4rem   / 64px  - Hero spacing
```

### Spacing Usage Rules
- **Between paragraphs:** 1rem (sm)
- **Between sections:** 3rem (xl)
- **Between projects:** 2rem (lg)
- **Padding inside cards:** 1.5rem (md)
- **Margin around headings:** 1.5rem top, 1rem bottom

### Responsive Breakpoints
```
Mobile:  < 768px   (single column, reduced spacing)
Tablet:  768-1024px (optimize for touch)
Desktop: > 1024px   (full layout)
```

### Layout Patterns

**Standard Page:**
```
[Navigation: 60px fixed height]
[Content Container: 800px max-width, centered]
  [Page Title: H1 + subtitle]
  [spacing: xl]
  [Content sections with lg spacing between]
[Footer: minimal, center-aligned]
```

**Project Listing:**
```
[Project Card]
  [Title: H3, Libre Baskerville]
  [spacing: sm]
  [Tags: inline, small]
  [spacing: sm]
  [Description: 2-3 lines max]
  [spacing: sm]
  [Link: "View project →"]
[spacing: lg]
[Next Project Card]
```

---

## 5. Components

### Navigation Bar

**Specifications:**
- Height: 60px fixed
- Background: `#1a1a1a` (solid, no transparency)
- Border-bottom: `1px solid #3a3a3a`
- Position: Sticky top

**Elements:**
- Logo: "cool dad" in Libre Baskerville, brand teal
- Nav links: Monospace, 16px, uppercase
- Spacing: 2rem between links
- Hover: Underline in brand brown

**Mobile Behavior:**
- Collapses to hamburger at < 768px
- Menu slides from right
- Background: same as nav bar

### Project Cards

**Specifications:**
- Border: `1px solid #3a3a3a`
- Border-radius: `4px` (subtle)
- Padding: `1.5rem`
- Background: `#1f1f1f` (slightly lighter than page)
- Transition: `all 0.2s ease`
- Hover: Border changes to brand brown `#6B4A3A`, `box-shadow: 0 4px 12px rgba(107, 74, 58, 0.2)`
- Focus-within: Same as hover (when any link inside card receives focus)

**Structure:**
```
[Project Title - H3 in Libre Baskerville]
[Tags - comma separated, brand teal, 14px]
[spacing: sm]
[Description - 2-3 lines, monospace]
[spacing: sm]
[Link - "View project →" in brand teal]
```

**Tags Format:**
- Display: inline
- Color: brand teal
- Separator: `, ` (comma space)
- Font: monospace, 14px
- No background, no pills

### Buttons

**Primary Button:**
- Background: brand brown `#6B4A3A`
- Text: brand teal `#CFEFF2`
- Font: Monospace, 16px
- Padding: `0.75rem 1.5rem`
- Border: none
- Border-radius: `4px`
- Hover: Background darkens to `#5a3d2f`
- Focus: `2px solid #CFEFF2` outline with `2px` offset + `box-shadow: 0 0 0 3px rgba(207, 239, 242, 0.2)`
- Active: Background darkens to `#4a2f1f`
- Disabled: Background `#3a3a3a`, text `#6a6a6a`, cursor `not-allowed`

**Secondary Button (Link Style):**
- No background
- Text: brand teal
- Font: Monospace, 16px
- Underline on hover
- Focus: same as link focus
- Arrow: ` →` appended

**Button Usage:**
- Primary: Call-to-action (contact, download)
- Secondary: Navigation (view project, read more)

### Links

**Default Link:**
- Color: brand teal `#CFEFF2`
- Text-decoration: none
- Hover: color changes to brand brown `#6B4A3A`, underline appears
- Focus: `2px solid` outline in brand teal, `2px` offset
- Transition: 0.2s ease

**Inline Text Links:**
- Underline: always visible
- Color: brand teal
- Hover: brand brown
- Focus: same as default link

**External Links:**
- Append ` ↗` to indicate external
- Optional: subtle icon

### Interactive States (Accessibility)

**Focus Indicators:**
All interactive elements (links, buttons, form inputs) must have visible focus states for keyboard navigation.

- **Default Focus:** `2px solid #CFEFF2` outline with `2px` offset
- **Button Focus:** Same outline as default, plus subtle glow `box-shadow: 0 0 0 3px rgba(207, 239, 242, 0.2)`
- **Never remove:** `outline: none` without providing alternative focus style

**Interaction State Order:**
1. Default (normal state)
2. Hover (mouse over)
3. Focus (keyboard navigation)
4. Active (mouse down / key press)
5. Visited (for links only)

All interactive elements should provide clear visual feedback for each state.

### Code Blocks

**Inline Code:**
- Background: `#2a2a2a`
- Border: `1px solid #3a3a3a`
- Padding: `0.25rem 0.5rem`
- Font: Monospace, 14px
- Color: brand teal

**Block Code:**
- Background: `#1f1f1f`
- Border: `1px solid #3a3a3a`
- Padding: `1rem`
- Font: Monospace, 14px
- Line numbers: optional, in muted teal
- Max-width: 100% (horizontal scroll if needed)

### Terminal/Console Elements

**Command Prompt:**
```
$ command-here
```
- Prefix `$ ` in brand teal
- Command in white
- Use for demonstrating CLI interactions

**Output Block:**
- Same styling as code block
- No prefix
- May include colored output (success green, error red)

**ASCII Art:**
- Font: Monospace
- Color: brand teal
- Use sparingly for personality
- Keep small (< 10 lines)

---

## 6. Content Guidelines

### Image Specifications

**Project Thumbnails:**
- Aspect ratio: 16:9 or 3:2
- Recommended size: 800x450px (16:9) or 800x533px (3:2)
- Format: JPG or PNG
- Optimization: < 200KB per image
- Alt text: Required, descriptive

**Logo Usage:**
- Primary logo: "cool dad" text on brown background
- Size: 120x60px for nav bar
- Format: PNG with transparency (outside of brown box)
- Always maintain aspect ratio

**Icon Style:**
- Prefer text symbols: `→ ↗ ✓ ✗ ~`
- If icons needed: line style, 24px, brand teal
- Avoid icon libraries if possible (keep it minimal)

### Writing Tone & Voice

**Do:**
- Write like you're explaining to a curious colleague
- Use conversational language ("I built this because...")
- Include honest reflections ("This was harder than expected")
- Embrace technical specificity without jargon-dumping
- Be self-deprecating when earned

**Don't:**
- Use marketing speak or buzzwords
- Oversell the significance of side projects
- Write in third person
- Hide challenges or failures
- Use excessive exclamation points!!!

**Example Project Description:**
```
Good: "A Chrome extension that replaces all instances of 
'synergy' with 'friendship' on corporate websites. Built 
with vanilla JS because sometimes the simple solutions are 
the right ones."

Bad: "Leveraging cutting-edge browser APIs to disrupt the 
corporate communications paradigm through linguistic 
transformation! 🚀"
```

### Project Description Format

**Title:** 
- 3-8 words
- Descriptive but punchy
- Libre Baskerville (let it breathe)

**Tags:**
- 2-5 tags maximum
- Technology: `python`, `rust`, `javascript`
- Type: `tool`, `experiment`, `learning-project`
- Keep lowercase, no special characters

**Description:**
- 2-3 sentences (max 280 characters for scan-ability)
- Structure: What + Why + How (or any two of these)
- Include one technical detail
- Optional: one self-aware comment

**Example:**
```
Title: Potato Quality Classifier

Tags: python, opencv, machine-learning, food

Description: Trained a CNN to classify potatoes as "suitable 
for mashing" vs "suitable for frying" because my wife asked 
me to help with dinner. Achieved 87% accuracy using transfer 
learning on MobileNetV2. The model is more confident than I am.
```

---

## 7. Visual Style Examples

### Homepage Header
```
┌────────────────────────────────────────────────────┐
│                                                    │
│              cool dad                              │
│         (in Libre Baskerville, teal)               │
│                                                    │
│     whimsical code. purpose-built projects.       │
│            (in monospace, muted teal)              │
│                                                    │
└────────────────────────────────────────────────────┘
```

### Project Card Example
```
┌────────────────────────────────────────────────────┐
│ Email Excuse Generator                             │
│ python, api, automation                            │
│                                                    │
│ Generates plausible excuses for delayed email     │
│ responses using Markov chains trained on actual   │
│ out-of-office messages. Surprisingly effective.   │
│                                                    │
│ View project →                                     │
└────────────────────────────────────────────────────┘
```

### Typography Hierarchy Example
```
┌────────────────────────────────────────────────────┐
│                                                    │
│ Projects                                           │
│ (H1, Libre Baskerville, 40px, teal)               │
│                                                    │
│ things i've built for reasons that seemed good    │
│ at the time                                        │
│ (subtitle, monospace, 16px, muted teal)           │
│                                                    │
│ 2024                                               │
│ (H2, Libre Baskerville, 32px, teal)               │
│                                                    │
│ Project Name Here                                  │
│ (H3, Libre Baskerville, 24px, teal)               │
│                                                    │
│ Description text in monospace creates nice         │
│ contrast with the serif headings...                │
│ (Body, monospace, 16px, white-ish)                │
│                                                    │
└────────────────────────────────────────────────────┘
```

---

**End of Style Guide v1.0**