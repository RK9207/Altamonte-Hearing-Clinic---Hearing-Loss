\# Design system — Altamonte Family Hearing: hearing loss

Status: governing visual and interaction direction for Steps 4 and 5\. Prepared October 12, 2026\. This is an implementable specification, not a page build.

Use \[PAGE\_STRATEGY.md\](PAGE\_STRATEGY.md) for section order and conversion decisions and \[CONTENT\_DIRECTION.md\](CONTENT\_DIRECTION.md) for messaging and factual limits. Maintain this system through the complete first draft and interactive rebuild. Significant changes in identity, hierarchy, interaction, or image direction must be explained and approved, then recorded here; ordinary layout tuning within these rules is expected.

\#\# Evidence and design decisions

Research §8 correctly marked typography and most colors as unknown because its fetch was text-only. For this step, the live homepage, its linked stylesheets, the site logo and representative photos were retrieved on October 12, 2026\. The following values are declared in the site's CSS, not inferred from a screenshot:

\- Primary green \`\#006241\`, deep green \`\#004D33\`, night/pine \`\#1A3028\`.  
\- Accent gold \`\#CBA052\`, soft gold \`\#E8D3A6\`.  
\- Cream \`\#FBF8F1\`, paper \`\#FFFDF8\`, mist \`\#DEE7E3\`, mist-deep/line \`\#C9D8D1\`.  
\- Ink \`\#1A3028\`, muted ink \`\#4A5E55\`, on-dark \`\#EEF3EF\`, muted on-dark \`\#C7D6CD\`.  
\- Heading family \`DM Serif Display\`; body family \`Satoshi\`; content container \`1240px\`.  
\- Live radius tokens: 44px, 28px, 18px and pill; photo radius 18px and card radius 28px.

\*\*Source URLs:\*\* \[homepage\](https\://altamontefamilyhearing.com/), \[base stylesheet\](https\://altamontefamilyhearing.com/\_astro/Base.B5jTdihY.css?dpl=6acca7d41ea6d53704f4c03a), \[homepage stylesheet\](https\://altamontefamilyhearing.com/\_astro/index.BEB6x0St.css?dpl=6acca7d41ea6d53704f4c03a), \[additional linked stylesheet\](https\://altamontefamilyhearing.com/\_astro/es.DKGcdjtE.css?dpl=6acca7d41ea6d53704f4c03a). Hashed asset paths can change; obtain current stylesheet links from the homepage rather than relying on these hashes forever.

The token roles, sizing choices, and component rules below are this landing page's design decisions. The site proves the palette and fonts, but it does not designate a single official “secondary brand color.” We assign the brand's \*\*soft gold\*\* to that role because it works accessibly on primary green for the brief's mobile call CTA. Use the deeper gold as a restrained accent. We retain the site's warm serif/sans identity without importing its animations, large navigation menus, or every decorative treatment. No full browser-rendered/computed-style audit was performed; this is stylesheet extraction plus inspection of image originals.

\#\# Brand foundation

| Token/role | Value | Application |  
|---|---|---|  
| Primary brand | \`\#006241\` | Primary CTA on light backgrounds; mobile call-bar background; modest functional emphasis. |  
| Primary hover/deep | \`\#004D33\` | CTA hover/active; deeper green emphasis. |  
| Secondary brand | \`\#E8D3A6\` | Light-gold mobile call text/icon; filled CTA surface against a pine background; gentle highlights. |  
| Accent gold | \`\#CBA052\` | Stars, small rules, restrained decorative details. Not normal-size text on light backgrounds. |  
| Pine/night | \`\#1A3028\` | Main text, dark review or final-CTA surrounds, footer, text on soft-gold buttons. |  
| Page background | \`\#FBF8F1\` | Main warm-cream canvas. |  
| Raised surface | \`\#FFFDF8\` | Header, cards, FAQ panels and scheduler surround. |  
| Supporting mist | \`\#DEE7E3\` | Selected section backgrounds and subtle process groupings. |  
| Soft border | \`\#C9D8D1\` | Quiet card/section dividers. Does not alone provide adequate form-control contrast. |  
| Muted text | \`\#4A5E55\` | Supporting text on cream/paper; never faint gray for essential information. |  
| On-dark text | \`\#EEF3EF\` | Primary copy on pine. |  
| On-dark secondary | \`\#C7D6CD\` | Supporting copy on pine. |  
| Functional input border | \`\#4A5E55\` | App-owned fields and controls where a visible boundary is required. Third-party form styling may be inaccessible. |  
| Focus | \`\#006241\` on light; \`\#E8D3A6\` on dark | 3px visible outline with 3px offset; adapt per surface, not removed on buttons. |  
| Error | \`\#9C2F2F\` | Proposed functional token, not extracted brand color. Pair with explicit message and icon; use on paper. |  
| Success | \`\#006241\` | Proposed semantic use of primary green; pair with text. |

\#\#\# CTA and contrast rules

Primary booking on light: green background, paper text, deep-green hover. On a pine final-CTA surround: soft-gold background with pine text. Secondary CTA: transparent/paper surface, green text and visible green border. Phone links: pine/green text on light; soft gold on pine. The mobile sticky call action specifically uses primary green with secondary soft-gold text/icon, as the brief requires.

Calculated WCAG contrast ratios from the solid tokens:

| Pair | Ratio | Decision |  
|---|---:|---|  
| Paper \`\#FFFDF8\` / green \`\#006241\` | 7.32:1 | Primary button text passes normal-text AA. |  
| Soft gold \`\#E8D3A6\` / green \`\#006241\` | 5.06:1 | Mobile call text/icon passes normal-text AA. |  
| Soft gold \`\#E8D3A6\` / pine \`\#1A3028\` | 9.55:1 | Dark-section CTA and highlights work well. |  
| Muted ink \`\#4A5E55\` / cream \`\#FBF8F1\` | 6.55:1 | Supporting copy remains readable. |  
| Accent gold \`\#CBA052\` / green \`\#006241\` | 3.08:1 | Do not use as normal-size button text. |  
| Accent gold \`\#CBA052\` / cream \`\#FBF8F1\` | 2.28:1 | Decoration only; not essential icons, text, or control boundaries. |

Target AA: at least 4.5:1 normal text, 3:1 large text and essential graphical/control indicators. Recheck actual states, translucent surfaces, image overlays and browser-rendered combinations in Step 4\. Stars may be decorative when an accessible numeric rating is also present. Links in prose are underlined; color alone must not signal link state, error, urgency or success.

\#\# Typography

\*\*Heading font:\*\* DM Serif Display, weight 400\. \*\*Body/control font:\*\* Satoshi, regular 400, medium 500, bold 700 where needed. Fallbacks: \`Georgia, serif\` for headings; \`system-ui, \-apple-system, "Segoe UI", sans-serif\` for body. The logo keeps its own artwork and is not recreated with web type.

The live site preloads \`/fonts/satoshi/Satoshi-Variable.woff2\` and DM Serif Display regular/italic files under \`/\_astro/\`. Prefer the clinic's existing font assets with appropriate usage rights; obtain current URLs for the hashed DM files. Preserve \`font-display: swap\` and metric-appropriate fallbacks so content/actions remain usable if fonts fail. Do not load Google Fonts or multiple unrelated families unnecessarily. Use genuine supplied weights/italic files rather than synthetic styling when possible.

| Style | Desktop ≥1024px | Tablet 768–1023px | Mobile \<768px | Line height |  
|---|---|---|---|---|  
| H1 | 56–64px fluid | 44–52px | 36–42px fluid | 1.08–1.12 |  
| H2 | 38–44px | 34–38px | 28–34px | 1.14–1.20 |  
| H3 | 24–26px | 24px | 22–24px | 1.22–1.30 |  
| Lead/supporting hero | 20px | 19–20px | 18–19px | 1.5–1.6 |  
| Body/reviews/FAQ answers | 18px | 18px | 18px; 17px minimum when justified | 1.6–1.7 |  
| Buttons/navigation | 16–18px, Satoshi 500–700 | Same | 16px minimum | 1.25–1.4 |  
| Small supporting/captions | 15–16px | Same | 15–16px | 1.5–1.6 |

Use rem-based/fluid sizing and allow browser zoom. These are landing-page scales, intentionally somewhat calmer than the live site's largest H1 token (4.6rem). Do not treat desktop sizes as mandatory when a real headline needs a different wrap. Keep one H1, logical H2 sections, and H3 subtopics; do not choose heading levels just for appearance.

Limit paragraph measure to 55–65ch; hero copy about 40–48ch. Left-align reading copy. A centered section title is optional for reviews/final conversion, but long descriptions remain left-aligned. Use modest or neutral heading tracking; no tightly compressed all-caps paragraphs. One short italic phrase in a heading may echo the site identity, but is optional and must not reduce clarity. H1 should usually wrap into two or three lines on desktop and naturally into more on mobile; no forced line breaks that create awkward small-screen fragments.

\#\# Layout and rhythm

| Rule | Specification |  
|---|---|  
| Main container | Maximum 1240px, centered. Hero and split-content interiors may use 1120–1200px for comfortable balance. |  
| Reading/FAQ container | 760–880px maximum; paragraphs still constrained by character measure. |  
| Horizontal gutters | Desktop 32–40px; tablet 24–32px; mobile 20px, 16px only at very narrow widths. |  
| Section vertical padding | Desktop 80–96px; tablet 56–64px; mobile 40–48px. Adjacent short sections may use 32–40px without crushing their hierarchy. |  
| Desktop grid | 12 columns; copy/image splits about 6/6 or 7/5. Use 3 columns for reviews/sign groupings; 2 for specialists. |  
| Tablet grid | 6 columns; retain 2-column arrangements only when copy and faces remain comfortable. Reviews use one column if 3 becomes cramped. |  
| Mobile grid | One column; ordered vertically. Two small utility facts can share a row only if readable without cramped labels. |  
| Grid gaps | Desktop 32–48px for copy/image; cards 24px; tablet 24px; mobile 20–24px. |  
| Internal spacing | 8px base scale: 8, 16, 24, 32, 48, 64, 80, 96\. Caption/image gap 12–16px where needed. |  
| Component breakpoints | 480px narrow-mobile adjustment; 768px tablet; 1024px full desktop header/layout; 1280px large-screen sizing. Break earlier if content collides. |

Use content-driven height, not viewport-height sections. Headings, descriptions, and content groups should have a clear spacing hierarchy; do not give every paragraph the same gap as a section break. Alternate composition rather than alternating colored stripes mechanically.

Suggested rhythm: cream hero → paper/cream signs → mist evaluation → cream care → paper team → pine review surround with paper cards → cream FAQ → mist location → pine final-conversion surround with a paper scheduler → pine footer. Two adjacent similar sections can share a quiet background instead of needing a decorative divider. Keep the embedded scheduler itself on a light surface; never force a dark-mode form through CSS filters.

\#\# Component specifications

\#\#\# Header and navigation

Use an opaque paper header with a subtle bottom border, approximately 88px desktop and 68–76px mobile. Sticky at the top; no shrinking animation that changes touch targets. Original horizontal logo approximately 230–280px desktop; mobile about 150–175px, adjusted for aspect ratio and available width. Preserve clear space and the full mark; do not crop the tagline or recreate the symbol.

Desktop places logo left, four compact section anchors visually balanced in the middle, phone and primary booking right. Mobile presents logo and booking; omit full navigation and desktop phone. Do not reproduce the source site's mega-menu. Anchors account for sticky-header offset. At narrow widths, allow an appropriately smaller logo/button gap before reducing text; test 320px without collision. Keep the visible logo legible; its destination and alt text identify the clinic.

\#\#\# Primary CTA

Satoshi 500–700; exact label \`Book Appointment\`; minimum height 48px, preferred 52px; 20–28px horizontal padding; pill radius. High contrast, no gradient or glossy effect. Use an actual button for dialog opening. Hover changes surface color; focus stays clearly visible; pressed state is subtle without layout shift. Mobile hero action can be full width; the header action remains compact. Disabled/loading states need text and must never be mistaken for success. Do not add animated arrows or change the label into “Free Test.”

\#\#\# Secondary CTA and phone CTA

Secondary outlined action is visually lighter, using the same typography and touch-target height when button-like. Text links need a 44px usable target when isolated controls. Phone links pair a simple phone icon with a readable label/number; \`tel:+14078098154\`. Avoid making the phone visually dominant beside the hero booking button. On pine use soft-gold text, with an obvious focus treatment. \`Get Directions\` and outbound review links are secondary actions with descriptive labels.

\#\#\# Cards

Use cards where content units need boundaries: reviews, selected provider profiles, grouped option facts. Do not wrap every paragraph or symptom in its own elevated box. Paper surface, 1px soft border, 24–32px padding desktop and 20–24px mobile, radius 18–28px. Cards are not clickable unless there is a real destination; no hover lift on static content. Avoid equal-height constraints that create vast blank space or cut content. Use an editorial split or numbered list for explanations when it scans better than a card grid.

\#\#\# Trust badge

Small inline paper/mist unit with “Google,” numeric \`5.0/5\`, star decoration, and \`157 reviews\`; accessible text conveys the full meaning. It must not look like a fabricated certification. Prefer placing it below the hero action or supporting copy, not floating over faces. If positioned on an image, use a fully opaque readable surface and avoid hiding care details. Keep the same aggregate everywhere; no unsupported “\#1 clinic” label or invented Google endorsement.

\#\#\# Review cards

Three paper cards in a desktop row, one column on mobile. Use numeric/accessible individual rating, exact reviewer name, clearly labeled Google source, and body text at the regular reading size. No autoplay carousel or horizontal swipe dependency. Long text may use \`Read full review\` expansion with an explicit control and complete original text; collapse/expand must preserve readable order and keyboard access. Do not reduce type to equalize heights. No fake reviewer portraits; screenshots, if used, remain readable and have equivalent accessible text. Emily's repair context is an adjacent editorial label, not an alteration to her quote.

\#\#\# FAQ

Paper/cream surface, fine separators, 18–20px question text, generous 20–24px vertical spacing, clear plus/minus indicator. Native disclosure or a correctly implemented button/region pattern; controls expose expanded state. Full-width question targets, minimum 48px height. Several items may remain open; avoid closing a reader's answer unexpectedly. The cost answer may start open if that helps the actual first draft. Do not truncate answers on mobile. The urgent-care guidance in S03 remains visible independently.

\#\#\# Forms and booking popup

Use the supplied portal rather than designing a second application form. The fetched clinic \`/schedule\` markup provides an existing implementation precedent: iframe title, \`width="100%"\`, \`height="900"\`, and scrolling enabled. Treat 900px as a starting height, not proof it fits every viewport. Preserve the brief's \`src\` and query string exactly:

\`\`\`text  
https\://myhearingportal.com/?clinic=P2FwaUtleT1TMDd0THc0OEtTNVJROFdDcW1hTU40QWZjRFFCZHdySiZjbGluaWNOYW1lPUZMX2FmaCZmdWxsV2lkdGg9MQ==  
\`\`\`

S10 has a light, wide scheduler surface, clear heading/subheading and preparation/fallback text. Do not wrap it inside a narrow decorative card that restricts the portal. Desktop dialog: up to 960px wide, within viewport gutters, maximum height roughly 90dvh; named heading and persistent accessible close control. Mobile: full-height or near-full-height sheet with safe-area padding and stable internal scrolling. Avoid both an iframe scrollbar and nested wrapper scrollbar where possible; test the real portal before settling height/scroll ownership. Do not impose iframe internals via cross-origin hacks or untrusted message listeners. Use documented, origin-validated resizing events only if supported.

Manage focus entry/return, keyboard navigation, Escape, background inertness and scroll locking. Hide the mobile call bar while the dialog is open; never obscure a field or close control. Preserve entered state across popup/inline presentations as described in strategy. If loading fails, show accessible fallback actions to call or visit \`https\://altamontefamilyhearing.com/schedule\`. Do not show an invented success message or claim a booking from a button click. This system specifies future validation; portal submission has not been exercised in this strategy step.

\#\#\# Location/map block

Desktop: address/hours at left, map at right, approximately 5/7 split. Mobile: address and hours first, then map, then directions button. The directions control sits immediately below the map with a location/direction icon, per the brief. Map frame approximately 16:10 or 4:3, minimum practical height about 280–320px on mobile, radius 18px. Include a meaningful iframe title. The clinic homepage uses \`https\://www\.google.com/maps?cid=12379218337608981477\&z=15\&output=embed\`; verify loading at build time. The brief's original place link remains the directions destination. Text address and directions link must work even if map loading is blocked. No fake exterior image or unverified accessibility icon.

\#\#\# Provider blocks

Two primary specialist profiles with actual portraits, names, accurate titles and concise credential explanations. Keep credentials next to the matching portrait; do not ambiguously attribute Jaysee's certification to the entire team. Portrait crop about 4:5 or native 5:4 where needed; do not distort source proportions. A team photo can replace excessive portrait repetition and support a small coordinator line. Avoid a wall of seals, floating signatures, invented quote bubbles, or “Dr.” labels. HearingUp logo is optional only as an intact sourced mark with appropriate use; the plain-text certification is sufficient.

\#\#\# Final CTA

S10 combines final reassurance and appointment access. A pine surround can provide a strong end-of-page change in emphasis; heading/body use on-dark tokens, scheduler stays paper. A button, if used, is soft gold with pine text and opens the popup consistently. Keep preparation and phone assistance readable. Do not add another “ready to transform your life?” panel after the form.

\#\#\# Mobile sticky call CTA

Below 768px, fixed bottom call bar with green \`\#006241\` background and soft-gold \`\#E8D3A6\` text/icon. One phone action only: \`Call 407-809-8154\`. Control height about 56px plus \`env(safe-area-inset-bottom)\`; body reserves equal bottom space. Use a phone icon plus text, not icon-only. Top booking remains accessible. Hide during the booking dialog and whenever it would obstruct the active scheduler/keyboard; restore without losing page position. At zoom/small landscape sizes, favor content access over keeping both bars visible. Respect reduced-motion preferences; no pulsing attention effect.

\#\# Graphic design principles

\- \*\*Visual personality:\*\* warm, competent, local and personal. Forest green, light gold and cream fit the actual clinic identity; serif headlines give warmth while the sans body stays practical. Avoid futuristic medical graphics, luxury spa styling, or sentimental family stock imagery as the main identity.  
\- \*\*Whitespace:\*\* enough space to separate decisions and keep reading comfortable, without enormous empty hero areas or sparse cards. Whitespace should support useful content, not displace it below oversized photography.  
\- \*\*Contrast:\*\* dark readable text on warm light surfaces, with high-contrast actions. Dark sections are deliberate emphasis points, not alternating obligatory stripes. Essential information never relies on gold-on-cream or translucent image backgrounds.  
\- \*\*Images:\*\* rectangular photos with 18px corners, preserved natural colors, no heavy brand tint. Captions explain real care steps or identify providers; do not invent patient names or outcomes.  
\- \*\*Card usage:\*\* boundaries for parallel evidence/choices; open layouts for narrative explanations. Do not use the same three-card treatment for every section.  
\- \*\*Shadows:\*\* restrained, optional. Source-like soft shadow may use \`0 18px 40px \-22px rgba(26,48,40,.20)\`; use mainly for modal separation or one emphasized card, not all elements. No black glows or exaggerated elevation.  
\- \*\*Borders:\*\* 1px mist-deep for quiet grouping; stronger functional border for controls. Avoid double outlines and decorative frames that reduce image area.  
\- \*\*Corners:\*\* photos/smaller panels 18px; large cards 28px; large section surround up to 44px where it fits; pill actions. Do not give every section rounded corners or force unusual mask shapes.  
\- \*\*Transitions:\*\* clean background changes, spacing, or thin rules. No waves, diagonals, scallops, large blobs or ornamental ear/soundwave patterns.  
\- \*\*Icons:\*\* one consistent simple line-icon family, roughly 20–24px, with matching stroke weight. Pair explanatory icons with labels; mark redundant ones decorative. No emoji as clinical credibility or inconsistent icon sets.  
\- \*\*Motion:\*\* content visible without animation; optional brief 150–200ms color/disclosure transitions. No parallax, auto-playing video/audio, scroll-triggered content hiding or mandatory hover discovery. Reduced motion must preserve the entire experience.

\#\# Image system

\#\#\# Source preference and inspected assets

Real clinic, team, equipment and appropriately supplied GBP photography takes priority wherever an image implies who provides care, where care occurs, or what the clinic does. During this step the following original site assets were actually retrieved and visually inspected; these are firmer choices than descriptions alone:

| Asset | Intended role | Crop/use direction |  
|---|---|---|  
| \[Site logo\](https\://altamontefamilyhearing.com/assets/logo-altamonte-626.png) | Brand identity; genuine green horizontal logo. | Preserve full artwork/aspect ratio and legibility. The brief-hosted asset returned 403 and has not been visually compared. Use this site logo as the drafting fallback, not as a claimed inspection of the supplied file. |  
| \[AFH-C-28.webp\](https\://altamontefamilyhearing.com/assets/photos/AFH-C-28.webp) | Hero or evaluation: Jaysee performing an ear exam with a smiling patient. | Primary hero recommendation, subject to responsive crop checks. Native landscape suits a desktop split. Keep ear, hands and procedure context intact; move the face away from any badge. |  
| \[AFH-B-3.webp\](https\://altamontefamilyhearing.com/assets/photos/AFH-B-3.webp) | Results explanation and personal care: Jaysee holding an audiogram. | Native portrait; strong S04 supporting image or hero alternative. Maintain the chart and facial context; do not claim the pictured example is the visitor's result. |  
| \[AFH-C-196.webp\](https\://altamontefamilyhearing.com/assets/photos/AFH-C-196.webp) | S05 method explanation: actual REM probe placement. | Native landscape; show provider hands and ear/probe context. Plain caption explains measuring sound in the ear. |  
| \[staff-AE8A1554-3.webp\](https\://altamontefamilyhearing.com/assets/photos/staff-AE8A1554-3.webp) | S06 team credibility; real clinic sign/location context. | Native landscape; retain all four people. Do not squeeze into a portrait crop that cuts out staff. Use a caption or adjacent named profiles, not guessed left-to-right identities. |

Research §9 also lists sound-booth photos, specialist portraits, fitting images, white logo and additional clinic assets. They are candidates, not all inspected assets. Inspect the selected originals before use. There are no local original review screenshots or supplied GBP images; research contains transcriptions of the former. GBP/exterior photos can later improve S09 wayfinding, but their absence does not require fabricated replacements.

\#\#\# AI-generated and editorial imagery

AI-generated lifestyle/editorial imagery may be appropriate only for a supplementary everyday listening context when real supplied imagery cannot meet that role. Label it as illustrative when its context might imply a real patient; never suggest it documents this clinic or an actual result. The first draft can be complete using available real clinic photos, so generated imagery is not required.

Never generate or cosmetically invent the clinic, providers, patient testimonials, equipment used by the clinic, credentials, map, exterior/entrance, or clinical before/after evidence. Never put hearing devices or procedures into generated photos if their anatomy/placement would need factual verification. Avoid generic silver-haired couples gazing at sunsets, excessive smiling, plastic skin, staged handshake scenes, uncanny ears/hands, glowing soundwaves, artificial bokeh, and implausibly spotless equipment scenes. Select ordinary, believable activities and varied adult ages when an editorial context is useful.

\#\#\# Cropping, composition and pairing

\- Desktop hero: landscape or near-square crop in a roughly 45–50% image column; preserve provider/patient interaction. Mobile: lower-height 4:3/3:2 crop after copy and CTA, not a full-screen portrait that delays information.  
\- Process/REM: 3:2 or 4:3 whenever it preserves the relevant hands/equipment; inspect \`object-position\` at each breakpoint. Team: native landscape. Specialist portraits: about 4:5, adjusting to the actual asset.  
\- Use one image per important proof/explanation role, not a photo beside every small paragraph. S03 and FAQ do not need decoration to feel complete.  
\- Pair image and explanation closely; mobile DOM order follows the argument rather than alternating image-first sections mechanically. Avoid captions separated from their image by unrelated content.  
\- Rounded photo corners are suitable. Overlays are generally unnecessary; if a badge sits nearby, prefer a separate surface. Never overlay small text on busy photography or crop out relevant clinical context to make space.  
\- Caption procedural images when the method would otherwise be unclear; caption portraits accurately. Alt text describes the image's purpose without introducing unsourced titles, diagnoses or outcomes. Decorative images can have empty alt text.  
\- Do not repeat the same hero photo throughout the page. Do not over-sharpen, apply skin smoothing, or alter uniforms/signage to fit the palette.  
\- Deliver suitable responsive image sizes, dimensions and modern formats; eager-load the actual hero image, lazy-load below-fold images. Do not preload every source asset or treat a massive original as the mobile delivery file.

\#\# Responsive hierarchy

Mobile changes reading order and priority, not just font size. The first view should establish clinic/topic, a clear benefit, booking, and proof; photography follows when space requires it. A full-screen hero image, dense header, or large slogan must not displace the action.

| Desktop treatment | Mobile treatment |  
|---|---|  
| Logo \+ balanced anchors \+ phone \+ booking | Logo \+ compact booking only; secondary phone in required bottom bar. |  
| Hero copy/image split | Copy → booking/call option → trust cue → compact real image. |  
| Four horizontal process steps | Vertical numbered sequence with explanatory text; no horizontal timeline scrolling. |  
| Care copy plus REM photo/benefit groups | Core benefit/mechanism first, image/caption next, supporting selection/aftercare below. |  
| Two specialist profiles/team composition | Stacked profiles; titles/credentials remain beside their names; no tiny multi-person montage. |  
| Three review cards in a row | Three stacked readable cards with complete-text expansion. |  
| FAQ container and surrounding space | Full-width question targets; same substantive answers; no reduced type to shorten the page. |  
| Address/hours beside map | Address/hours → map → directions; scheduling remains next. |  
| Wide appointment area/dialog | Full-width light scheduler; usable viewport-height dialog and close control; call bar suppressed when necessary. |

At 200% zoom, reflow rather than clipping. Support at least 320px widths and test small landscape viewports, sticky-header anchor offsets, virtual keyboard, safe areas and long labels. No fixed-height text cards, forced desktop line breaks, horizontal page overflow, or tiny multi-column mobile grids. Essential cost, medical-urgency and credential information must survive every breakpoint.

\#\# Step 4 implementation and Step 5 review criteria

The implementation should demonstrate this system through the real content and assets. Validate contrast/focus states, logical headings and reading order, keyboard disclosure/dialog controls, legible imagery, review integrity, consistent phone/rating values, scheduler/map fallbacks, and small-screen content access. Do not claim booking completion merely because the iframe loads.

When reviewing the first draft, first ask whether the hierarchy makes the evaluation clear, proof is credible, explanations are useful, and actions are easy to use. Tighten layout and copy after seeing those relationships. A different crop, spacing adjustment or headline wrap is ordinary refinement. A new brand palette/font, fabricated image direction, deleted objection content, competing lead form, changed CTA behavior or significant section reordering is a meaningful departure requiring explanation and user approval before it becomes the new governing choice.

