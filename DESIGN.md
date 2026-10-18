---
name: Rich Aronson
description: Small moves and clean outs, one guy and a Sprinter van; a quilted moving blanket on an orange ratchet strap.
colors:
  ground: "#142b5e"
  deep: "#0f2350"
  blanket: "#2452b3"
  binding: "#0b1b40"
  strap: "#ff8a1e"
  strap-hi: "#ff9d40"
  on-strap: "#1d1204"
  ink: "#f3f6ff"
  soft: "#bccbf0"
  stitch: "#9fb8f2"
  focus: "#8fd6ff"
  err: "#ffb3a8"
  line: "rgba(188,203,240,.22)"
  line-strong: "rgba(188,203,240,.6)"
  field-fill: "rgba(11,27,64,.55)"
  mustard: "#ecbd58"
  walnut: "#8a5631"
  kraft: "#d3a46b"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(3.4rem, 17.5vw, 7.2rem)"
    fontWeight: 900
    lineHeight: 0.86
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(2rem, 8.4vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(1.45rem, 6.4vw, 2.2rem)"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "-0.01em"
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "clamp(1.08rem, 4.5vw, 1.25rem)"
    fontWeight: 400
    lineHeight: 1.45
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "1.05rem"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "0.06em"
rounded:
  field: "14px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter: "20px"
  gutter-desktop: "36px"
  stack-tight: "10px"
  stack: "18px"
  section: "56px"
  section-desktop: "84px"
  container: "1180px"
components:
  button-primary:
    backgroundColor: "{colors.strap}"
    textColor: "{colors.on-strap}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "58px"
  button-primary-hover:
    backgroundColor: "{colors.strap-hi}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "58px"
  input-text:
    backgroundColor: "{colors.field-fill}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "14px 16px"
    height: "54px"
  chip:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.ground}"
  service-row:
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    height: "78px"
  service-row-arrow:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "48px"
  service-row-arrow-hover:
    backgroundColor: "{colors.strap}"
    textColor: "{colors.on-strap}"
  step-marker:
    backgroundColor: "{colors.blanket}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "52px"
---

# Design System: Rich Aronson

## Overview

**Creative North Star: "The Moving Blanket on a Ratchet Strap"**

The whole page is made of the two things that protect your furniture in the back of Rich's van: a quilted royal-blue moving pad and an orange ratchet strap. The page ground is the pad (drenched navy blues, never black), every section edge is the pad's navy binding with a pale-blue running stitch, and the strap's orange is reserved for the one thing a visitor should do: text Rich. The hero is a live verlet-cloth blanket hung from the strap that drops over a piece of furniture and lifts with it gone ("I can make it disappear"), and the same breeze sways every section divider.

The page is phone-first and dense: heavy uppercase system-sans headings that fill the width, plain sentence-case body, big pill buttons, full-width tappable rows. Warmth comes only from the furniture inside the blanket stage (mustard upholstery, walnut wood, kraft boxes); the chrome never borrows those colors. Depth is quilting and binding, not cards and shadows.

The system rejects the moving-category defaults: cardboard-box icons, truck clip art, stock photos of families carrying a couch.

**Key Characteristics:**
- Drenched blue grounds alternating between pad navy and a deeper panel navy, joined by animated hem dividers.
- One action color (strap orange), used for filled buttons, the phone glyph, headline emphasis words and hovered arrows.
- Heavy uppercase display type (900) in the system font stack; sentence-case body.
- Pills and circles for everything you tap; 14px corners only on text fields and form panels.
- One shared animation loop; cloth and hems both pause off-screen and hold a still frame under reduced motion.

## Colors

A drenched, single-hue blue world with one hot action color and a warm furniture palette confined to the illustration.

### Primary
- **Ratchet-Strap Orange** (strap): the only action color. Filled primary buttons, the header phone glyph, the emphasis word in the hero and closing headlines ("soon?", "Text Rich."), hovered and focused service arrows, the text caret, text selection, and the strap itself in the hero canvas. Lightens to **Strap Highlight** (strap-hi) on hover. Text on orange is **Strap Shadow** (on-strap), a near-black brown, never white.

### Secondary
- **Royal Moving-Pad Blue** (blanket): the quilt fabric. Fills the step-number discs and, in the canvas, the cloth body (rendered in a hue-221 lightness ramp around it).

### Tertiary (illustration only)
- **Mustard Upholstery** (mustard), **Walnut** (walnut), **Kraft Box** (kraft): the furniture the blanket swallows (armchair, dresser, stacked boxes), drawn with gradients and seams. These live only inside the hero stage; no chrome, text or control uses them.

### Neutral
- **Pad Navy** (ground): page ground, the hero and the light-rhythm sections; also `theme-color`.
- **Panel Navy** (deep): alternating section ground (services, how-it-works/quote), still blue.
- **Binding Navy** (binding): the 7px hem binding stroke, the footer ground, inset ring on step discs.
- **Quilt White** (ink): headings, primary text, ghost-button text, selected chip fill.
- **Faded Denim** (soft): secondary text, promise lines, ledes, optional-field hints, footer copy.
- **Stitch Blue** (stitch): the dashed running stitch along every hem (75% opacity).
- **Hairline** (line) and **Strong Hairline** (line-strong): service-row rules and the resting borders of fields and chips.
- **Field Well** (field-fill): translucent binding-navy inside text fields and the sent-message panel.
- **Sky Focus** (focus): form-control hover and focus outlines, and the global focus-visible ring.
- **Soft Coral** (err): inline field errors and the error border.

### Named Rules
**The One Strap Rule.** Orange means "do this." It goes only on actions and on the words that name the action. Non-interactive elements never use it at rest; arrows and icons turn orange on hover, not by default.

**The Never Black Rule.** Every ground is a blue (darkest is binding navy). No black or near-black surface, ever; this is a brand commitment.

**The Furniture Stays In The Blanket Rule.** Mustard, walnut and kraft exist only inside the hero illustration. The page chrome stays blue, white and orange.

## Typography

**Display Font:** System stack (-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif)
**Body Font:** Same system stack

**Character:** One family at two voices: black-weight uppercase with tight negative tracking for anything that sells, plain 17px sentence case for anything that explains. The system stack is a house mandate for speed inside Facebook's in-app browser, not a world-derived choice; weight, case and tracking carry the identity.

### Hierarchy
- **Display** (900, clamp(3.4rem, 17.5vw, 7.2rem), 0.86, -0.035em, uppercase): the hero headline only. One emphasis word in strap orange via upright `em`.
- **Headline** (900, clamp(2rem, 8.4vw, 3.6rem), 0.95, -0.02em, uppercase, balanced wrap): section headings. The closing call scales up to clamp(2.6rem, 12vw, 5.4rem) at line-height 0.9 with its own orange emphasis.
- **Title** (900, clamp(1.45rem, 6.4vw, 2.2rem), 1, -0.01em, uppercase): service row names.
- **Lead** (400, clamp(1.08rem, 4.5vw, 1.25rem), 1.45): hero promise (max 30ch) and section ledes (max 46ch), in faded denim with key phrases bolded in quilt white.
- **Body** (400, 17px, 1.55): everything else; step text is 700 at 1.18rem with a soft supporting line.
- **Label** (800, 1.05rem, 0.06em, uppercase): button text. Form labels and legends are 700, 1rem, sentence case.

### Named Rules
**The Two Voices Rule.** Uppercase 900 sells, sentence case explains. Never uppercase a sentence of body copy; never set a heading in a light weight.

**The Tabular Number Rule.** The phone number always renders with tabular numerals and never wraps.

## Layout

Phone-first single column inside a 1180px container with a 20px gutter (36px from 760px), respecting safe-area insets. Sections pad 56px vertically (84px from 760px) and alternate pad navy and panel navy. Vertical stacks use a tight 10px rhythm for button pairs and chips and 18px between form fields; headings sit 14 to 28px above their content.

First phone screen: wordmark top-left, tap-to-call number top-right (the only phone number on that screen), the display headline, one promise line, two side-by-side 58px pill buttons, then the blanket stage (clamp(280px, 76vw, 380px) tall, bleeding through the gutter to the screen edges) fills the rest.

From 1024px: hero splits copy left / stage right (1fr : 1.05fr, stage 560px); services and specialty go to a 0.8fr : 1.2fr heading-left grid; how-it-works and quote sit in two equal columns. From 760px the hero buttons size to content and paired form fields go two-up. Below 390px the header and button labels tighten rather than wrap, and below 400px the wordmark drops its tagline.

**The No Sticky Bar Rule.** Nothing is fixed to the viewport. The call path is the top-right number; the text path is the hero button, the service rows, the form and the closing button.

## Elevation & Depth

Flat surfaces with material depth. Sections do not lift; they are joined by the hem, an animated SVG edge of the blanket: a wavy fill in the next section's color, a 7px binding-navy stroke along the edge, and a dashed stitch-blue line 8px inside it, all swaying on three layered sines. Only the two filled call-to-action pills carry a shadow, as if resting on the pad. The step discs get their depth from inset binding rings, not a drop shadow.

### Shadow Vocabulary
- **Lift** (`box-shadow: 0 8px 18px -8px rgba(4,12,32,.7)`): filled primary buttons and the Facebook button only. Soft, tinted navy, never a hard offset.
- **Bound Disc** (`box-shadow: inset 0 0 0 3px #0b1b40, inset 0 0 0 5px rgba(159,184,242,.35)`): step-number discs; a binding ring plus a faint stitch ring.

### Named Rules
**The Hem Not Line Rule.** Section changes are always a moving hem divider in the world's own binding and stitch, never a straight color edge or a hairline rule. Flipped hems fill from the section above; the fill color is read from the neighbouring section so the edge never shows a gap.

## Shapes

Round for touch, soft-square for writing. Every button, chip and copy control is a full pill (999px); arrows and step markers are circles (50%); text fields, the textarea and the sent-message panel use gently rounded 14px corners. Borders are 2px everywhere a control has one. The primary pill carries an inner dashed stitch (1.5px, 4px inset, on-strap at 32% opacity) like the stitching on a strap webbing. Service rows have no shape at all: hairlines above and below, nothing around them.

## Components

### Buttons
Big, round, thumb-sized.
- **Shape:** full pill (999px), 58px tall, 2px border.
- **Primary:** strap orange fill and border, on-strap text, uppercase label type, lift shadow, inner dashed stitch. Used for Text Rich (hero, close) and the form submit.
- **Hover / Focus:** hover lightens to strap-hi (hover-capable devices only); press scales to 0.98. Inside the form the submit also takes a 3px sky-focus outline on hover and focus.
- **Ghost:** transparent with a 2px quilt-white border at 55% and quilt-white text; hover firms the border to full ink with a 6% white wash. Secondary hero action only; the hero never holds more than these two buttons and never a Call button.
- **Facebook:** platform-blue pill (#1460cf) with the white "f" mark, 58px tall, lift shadow, placed directly under the specialty copy. A platform-recognition exception, not part of the palette.

### Chips
- **Style:** 48px pills, 2px strong-hairline border, 700 weight, sentence case. Radio choices in the form only.
- **State:** selected fills quilt white with pad-navy text. Hover and keyboard focus add a 3px sky-focus outline (2px offset); no color change on hover.

### Inputs / Fields
- **Style:** 54px minimum (textarea 120px), 14px corners, 2px strong-hairline border, field-well fill, quilt-white 17px text, orange caret, placeholders in #93a6d6.
- **Focus:** hover (hover devices) and focus both swap the border for a 3px sky-focus outline at 2px offset.
- **Error:** soft-coral border plus a plain-language coral line under the field, written in Rich's voice.

### Navigation
- **Header:** not sticky. Wordmark left (900 uppercase name over a 0.75rem tracked uppercase tagline in soft), tap-to-call number right at 800 weight with an orange phone glyph; the number turns orange on hover. Both 44px tap targets.
- **Footer:** binding-navy ground, soft text, name in tracked uppercase, phone and Facebook as 44px links.

### Service Rows
Whole-row text links with one arrow cue.
- 78px rows divided by hairlines; title type on the left, a 48px outlined circle with an arrow on the right (2px border, white at 40%).
- **Hover:** only the arrow changes: it fills strap orange with on-strap arrow. The row never gets a background, border, outline or shadow.
- **Focus:** same arrow fill plus a 3px orange ring around the arrow circle, not the row.
- Each row opens a pre-filled text for that service.

### Step Markers
52px royal-blue discs with a 900-weight counter numeral, bound by a navy inset ring and a faint stitch ring, aligned to the first line of a 700-weight step sentence.

### The Blanket Stage (signature)
A canvas verlet cloth: a quilted royal-blue pad with pale diamond stitching and navy binding, hung from an orange ratchet strap with a grey buckle. It sways on layered-sine wind, follows page scroll, and is pushed by finger or mouse. On a loop it lowers over a mustard armchair, a walnut dresser, or kraft boxes, the piece vanishes with a puff of floor dust, and the blanket lifts empty before the next piece slides in. Dragging the strap down performs the trick by hand; a single strap tug hints at that once per visit. Tunables (cell size, gravity, wind, timing, push reach) are named constants at the top of its script. Under reduced motion it renders one settled frame and the canvas passes vertical scroll through.

## Do's and Don'ts

### Do:
- **Do** keep every ground a blue from the token set; alternate pad navy and panel navy between sections.
- **Do** join sections with the animated hem (fill, 7px binding, dashed stitch) driven by the shared animation loop.
- **Do** reserve strap orange for actions, the action's words in headlines, and hover/focus states of tappable cues.
- **Do** outline every form control (fields, chips, form buttons) in sky focus (#8fd6ff) on hover and focus, and nothing outside the form that way.
- **Do** set selling copy in 900-weight uppercase system sans with negative tracking; explain in 17px sentence case.
- **Do** make tappable things pills or circles at 44px minimum, primary buttons 58px.
- **Do** keep the phone number top-right as a tap-to-call link and the only number on the first screen.
- **Do** pause motion off-screen and hold a still frame under reduced motion.

### Don't:
- **Don't** use a black or near-black ground anywhere.
- **Don't** put orange on anything non-interactive at rest, including service arrows before hover.
- **Don't** highlight a service row on hover; only its arrow fills.
- **Don't** add a sticky bottom bar or any fixed element.
- **Don't** put a Call button under the hero headline or show the number twice on one screen.
- **Don't** use mustard, walnut or kraft outside the blanket stage.
- **Don't** separate sections with straight color edges or hairline rules.
- **Don't** use hard offset shadows; the only drop shadow is the soft navy lift under filled pills.
- **Don't** use cardboard-box icons, truck clip art or stock movers.
