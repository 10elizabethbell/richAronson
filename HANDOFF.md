# Rich Aronson (small moves + clean outs) — handoff at ~60%

**Live:** https://10elizabethbell.github.io/richAronson/ · **Repo:** https://github.com/10elizabethbell/richAronson · **Built:** 2026-10-18 from Muse brief of 2026-10-18 (Facebook group ad, cross-posted in two NJ groups)

## What's built
- One page, single `index.html`, phone first. Header: "Rich Aronson / Small moves & clean outs" wordmark left, 732-682-7345 (tap to call) top right.
- Hero: "MOVING SOON?" (Rich's own opener), one promise line, **Text Rich** (orange, pre-filled SMS, stitched edge) + **What I do** (outlined, jumps to services), side by side on phones so the whole trick fits Facebook's in-app first screen (checked at 390×664 and 360×664).
- **Signature element:** a quilted blue moving blanket (verlet cloth) hanging from an orange ratchet strap. It plays Rich's line "I can make it disappear" by itself: lowers over a piece of furniture (armchair, dresser, box stack), the piece shows through the cloth, then the blanket sinks flat with dust spilling from the hem, lifts, and the next piece slides in. Finger or mouse pushes the cloth in every direction; dragging the strap pulls the blanket down by hand; a tap starts the trick; the strap gives one small tug after the first trick to hint it's pullable; scrolling swings the blanket a little. Tunable constants (timings, wind, gather, push) sit at the top of the cloth script. Reduced motion: one still frame, and the stage scrolls normally.
- Section dividers are the blanket's hem (navy binding with stitching) swaying in the same breeze.
- What I do: Small moves / Clean outs / Furniture removal, each row a pre-filled text.
- Small moves are my specialty: care line, the "disappear" line, the clean-out rule ("you get the dumpster, and I provide the labor to fill it"), and a big "See more on my Facebook" button.
- How it works (3 steps).
- Get a price by text: short form (job type chips, from/to, when, what's going, name) that writes the text message for the customer and opens their texting app; shows the message with a copy button as a fallback.
- Close ("Moving soon? Text Rich." + call line), footer with name, phone, Facebook. No email (none exists).

## Assumptions I made
- **Name on the site is "Rich Aronson"**, his real name, because no business name is published. Muse: don't ship under a made-up name. If Rich has a business name, it replaces the wordmark, `<title>`, og tags and footer.
- **Colors:** no logo or brand colors exist. Moving-pad blue and ratchet-strap orange were chosen from the trade itself.
- **Favicon/home-screen icon:** no logo, so it's an "R" on a quilted blue square with the orange strap.
- **"New Jersey"** appears in the footer and meta description, inferred from the 732 area code. No towns are on the page.
- **Voice:** first person "I" for the promise (his ad mixes "we" and "I"). If he works with a helper, "I pull up with the van and do the lifting" should become "we".
- **How it works** steps are generic to how a texted small-move job goes (text details, pick a day, show up). Step 2 avoids claiming he quotes by text, but the form is titled "Get a price by text"; confirm he quotes that way.
- **Specialty copy** ("A small move is still your whole life in the back of my van. I take it piece by piece and treat every one like it's going into my own house.") is written in his voice about care; it is not something Rich said. Check it sounds like him.
- Customers are not assumed to be 40+, so the page has the full signature motion.

## Placeholders and gaps
- **Business name** (needed before delivery).
- **Photos: none.** The ad's flyer image is behind Facebook's login wall and couldn't be downloaded. Photos of the van (with plates blurred), Rich, and real jobs would help the most. A photo of the actual Sprinter could replace one of the drawn furniture pieces or sit in the specialty section.
- Service towns, hours, prices, email, Instagram, reviews: none published, none on the page.
- Facebook link points at Rich's **personal profile** (no business page exists). Confirm he wants that public on the site.

## Questions for the owner
1. What's the business called, if anything?
2. Which towns or how far do you go?
3. Is it just you, or do you bring a helper?
4. Do you quote by text from a list and photos?
5. Can I use a few photos of the van and past jobs?
6. Days and hours you take jobs? Do you do same-day?
7. Do you haul furniture to donation or the dump, and do you charge for it?
8. OK to link your personal Facebook, or do you want a business page?

## Impeccable sweep and finish review
- Ran every mode except `live` and `onboard` (no first-run flow): critique, audit, harden, optimize, adapt, polish, layout, typeset, colorize, clarify, distill, extract, animate, delight, bolder, quieter, overdrive. Fixes applied, then the finish reviewer ran twice.
- Final verdict: **fix**, with three items still open after the two rounds an unattended run gets:
  1. **Drape:** when the blanket is lowered, its outline stays a rectangle. The chair shows only as a lighter band, not as a back hump and arm shoulders. A real fix probably means colliding the cloth with the piece's outline or warping the hem around it.
  2. **Fold shading:** on desktop, especially when the blanket is collapsed, the shading still looks faceted, and at 2x faint square blocks show in the quilt. Smoothing it needs per-pixel light (e.g. a low-res light canvas, blurred and multiplied) or a finer mesh.
  3. **Desktop dead space** in the left column under How it works, next to the form.
- Things the reviewer thought could go further (not required): strap or buckle details on the buttons and arrows, quilt texture on section grounds.
- Detector flags I suppressed (in `.impeccable/config.json`): overused-font=roboto (the house font stack), cramped-padding on `.rows` and `section.deep` (a ruled list and a full-bleed band), flat-type-hierarchy (the detector ignores the clamp() headings).

## Ideas not built (yours to pick)
- **Runner-up world:** a curbside hand-lettered sign world (marker on cardboard, "FREE" curb furniture), the assigned roll before the cloth challenger beat it. Others on the list: NJ Turnpike/Parkway guide signs, the Sprinter's cargo bay (E-track rails and tie-downs), bubble wrap you can pop.
- The blanket could drape over a drawing of the Sprinter's open back doors on the specialty section, or over a real van photo once we have one.
- Let the visitor pick which piece goes next (tap a chip: couch, mattress, TV).
- A "what I take" list for furniture removal once Rich says what he will and won't haul.
- A ratchet "click" (a buckle kick plus `navigator.vibrate(6)` on Android) for each notch as the strap is pulled.
- The incoming piece tips slightly as it's carried in and settles with a small wobble.

## Not verified
- Real-device touch (iPhone Safari, Android Chrome, Facebook's in-app browser): tested only with simulated pointer events in headless Chrome.
- SMS handoff on real iOS/Android (the `sms:+1…?&body=` form is the cross-platform pattern but untested on device).
- Frame rate of the cloth on old phones (about 700 cloth points on a 390px phone).
