# IMAGE_PROMPTS.md: Altamonte Family Hearing, hearing loss

Status: Step 4B reference for Step 5. Prepared October 13, 2026, from the Step 4A `index.html` draft.
Governing documents: PAGE_STRATEGY.md, CONTENT_DIRECTION.md, DESIGN_SYSTEM.md, RESEARCH.md.

If a section's layout, crop or visual purpose changes materially in Step 5, update its entry here instead of leaving it stale.

---

## How to read this file

**Scope.** The Step 4A page has six image slots, each tagged `data-img="..."` in the HTML. Two are true placeholders (`IMG-PROVIDER-01`, `IMG-PROVIDER-02`). Four already carry real clinic photos from the design system's inspected asset list (`IMG-HERO-01`, `IMG-CLINIC-01`, `IMG-CLINIC-02`, `IMG-TEAM-01`). All six are covered, with exactly three options each. No section without an image slot has an entry.

**Real imagery rule.** DESIGN_SYSTEM.md says real clinic, team, equipment and provider photography takes priority wherever an image implies who provides care, where care happens or what the clinic does. It also says never to generate the clinic, providers, equipment used by the clinic, credentials, an exterior or entrance, or clinical before/after evidence. This changes what "three prompt options" means in two places:

- **Everyday-context slots (hero):** the options are true text-to-image prompts for *illustrative* lifestyle images. The real photo remains the recommendation.
- **Slots that depict real people, equipment or the clinic (providers, team, audiogram review, Real Ear Measurement):** the options are either image-edit prompts that use the real photo as the input, or non-depictive conceptual images. None of them invent a person, a device or a procedure.

**Shared look (all generated or edited images).** Natural, unretouched color. Forest green, cream, soft gold and warm neutrals may appear in the environment (linen, foliage, wood) but are never applied as a color grade. Real skin texture, candid body language, adults of varied ages, nothing staged for the camera. Healthcare advertising that feels local and personal, not luxury spa and not hospital.

**Shared negative prompt (append to every text-to-image prompt).**
`no text, captions, signage, logos, watermarks or brand names; no stock-photo handshakes, thumbs-ups or exaggerated grins; no stethoscopes, syringes, hospital beds or sterile corridors; no glowing soundwaves, bokeh orbs, lens flare or HDR glow; no plastic or over-smoothed skin; no distorted ears, fused or extra fingers, mismatched earrings or asymmetric eyes; no before/after split; no hearing devices unless the prompt asks for them`

**Image-edit rule (all edit prompts).** Upload the real photo as the reference input. The person's face, hair, ears, any worn hearing aids, clothing and uniform must stay identical. Do not smooth skin, change expression, or alter signage.

**Disclosure.** Any generated lifestyle image that could be read as a real patient or real clinic scene should carry a short "Illustrative image" caption.

## Slot summary

| ID | Section | Current state in Step 4A | Recommended source |
|---|---|---|---|
| IMG-HERO-01 | S02 Hero | Real photo `AFH-C-28` wired in | Real clinic image preferred |
| IMG-CLINIC-01 | S04 Evaluation | Real photo `AFH-B-3` wired in | Real clinic image preferred |
| IMG-CLINIC-02 | S05 Verified fitting | Real photo `AFH-C-196` wired in | Real clinic image preferred |
| IMG-TEAM-01 | S06 Team | Real photo `staff-AE8A1554-3` wired in | Real team image preferred |
| IMG-PROVIDER-01 | S06 Team (Jaysee) | Placeholder | Real provider image preferred |
| IMG-PROVIDER-02 | S06 Team (Toni) | Placeholder | Real provider image preferred |

---

## IMG-HERO-01 - S02 Hero

### Placeholder purpose
Give the first screen a human, believable reason to trust the clinic. The image supports the headline about following conversations and starting with a hearing evaluation in Altamonte Springs. It must not delay the booking action, and it must not imply a hearing aid has already been prescribed or promise an outcome. The benefits stay in the page text, not in the image.

### Recommended source type
Real clinic/GBP image preferred. AI-generated lifestyle/editorial images are appropriate only as an illustrative alternative.

### Recommended composition
- **As built:** a two-column hero. The image frame is 5:6 portrait on desktop (1024px and up), 4:3 on tablet and 3:2 on mobile, using `object-fit: cover`.
- **Generate one master at 3:2 landscape (at least 3000 × 2000)** with the main subjects inside the central 60% of the width. That region survives all three crops. The 5:6 desktop crop removes a lot of the left and right edges.
- No negative space is needed, because the copy sits in its own column. Keep faces away from the bottom edge, where the trust badge is nearby.
- **Mobile:** the image sits below the copy and CTA, so it can be less dramatic and should read clearly at roughly 350px wide.
- **Note on the example in the brief:** the 16:9 "subject right, negative space left" layout does not match the implemented split hero. Use the 3:2 master above.

### Option 1 - Lifestyle outcome: the easy conversation
Candid editorial photograph of a man in his late 60s and a woman in her early 60s seated at a small round table on a shaded Florida lanai, mid-conversation over iced tea. He leans slightly forward, listening with a relaxed, engaged expression. She is mid-sentence with a gentle, natural smile. Linen shirt and a soft cotton cardigan in sand, cream and muted sage. Late-morning diffuse light through a screen enclosure, lush green foliage softly out of focus behind them. Eye-level camera, 50mm lens at f/2.8, shallow depth of field, both faces sharp. Subjects centered within the middle 60% of a 3:2 frame. Calm, connected mood. Natural skin texture, muted film-like color, no color grade. Realistic hands. No hearing aids visible, no medical props. Authentic editorial healthcare advertising, not stock.

### Option 2 - Family-assisted: an adult child beside a parent
Documentary-style photograph of a woman in her mid 40s sitting close beside her father, early 70s, on the steps of a suburban Central Florida porch. She speaks near him with a patient, warm expression while he listens with a wry half-smile. Casual everyday clothing in cream, denim and soft green, nothing coordinated. Soft early-evening side light, gentle warm tones, plants and a wooden railing out of focus behind. Slightly low, eye-level framing, 35mm lens at f/2.8, subjects in the central 60% of a 3:2 frame. Emotional tone is quiet support, not worry. No medical props, no brochures, no hearing aids visible. The Hispanic family detail is optional, since the clinic offers care in Spanish. Natural skin, realistic hands, candid body language.

### Option 3 - Premium editorial: the attentive listener
Tight editorial portrait of a woman in her late 50s with silver-streaked hair, head tilted slightly, eyes directed toward someone just off-frame, listening with the beginning of a smile. Soft window light from the left, warm neutral interior blurred behind her with a hint of a green armchair and wood. Open-collar linen shirt in oat. 85mm lens at f/1.8, shallow depth of field, her face near the center of a 3:2 frame with quiet space on both sides so the 5:6 desktop crop stays clean. Understated, intimate, high-end magazine feel. Natural skin texture with fine lines kept, no retouch gloss. No hearing aids, no jewelry that draws attention.

### Recommended option
**Keep the real photo (`AFH-C-28`).** If an illustrative alternative is wanted, use **Option 2**. It speaks to the family members the strategy names as the second audience, and it keeps the page from implying a clinical scene that was not photographed at the clinic. Option 1 is the safest fallback for the primary audience of adults noticing gradual difficulty.

### Real-image note
**REAL CLINIC / GBP IMAGE PREFERRED.** `AFH-C-28` shows the provider, the actual ear exam and a smiling patient. It carries local, real-care trust that a generated lifestyle image cannot. Do the responsive crop checks on it, since the face and procedure context must survive the 5:6 desktop crop and sit away from the badge. Use a generated image only if the real photo's rights or quality fail.

---

## IMG-CLINIC-01 - S04 Evaluation and results

### Placeholder purpose
Support the numbered four-step process by making the results review feel personal and understandable. It is not a fifth step and it does not depict the visitor's own result.

### Recommended source type
Real clinic/GBP image preferred. AI-generated conceptual/illustrative images are acceptable only as non-depictive alternatives.

### Recommended composition
- **As built:** 4:5 portrait on desktop, sticky beside the steps. 3:2 on mobile and tablet, placed after the steps.
- Native portrait source (`AFH-B-3`). Keep the audiogram and the provider's face and hands in the frame. On mobile, the 3:2 crop must still read as someone explaining a chart.
- A generated alternative should be a 4:5 portrait master with a quiet upper third, so the 3:2 crop can be taken from the middle.

### Option 1 - At home: taking the information with you
Documentary photograph of an adult daughter in her early 40s and her father in his early 70s at a wooden kitchen table, reviewing a paper folder and a handwritten notepad after an appointment. Her hand rests lightly on the page and he looks at it thoughtfully. The pages are not readable and show no charts or text. Late-afternoon window light, a green plant and a ceramic mug, warm neutral kitchen. 40mm lens at f/3.2, camera slightly above eye level, 4:5 portrait with the subjects in the middle two-thirds. Calm, unhurried mood that supports "you can take the information home and decide." No doctors, no clinic, no medical props.

### Option 2 - Hands-only: walking through a page
Close-up photograph of two sets of hands over a plain printed page on a light wood desk, one adult hand pointing with a pen to a blurred area and the other hand resting beside it. The page content is unreadable and abstract, with no numbers, no chart curves and no text. A pair of reading glasses and a small plant sit softly out of focus at the edge. Soft north-facing window light, 65mm macro-feel lens at f/2.8, top-down at a slight angle, 4:5 portrait. Warm neutrals with a touch of sage. Human and unhurried, with no faces and no identifiable clinic. Natural skin texture and hands, realistic nails.

### Option 3 - Conceptual: hearing across pitches
Flat vector editorial illustration on a cream background (#FBF8F1). A simple, abstract horizontal band of thin pine-green (#1A3028) lines of varying length suggesting "pitch from low to high", with a single soft-gold (#CBA052) accent mark and a small primary-green (#006241) dot. No axes, no numbers, no labels, no text, and no recognizable audiogram symbols. Generous negative space, a calm and calm-clinical feel, rounded line ends, 4:5 portrait. It must not read as a medical chart and must not imply any test result.

### Recommended option
**Keep the real photo (`AFH-B-3`).** If a replacement is ever needed, **Option 1** best matches the content direction's "you can take the information home and decide" and shows the family-member support the page describes. Option 3 is a useful fallback only if a quiet, non-photographic treatment is wanted.

### Real-image note
**REAL CLINIC / GBP IMAGE PREFERRED.** An image of the provider explaining an audiogram directly answers the visitor's question, "will someone explain the results?" A generated image cannot show the real person or the real review. DESIGN_SYSTEM.md also forbids invented audiograms and before/after evidence. Caption the real photo as an example, not the visitor's result.

---

## IMG-CLINIC-02 - S05 Verified fitting (Real Ear Measurement)

### Placeholder purpose
Make the clinic's main care differentiator concrete: sound measured in the person's own ear, with the aid in place. It accompanies the measure, adjust and re-check explanation and needs a plain caption.

### Recommended source type
Real clinic/GBP image preferred. A non-depictive conceptual image is the only acceptable AI alternative.

### Recommended composition
- **As built:** 4:5 portrait on desktop (sticky), 3:2 on mobile and tablet.
- Native landscape source (`AFH-C-196`). The provider's hands and the ear/probe-tube relationship must stay visible. Check `object-position` at each breakpoint, since the 4:5 desktop crop can cut off the context.
- A generated alternative should leave quiet space in the lower third for the caption.

### Option 1 - Simple explanatory diagram (requires clinic review)
Minimal flat vector illustration on a cream background. A simplified side-profile outline of an ear in soft pine-green line work, a thin pale-gold line suggesting a probe tube entering the ear canal, and a small rounded generic device shape at the ear. Two or three gentle curved lines in primary green suggest sound reaching the ear. No text, no labels, no numbers, no brand marks. Anatomically restrained, with no cross-section detail. 4:5 portrait, generous negative space. Non-diagnostic and unlabeled. **The clinic must review the final image for anatomical and procedural accuracy before use.**

### Option 2 - Still life: calibration
Macro still-life photograph of a brass tuning fork resting on a folded cream linen cloth on a pale wooden surface, window light from the upper left casting a soft shadow. 100mm lens at f/3.5, very shallow depth of field with the fork's tines in focus, gentle warm neutral background with a touch of sage. 4:5 portrait, quiet negative space at the bottom. Calm, precise and craft-like. It signals accuracy and tuning without showing any clinical device. No hearing aids, no probe tubes, no ears, no hands, no text.

### Option 3 - Three-step visual metaphor
Flat editorial illustration of three simple, abstract rounded shapes arranged left to right on a cream background, connected by a thin soft-gold line: the first a small circle, the second an adjustable slider-like capsule, the third a circle with a quiet check-like curve. Pine-green and primary-green palette with one soft-gold accent. No text, no numerals, no icons that suggest a specific medical device. Generous negative space, 4:5 portrait, calm and precise. It stands for "measure, adjust, re-check" without depicting any equipment.

### Recommended option
**Keep the real photo (`AFH-C-196`).** If it fails technically, use **Option 1** after clinic sign-off, since it explains the idea most directly. Option 2 is the better fit for a quiet, premium mood if the page later drops the literal image.

### Real-image note
**REAL CLINIC / GBP IMAGE PREFERRED.** A photo of the actual probe-tube measurement is the proof of method. DESIGN_SYSTEM.md bars generated procedures and equipment that the clinic would have to verify, and any substitute would weaken the credibility this section exists to build.

---

## IMG-TEAM-01 - S06 Team photo

### Placeholder purpose
Show the real people behind the care and connect them to the clinic's local setting. It supports the "independent, family-owned" message beside the named profiles. It is not a stand-in for the individual portraits.

### Recommended source type
Real provider/team image preferred. No AI-generated version is appropriate.

### Recommended composition
- **As built:** native landscape, uncropped, all four people in frame, on the right of the section on desktop and stacked on mobile.
- Do not squeeze it into a portrait crop. Do not guess left-to-right names in the caption.
- Any edit must keep the clinic sign and the four team members intact.

### Option 1 - Light finishing edit of the real photo
Image-edit prompt using the real team photo as the reference input. Apply a gentle, natural tonal balance: recover highlight detail in the white coats, lift shadows slightly, correct the white balance toward neutral warm so skin tones read true and the green scrubs and sign keep their real color. Do not smooth skin, alter faces, expressions, uniforms, the sign or the background. Keep the native landscape aspect ratio and original framing. Output at 2400px wide, slight sharpening only.

### Option 2 - Canvas extension for flexible cropping
Image-edit prompt using the real team photo as the reference input. Extend the canvas by about 12% on the left and right only, filling with a plain continuation of the existing wall and floor so a 3:2 or 16:9 crop is possible without cutting anyone off. Do not add people, objects, signage or text. Do not change the four people, the sign, lighting or color. Keep the seams invisible. Output at 3:2.

### Option 3 - Fresh-shoot direction (human photographer, not AI)
Photography brief for a new group photo in the actual office: the four team members standing loosely in front of the clinic sign, relaxed and not lined up in a row, natural conversation or a brief laugh, wearing their usual white coats and green scrubs. Soft, even daylight from the front window plus fill, 35mm lens at f/4 for context with faces sharp, camera at chest height, landscape 3:2 with a little space around the group. Capture two frames: a posed one and a candid one. Add a vertical alternate for stacked mobile layouts. No stock-photo poses and no props.

### Recommended option
**Option 1.** The current photo already matches the design system's team treatment. A light finishing edit is the lowest-risk improvement. Use Option 2 only if the Step 5 layout needs a wider crop. Option 3 is worth requesting if the client can arrange a shoot.

### Real-image note
**REAL TEAM IMAGE PREFERRED, AI NOT ACCEPTABLE.** DESIGN_SYSTEM.md forbids generating the clinic's providers, and a team photo is the core proof of who is providing care. Do not generate or composite faces.

---

## IMG-PROVIDER-01 - S06 Team: Jaysee A. Soto portrait

### Placeholder purpose
Put a face to the owner's credentials (HAS, BC-HIS, HearingUp Certified Provider) so the visitor can recognize who will care for them. The credentials sit beside the portrait in text.

### Recommended source type
Real provider image preferred. The site already has a white-coat portrait (`jaysee-portrait.webp`, `jaysee-about.webp`). Needs to be inspected and cleared for use.

### Recommended composition
- **As built:** 4:5 portrait. About 96px wide beside the name on mobile and 170 to 190px wide beside the text on tablet and desktop.
- Head and shoulders, with eyes roughly in the upper third. Keep the white coat visible, since it is part of the real photo, but never add a title or label that says "Dr."
- Leave a little headroom so the 4:5 crop and the 96px mobile thumbnail both stay readable.

### Option 1 - Background normalization
Image-edit prompt using the real portrait of Jaysee A. Soto as the reference input. Replace only the background with a soft, out-of-focus warm neutral tone (light sage-cream), with a subtle gradient and realistic depth falloff so edges around the hair and white coat stay natural. Do not change his face, hair, ears, expression, white coat, posture or lighting on the subject. No smoothing, no slimming. Output 4:5 portrait, at least 1200 × 1500.

### Option 2 - Recompose to 4:5
Image-edit prompt using the real portrait as the reference input. If the original is not 4:5, extend the canvas upward and sideways to create a 4:5 head-and-shoulders composition with comfortable headroom, continuing the existing background naturally. Keep his face, hair, coat and expression exactly as shot. Do not add objects, text, badges or logos. Maintain the original lighting direction. Output 4:5 portrait at 1200 × 1500.

### Option 3 - Matched-pair harmonization
Image-edit prompt using the real portraits of Jaysee A. Soto and Toni Trager as reference inputs. Harmonize exposure, white balance and background tone so the two portraits look like one set. Use the same soft neutral background value, matching contrast and warmth. Do not alter either person's face, expression, hair, uniform or any worn hearing aids. No beauty retouching or skin smoothing. Output each as 4:5 portrait at 1200 × 1500.

### Recommended option
**Option 3**, once both portraits are in hand. The two profile cards sit side by side and are read as a pair, so matching them is the most visible improvement. If only this portrait is available, use Option 1.

### Real-image note
**REAL PROVIDER IMAGE PREFERRED, AI-GENERATED PORTRAIT NOT ACCEPTABLE.** Generating a portrait of a named, credentialed provider would be a fabricated image of a real person and violates DESIGN_SYSTEM.md. Use the clinic's own portrait, confirm reuse rights, and describe it accurately in the alt text with his real title (Hearing Aid Specialist), never "Dr." or "audiologist".

---

## IMG-PROVIDER-02 - S06 Team: Toni Trager portrait

### Placeholder purpose
Give the visitor a face for the specialist who also makes the home and care-facility visits, and whose lived experience with hearing aids informs her care. The portrait must feel as approachable as it is professional.

### Recommended source type
Real provider image preferred. The site has a white-coat portrait (`staff-AE8A1494.webp`). Needs inspection and rights confirmation.

### Recommended composition
- **As built:** 4:5 portrait, matching Jaysee's card in size and crop.
- Head and shoulders, eyes in the upper third, a little headroom. The same background value and framing as IMG-PROVIDER-01 so the pair reads as one set.
- **If she is wearing hearing aids in the photo, leave them exactly as they are.** Do not remove, hide or retouch them. They are part of her real story as the site tells it.

### Option 1 - Background normalization
Image-edit prompt using the real portrait of Toni Trager as the reference input. Replace only the background with a soft, out-of-focus warm neutral tone (light sage-cream) with a subtle gradient and natural depth falloff around her hair and white coat. Do not change her face, hair, ears, any worn hearing aids, expression, coat or lighting on the subject. No smoothing or reshaping. Output 4:5 portrait, at least 1200 × 1500.

### Option 2 - Recompose to 4:5
Image-edit prompt using the real portrait as the reference input. Extend the canvas as needed to create a 4:5 head-and-shoulders frame with comfortable headroom, continuing the existing background naturally. Keep her face, hair, ears, any hearing aids, white coat and expression exactly as shot. Do not add objects, text or logos. Maintain the original lighting direction. Output 4:5 portrait at 1200 × 1500.

### Option 3 - Matched-pair harmonization
Image-edit prompt using the real portraits of Toni Trager and Jaysee A. Soto as reference inputs. Match exposure, white balance, contrast and background tone across both so they read as one portrait set. Preserve every real detail of each person, including any worn hearing aids, hair, expression and uniform. No beauty retouching, no skin smoothing. Output each as 4:5 portrait at 1200 × 1500.

### Recommended option
**Option 3**, applied together with IMG-PROVIDER-01. If Toni's portrait is the only one that needs work, use Option 1.

### Real-image note
**REAL PROVIDER IMAGE PREFERRED, AI-GENERATED PORTRAIT NOT ACCEPTABLE.** The same reasoning applies as for Jaysee. Her story about wearing hearing aids since childhood is a real, personal detail, and a generated stand-in could misrepresent it. Alt text uses her real title (Hearing Aid Specialist).

---

## Step 5 maintenance notes

- If the hero becomes a full-width or 16:9 layout, rework the IMG-HERO-01 composition, since the current notes assume the 5:6 / 4:3 / 3:2 crops.
- If the S04 or S05 photo moves or gets a different crop, update the aspect-ratio lines in IMG-CLINIC-01 and IMG-CLINIC-02.
- If Google Business Profile or exterior photos are supplied, add a new entry for any location image. No AI exterior or entrance should ever be generated.
- If a new image slot is added to any section, give it an ID and add a three-option entry here before the section is approved.
