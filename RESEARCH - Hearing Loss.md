# RESEARCH.md — Altamonte Family Hearing (Topic: Hearing Loss)

**Stage:** Step 2 — research and factual extraction only. No design, no HTML/CSS, no final copy.
**Research date:** Monday, October 12, 2026
**Revision:** Google Reviews screenshots (captured Oct 12, 2026) added as verbatim text in §3A. Flags 2 and 3 updated, Flags 1, 5 and 12 extended.
**Primary source:** https://altamontefamilyhearing.com/ (pages fetched are logged at the bottom)
**Secondary sources:** third-party directory/review listings, used only for cross-checks and labelled as such.

> **How to read this file.** Facts are paraphrased from the clinic's pages, not copied. When final copy is written, pull exact wording from the live page named in each source note. Review text is the one exception: §3A reproduces the supplied Google Reviews screenshots exactly as written (typos included), because the brief says reviews must not be rewritten. The §3 theme map still covers reviews from the clinic's `/reviews` page that have no screenshot yet.

---

## 0. PRIORITY FLAGS (read first)

These are conflicts or gaps between PROJECT_BRIEF.md and the sources that affect strategy decisions.

| # | Flag | Detail |
|---|------|--------|
| 1 | **Phone number mismatch** | The brief specifies **407-809-8154**. Every page on the clinic's site, plus Healthgrades, Nextdoor and the Seminole Chamber listing, shows **407-949-6737**. The brief's number appears in no source I checked. It is probably a campaign/tracking number, but this needs confirmation. The clinic's WhatsApp link points to the 949-6737 number. **Update (Oct 12 screenshots):** the Google search results for the clinic also show **407-949-6737** ("Call 407-949-6737"). The brief's number is still unverified. |
| 2 | **Review count mismatch — RESOLVED** | The homepage says **157** five-star Google reviews. The site's `/reviews` page and `/llm-info` page (last updated Oct 6, 2026) say **5.0 stars across 155 reviews**. **Resolution:** the Google listing screenshots (captured Oct 12, 2026) show **5.0 stars and 157 reviews**. Use **157**. The 155 figure on `/reviews` and `/llm-info` is out of date. The count will keep moving, so the page should be re-checked before launch. |
| 3 | **Reviews partly supplied; GBP photos still missing** | Six Google Reviews screenshots were supplied. They give full text for **10 reviews** (§3A). Two more reviews (Jason Hoch, Teri Yanovitch) are cut off in the screenshots and have no readable text. **Google Business Profile photos have still not been supplied.** |
| 4 | **Brand fonts and colors are unconfirmed** | The brief's brand fields are AUTO-DETECT. A text-only fetch cannot read CSS or the logo pixels. The only confirmed brand value is a site-wide `theme-color` of **#1A3028** (dark forest green). Details are in §8. |
| 5 | **Provider title wording** | The site uses **Hearing Aid Specialist (HAS)** and **Board Certified in Hearing Instrument Sciences (BC-HIS)**. It never says "audiologist" or "Dr." for Jaysee or Toni. Some third-party listings and some patient reviews call Jaysee an audiologist. Page copy should not follow that, though reviews must stay unaltered. **Update (Oct 12 screenshots):** three of the 10 transcribed reviews call him "Dr." or "the good doctor" (Rocio M Stevens, Lena Espana, Larry Williams Music). The clinic's own public reply to Lena Espana's review carries a legal disclaimer saying Jaysee A. Soto is a *Board Certified Hearing Instrument Specialist, not a medical doctor*. Page copy should never use "Dr." for him. The other 7 transcribed reviews do not use a doctor title, so prefer those where possible, and confirm with the client before showing any "Dr." review unaltered. |
| 6 | **"Free hearing test" claim is qualified on the site** | The homepage CTA calls the evaluation "complimentary". The hearing-tests page says *most* evaluations are complimentary and tells people to call to confirm any costs. Avoid an unqualified "free" claim. |
| 7 | **Age range** | Current site copy says evaluations are for **adults** (adults of all ages). An older third-party snippet says "individuals of all ages". Pediatric care is not supported by the current site. |
| 8 | **Minor copy variants across pages** | `/services/hearing-aid-repair` and `/hearingup-jaysee-soto` show an older nav/footer variant ("Walk-in hour 1 to 2 pm, every day we're open", "Book my complimentary hearing evaluation"). Other pages say "Walk-in cleanings and minor repairs". The facts are the same, and the repair page text looks like a slightly older template. |
| 9 | **`{{location.name}}` in footer copyright** | The brief gives "© current year {{location.name}}". The value is not specified. The site footer uses "Altamonte Family Hearing". |
| 10 | **Booking embed** | The supplied iframe is identical to the one on the clinic's own `/schedule` page. The embed URL has no width, height or title attributes. The brief says not to modify it unless technically necessary. |
| 11 | **Google Reviews link** | The brief's link is a long Google *search* URL with session/tracking parameters. The clinic's own site links to a Google Maps place URL (`...!1s0x88e771506ecb647d:0xabcbd17d7a2f5be5...!9m1!1b1`). The place ID in the brief's map link matches the same listing. The screenshots show this listing as "Altamonte Family Hearing" at "715 Douglas Ave #45" (the brief's CTA text and the site say "Suite 45"). |
| 12 | **Conflicting claims in third-party snippets** | The screenshots show a Facebook search snippet saying "over 25 years of experience". This conflicts with the clinic's own site, where Jaysee has been in hearing care since 2013, and no founding year is stated. Do not use the 25-year claim. The Google result for Yelp also categorises the clinic as "Audiologist", which the clinic's site does not claim (see Flag 5). The owner's review reply uses the wording "Board Certified Hearing Instrument Specialist", while the site says "Board Certified in Hearing Instrument Sciences (BC-HIS)". Use the site's wording for credentials. |

---

## 1. COMPANY SUMMARY

**What the company is.** Altamonte Family Hearing is a family-owned, independently operated hearing care practice in Altamonte Springs, Florida. It states it is not part of a chain. The practice was opened by **Jaysee A. Soto, HAS, BC-HIS** (owner) and his wife **Grace Soto** (co-owner and Patient Care Coordinator). They live in the community where the office is located. *(Sources: /about, /hearingup-jaysee-soto, /llm-info)*

**Who it serves.**
- Adults with hearing concerns.
- People who already wear hearing aids, including those bought elsewhere.
- Family members and caregivers. Many reviews describe adult children bringing parents, and the site explicitly describes family-arranged home visits.
- Spanish-speaking patients. Evaluations, patient forms and a Spanish page (`/es`) are offered.
- Greater Orlando area residents, with a stated list of nearby communities (§4).

**Primary services (7 listed on the site).**
1. Hearing tests (comprehensive in-office evaluation)
2. Hearing aid fittings
3. Real Ear Measurement (REM)
4. Hearing aid repair and cleaning (all major brands)
5. Earwax removal (video otoscopy plus warm-water irrigation)
6. Tinnitus consultations
7. Mobile hearing services (home or care facility)

**Hearing aid brands fitted (6).** Phonak, Oticon, ReSound, Signia, Starkey, Widex. The site says the practice is not tied to one manufacturer. *(Source: /about FAQ)*

**Relevant specialties and differentiators stated by the site.**
- Verification-based fittings: Electroacoustic Analysis (EAA) plus Real Ear Measurement.
- Jaysee is a **HearingUp Certified Provider**.
- Five years of professional care included with hearing aids bought from the office.
- A stated 100% satisfaction guarantee on hearing aids from the office (terms not stated; see §10).
- Walk-in hour for cleanings and minor repairs.
- Care in English and Spanish.

**Locations.** One office: **715 Douglas Ave, Suite 45, Altamonte Springs, FL 32714**, inside **One Senior Place**. It also offers home and care-facility visits across the greater Orlando area.

**Status.** The homepage says the practice is "now accepting new patients".

---

## 2. SERVICE / TOPIC RESEARCH — HEARING LOSS

### 2.1 How the site frames the service
The service is a **comprehensive hearing evaluation**, followed by a recommendation and, only if appropriate, hearing aids with verified programming and ongoing follow-up. The site's dedicated `/hearing-loss` page is a patient-education page covering signs, types and next steps. Its homepage H1 is "Hearing Care That Feels Like Family".

### 2.2 Symptoms and signs mentioned (consolidated)
From `/hearing-loss`, `/services/hearing-tests`, `/hearing-aids`, and `/services/tinnitus`:
- Often asking people to repeat themselves.
- Hearing that someone is talking but not always catching the words.
- Difficulty following conversation in restaurants, at parties or gatherings, or in the car.
- Others saying the TV or phone is too loud.
- People seeming to mumble.
- Ringing, buzzing, humming or other sounds along with a change in hearing.
- Phone calls feeling harder.
- Feeling tired after conversations in noisy places.
- It has been a long time since the last hearing test, or the person has never had one.

### 2.3 Types of hearing loss (from `/hearing-loss`)
| Type | What happens | Common causes (per site) | Treatability (per site) |
|---|---|---|---|
| **Sensorineural** | Damage to the inner ear (hair cells) or hearing nerve | Age, family history, loud noise over time, some medications, illness, head injury | Usually permanent. Hearing aids may help. Sudden loss needs immediate medical assessment. |
| **Conductive** | Sound doesn't pass efficiently through the outer or middle ear | Earwax, middle-ear fluid, ear infections, perforated eardrum | Often treatable. May involve medical care, earwax removal or surgery. |
| **Mixed** | Both types together | A mix of the above | Conductive part may be treatable. Hearing aids or other care may help the remainder. |

The site says a hearing evaluation helps identify the type and degree of loss, and that some findings need medical assessment.

### 2.4 Related conditions the site addresses
- **Tinnitus.** The site defines it as perceiving sound without an external source. It often occurs with hearing loss. There is no universal cure. Some cases improve when an underlying cause is treated, and hearing aids (including models with built-in sound therapy) may make it less noticeable. The site notes it can feel louder in quiet settings.
- **Earwax blockage.** It is a common reason for muffled hearing, fullness, hearing-aid whistling and discomfort. Cotton swabs can push wax deeper.
- **Sudden hearing change.** The site treats this as a medical emergency (see §2.9).

### 2.5 Benefits mentioned
- Easier to follow conversations, enjoy TV and stay connected on the phone ("for many people with hearing loss").
- Speech can be easier to follow in noise with the right features. The site says no hearing aid removes background noise completely.
- Tinnitus may become less noticeable when hearing loss is also present. The amount of relief varies.
- A hearing evaluation gives a **baseline record** to compare against at future visits. It is useful even if hearing is normal.
- Verified fitting: the sound is measured in the patient's own ear rather than relying on software defaults.
- Five years of professional care, with follow-up adjustments.
- Same-day results explanation after the hearing test (per page meta description).

### 2.6 Service / treatment process

**A. Hearing evaluation (4 steps, `/services/hearing-tests`)**
1. **Consultation:** hearing history, overall health, and where hearing is hardest.
2. **Ear exam:** otoscope check of canals and eardrums for earwax or anything to address before testing.
3. **Hearing test:** in the sound booth, through headphones. It includes tones at different pitches and words in quiet and in background noise.
4. **Results:** the audiogram (a chart of hearing across pitches) is reviewed and explained. If hearing is within normal limits, the clinic says so.

The site says the test measures the softest sounds heard at different pitches in each ear, and also speech understanding in quiet and in noise.

**B. What happens next (`/hearing-loss`, 3 steps).** Book a hearing evaluation, then results explained (family or friend welcome), then talk through options. Depending on results, the next step may be earwax care, a medical referral, or hearing aids. If hearing aids are appropriate, the clinic compares options against hearing, daily life, preferences and budget.

**C. Hearing aid fitting (4 steps, `/services/hearing-aid-fittings`)**
1. **Recommendation:** review the audiogram, routine, preferences and budget.
2. **Physical fit:** comfort adjustments. Electroacoustic Analysis checks performance against manufacturer specifications before fitting.
3. **Programming:** targets calculated from the hearing test. Real Ear Measurement verifies the sound delivered in the ear.
4. **Follow-up:** visits over the first few weeks to fine-tune. The site says the brain needs time to adjust to sounds it hasn't heard clearly.

Also stated: coaching on inserting and removing the aids, daily care, and help with phone pairing and app features when devices are compatible.

**D. Real Ear Measurement (4 steps, `/services/real-ear-measurement`).** The steps are ear exam, probe-tube placement, measurement, and fine-tuning. A calibrated speech signal is played at soft, average and loud levels. Output near the eardrum is compared with prescriptive targets calculated from the hearing test "using a validated fitting formula" (formula not named). The measurement is repeated after adjustments, and loudness comfort is assessed. The site explains that ear canal size and shape and the dome or earmold fit change how much sound arrives, so two people with the same audiogram and settings can get different levels. REM can also be used to check hearing aids bought elsewhere.

**E. Earwax removal (4 steps, `/services/earwax-removal`).** The steps are a health screening questionnaire, a video otoscope exam (patient can see the screen), irrigation with the Earigator (body-temperature water at controlled low pressure), and a follow-up video check with home-care advice.

**F. Tinnitus consultation (`/services/tinnitus`).** It covers consultation, ear exam, hearing test, and options. Medical referral is made if symptoms point to a medical cause, and referral to another provider is made if more specialized tinnitus care is needed.

**G. Mobile visits (`/services/mobile-hearing-services`).** Toni brings portable testing equipment, a video otoscope and fitting supplies to a home or care facility. The visit is set up in the quietest available room. Some tests need the sound booth, and the site says it will explain when that applies.

### 2.7 Technologies, techniques and tools mentioned
- Sound booth; audiogram; speech-in-quiet and speech-in-noise testing.
- Otoscope and video otoscope.
- Electroacoustic Analysis (EAA) in a test box.
- Real Ear Measurement with a probe tube.
- Earigator irrigation system.
- Professional dehumidifier (for moisture-affected hearing aids).
- Portable testing equipment (home visits).
- On-site interactive items: a speech-in-noise "with/without hearing aids" sound demo (labelled as a simulation, with individual results varying) and a four-question hearing-aid style quiz.
- **Hearing aid styles carried (6):** RIC, BTE, ITE, ITC, CIC, IIC.
- **Models named as "current models we fit" (`/hearing-aids`):**
  - Phonak: EON, Audéo Sphere Infinio, Audéo Infinio, Virto
  - Oticon: Reveal, Zeal, Intent
  - ReSound: Sensia, Vivia
  - Signia: MaX, Pure Charge&Go IX
  - Starkey: Omega AI, Edge AI
  - Widex: Allure, Moment, SmartRIC
- **Features described:** rechargeable, Bluetooth and hands-free calls, streaming, noise/AI processing, Auracast, built-in tinnitus features. The site says features vary by model, technology level and device compatibility.

### 2.8 Provider qualifications relevant to the service
**Jaysee A. Soto, HAS, BC-HIS** *(/about/jaysee-soto, /hearingup-jaysee-soto)*
- Owner and Hearing Aid Specialist. In hearing care since **2013**.
- Florida-licensed Hearing Aid Specialist.
- **Board Certified in Hearing Instrument Sciences (BC-HIS).**
- **HearingUp Certified Provider.**
- **Florida Hearing Society Board, District 5 Director.**
- English and Spanish.
- Creates hearing care videos as "The Bald Hearing Guy" (YouTube, Instagram, TikTok).
- Altamonte Springs local.

**Toni Trager, HAS** *(/about/toni-trager)*
- Florida-licensed Hearing Aid Specialist. English.
- Has worn hearing aids since childhood (the site says she was born with hearing loss). The site presents this as informing her patient care.
- B.S. in Health Sciences (pre-clinical, minor in Health Services Administration), University of Central Florida. Previously worked in hospitality.
- Provides the mobile/home visits.

**Patient Care Coordinators:** Grace Soto (co-owner) and Francesca Natal, both bilingual (English/Spanish). They help with scheduling, insurance questions, patient forms and follow-up.

The site counts "2 Florida-licensed Hearing Aid Specialists" on staff. No audiologist or physician is listed. Referral to an ENT physician or other provider is described when medical care is needed.

### 2.9 Suitability, caveats, disclaimers
**Who may be a good fit (as stated by the site):**
- Adults noticing the signs in §2.2, or who have never had a hearing test.
- People with hearing loss and bothersome tinnitus. The site says clinical guidelines (not named) recommend a hearing aid evaluation for this group.
- People with hearing aids that "never sounded right", are several years old, or were fitted elsewhere and want a second opinion or verification.
- People who find getting to the office difficult (home or care-facility visits).
- Hearing aid wearers needing cleaning or minor repairs, including those who bought elsewhere.

**Important caveats and disclaimers on the site:**
- A **sudden drop in hearing is a medical emergency.** Seek medical care immediately rather than waiting for a routine evaluation. Tinnitus with sudden severe spinning also needs immediate care. Tinnitus that starts suddenly, is in one ear, or pulses with the heartbeat needs prompt physician care.
- Not everyone needs hearing aids, and the clinic says it will tell patients if they don't.
- Some findings need medical assessment or referral.
- Sensorineural loss is usually permanent.
- The sound demo is a simulation, not a hearing test or prediction. Individual results vary.
- Hearing aid features and water protection vary by model. Follow manufacturer guidance on moisture.
- No hearing aid removes background noise completely.
- Earwax irrigation is not suitable for everyone, for example with prior ear surgery, ear tubes, a perforated eardrum or recent infection. There is a screening questionnaire, and referral is made if wax cannot be cleared safely.
- Earwax removal and home-visit costs are "call for details". Mobile service availability and cost need a call.
- Insurance coverage varies by plan. Some plans help with part of hearing aid cost.
- OTC hearing aids and AirPods Pro hearing features are for adults 18+ with perceived mild-to-moderate loss. The site notes that hearing aids from the office include professional fitting and ongoing care.
- Some repairs need manufacturer service (water inside the case, cracked shell, failed circuit board). Manufacturer warranty may cover them.

### 2.10 Useful patient education points
- Hearing changes are often gradual and easy to miss, and a baseline test helps track change.
- Protect hearing: reduce exposure to loud sound, keep headphone volume down, use hearing protection when needed.
- Avoid cotton swabs in the ear canal; ear candling is not safe.
- Bring a family member or friend to results reviews: "a second set of ears".
- Hearing aids typically last about 3–7 years. Professional deep cleaning every six months is recommended. Wipe aids nightly (never with alcohol) and keep them out of the bathroom. Florida humidity increases moisture-related repairs.
- Health history and medications can be relevant to hearing changes. The site asks patients to bring a medication list.
- Own voice may sound different at first. Adjustment time varies.
- Ask your provider: Will you measure the sound in my ear? Compare it with my prescription? Test the hearing aid itself? How are follow-ups handled? What care is included and for how long? Is there a satisfaction guarantee? What happens if it needs repair? *(This list is on `/hearing-aids` and `/about/best-practices`.)*

### 2.11 Especially persuasive, decision-relevant facts
1. Fittings are **verified in the patient's own ear** (REM), plus device testing (EAA).
2. **Five years of professional care** on hearing aids from the office, at every technology level.
3. **100% satisfaction guarantee** stated on the homepage (terms not provided).
4. **Independent, family-owned**; two licensed specialists; consistent small team.
5. **Six manufacturers**, not tied to one. Recommendations are based on results, lifestyle, budget and preferences.
6. The clinic states it will **tell patients when they don't need hearing aids.**
7. Evaluation is **complimentary in most cases** (confirm cost by phone).
8. **Results explained same day**, and the patient is welcome to take the information home and decide.
9. **Walk-in hour** weekdays 1–2 pm for cleanings and minor repairs. Most small repairs are done in-office, often while you wait.
10. **Spanish-language** evaluations and forms.
11. **Home and care-facility visits.**
12. Insurance benefits checked for patients ("we accept many insurance plans").
13. Jaysee is a HearingUp Certified Provider: a network of providers committed to best practices, including Real Ear Measurement, founded by Dr. Cliff Olson (reviewed personally per the site).

---

## 3. TRUST SIGNALS

| # | Signal | Detail | Source | Verification note |
|---|--------|--------|--------|-------------------|
| 1 | Google rating | **5.0** stars | Google listing screenshots (Oct 12, 2026), /reviews, /llm-info | **Confirmed** on the live Google listing. |
| 2 | Google review count | **157** | Google listing screenshots (Oct 12, 2026), homepage | **Confirmed.** `/reviews` and `/llm-info` show an older figure of 155. See Flag 2. |
| 3 | Years in hearing care | Jaysee has been in hearing care since **2013** | /about/jaysee-soto, /hearingup-jaysee-soto | Site statement. The page also says "more than a decade". |
| 4 | Practice founding date | **Not stated.** | n/a | The earliest dated Google reviews on the site's reviews page run back to at least early 2020 (the fetched page was truncated, so earlier ones may exist). Do not state a founding year. |
| 5 | Florida licensure | Jaysee and Toni are Florida-licensed Hearing Aid Specialists | /about, homepage | Site statement. State license numbers are not given. |
| 6 | National board certification | Jaysee: Board Certified in Hearing Instrument Sciences (BC-HIS) | /about/jaysee-soto | Site statement. |
| 7 | HearingUp Certified Provider | Jaysee. Network founded by Dr. Cliff Olson; best practices incl. REM | /hearingup-jaysee-soto | Site statement. A HearingUp logo asset exists on the site (§9). |
| 8 | Professional association | Florida Hearing Society Board, District 5 Director (Jaysee) | /about, /about/jaysee-soto | Site statement. |
| 9 | Chamber membership | Seminole County Chamber of Commerce member | /about, /llm-info | Site statement. |
| 10 | Building affiliation | "Certified hearing care provider of One Senior Place" (the building that houses the office) | /about, /llm-info | Site statement. |
| 11 | Team size / licensure | 2 licensed Hearing Aid Specialists plus 2 Patient Care Coordinators | Homepage, /about | Site statement. |
| 12 | Satisfaction guarantee | "100% satisfaction guaranteed on hearing aids from our office" | Homepage stat strip | Explicit on the homepage only. **Terms (trial length, refund conditions) are not stated anywhere I found.** |
| 13 | Included care | Five years of professional care with hearing aids from the office, at every technology level | Homepage, /about, /hearing-aids, /llm-info | Consistent across pages. The detailed scope of "professional care" is not itemised. |
| 14 | Verification methods | EAA plus Real Ear Measurement | Homepage, /about/best-practices | Site statement. |
| 15 | Independence | "Not part of a chain": independent, family-owned | /about FAQ | Site statement. |
| 16 | Technologies | Sound booth, video otoscope, REM system, Earigator, EAA test box | Service pages | Site statements. Specific equipment brands/models are not named. |
| 17 | Number of locations | **1** office. Mobile visits are extra. | /llm-info | Site statement. |
| 18 | Languages | English and Spanish (Jaysee, Grace, Francesca bilingual) | /llm-info, /about | Site statement. |
| 19 | Community education | "We also share hearing health education throughout our community" | /about | **No specific events named.** |
| 20 | Media / content presence | YouTube "The Bald Hearing Guy" (Jaysee). Instagram/TikTok under the same handle. Facebook page. Podcast "Wax and Whiskey" (Apple Podcasts, Spotify). | /llm-info, footer | Links confirmed on the site. **Subscriber/download counts not verified.** |
| 21 | Awards / recognition | **None found.** | n/a | Do not claim any. |
| 22 | Third-party ratings | Yelp: 5.0 (3 reviews) as of a Dec 2025 snippet. Healthgrades, HearingTracker, Healthy Hearing and Nextdoor all have profiles. | Third-party search results | Third-party counts not independently verified. They are small compared with Google. |
| 23 | Third-party education claim | Healthgrades structured data lists "Miami Dade College" for Jaysee | Healthgrades | **Third-party only. Not on the clinic's site. Do not use without confirmation.** |

### Review inventory (themes only; verbatim text lives on https://altamontefamilyhearing.com/reviews and in the supplied screenshots)
Reviews on the site's `/reviews` page, which pulls from Google, group into these themes. This list is a theme map and is not a pull-quote list.

| Theme | Reviewers (date) |
|---|---|
| **Thoroughness of the hearing test / "most thorough ever"** | Daniel Jordan (Sep 2026), Pete Zeitler (Feb 2026), Anthony Valada (Feb 2026), Gartrelle Wilson (Aug 2025), Gladys Matos (May 2026), Barbara Morey (Jun 2025), Telva Thomas (Jan 2021) |
| **REM / verified fitting named by the patient** | Ron Phinney (Feb 2025: Real Ear Measurement with new Phonak aids) |
| **Honest advice, including not upselling or not needing aids** | Zunilda Grullo (Sep 2024: told she did not need aids and was referred back to her ENT), Joanne Godwin (Apr 2023: told she did not need top-of-line), Teri Yanovitch (May 2025: not just focused on selling) |
| **First-time wearers / nervous patients** | Sue Christensen (Sep 2026), Deborah Bradley (Dec 2024), Randall Ellington (Nov 2024), Ashley Harris (Jul 2026, claustrophobic, test with Toni), Priscilla Lopez (Jul 2020, anxious) |
| **Adult children bringing parents** | Cynthia O'Brien (Dec 2025, 92-year-old mother, 5 years), Evelyn Ramirez (Mar 2025, 88-year-old mother-in-law), Philip Zeitler (Feb 2026, father), Lyn Bergen (Feb 2024) |
| **Insurance / cost / budget help** | Jan Bradburn (Jun 2026), Harmonie J (Nov 2023), Ginger H (Jul 2023), Shannon Bonardy (Nov 2024), Evelyn Ramirez (Mar 2025), Christopher Powell (Dec 2025; he reports his own aids were covered by his Medicare. This is a patient statement, not a clinic claim.) |
| **Same-day repairs / walk-in / urgent help** | Emily Palo (May 2026, walk-in hours), Jason Hoch (May 2026, out-of-state visitor repaired same day), Tom Pitcock (Dec 2025), Justin Yang (Jan 2024), Kate Morgan (Oct 2024) |
| **Spanish-language care** | Noemí Cardona Delgado (Nov 2021), Zunilda Grullo (Sep 2024), Angela Del Pozo (Feb 2020, Spanish) |
| **Team warmth / "feels like family"** | Mary Schultz (May 2025), Mike Collins (Feb 2024), Mindi Clifton (Nov 2023) |
| **Patient education / learning to use aids** | Ron Brown (Apr 2025), Alice Rossum (Dec 2024, aids from the VA), Philip Zeitler (Feb 2026, phone pairing) |
| **Tinnitus / ringing** | ben (indicuts) (Dec 2024, ringing and high-frequency loss), Alexis (Jun 2025, long-term patient with Ménière's-related loss) |
| **Long-term loyalty** | Gary Teramae (Sep 2026, ~4 years), Mary Schultz (~4 years, 2nd set), Thomas Colwell (Mar 2024, 4th year) |
| **Brief / short punchy five-stars (usable for a compact card)** | Janet Kerkhoff (Sep 2026), Hector Sosa (Sep 2026), Richard Nottingham (Sep 2026), Pamela Levin (Jul 2026) |

*Reviewer-specific cautions:* some reviews reference competitor pricing or third-party providers (for example big-box stores or ENT offices). The Ménière's, Medicare, VA and ENT-referral mentions are patient statements about their own situations and should not be rephrased into clinic claims. Several reviews call Jaysee an "audiologist" (see Flag 5).

### 3A. Verbatim Google reviews (from supplied screenshots)

**Source:** six screenshots of the Google listing for Altamonte Family Hearing (715 Douglas Ave #45, Altamonte Springs, FL 32714), captured Monday, October 12, 2026.
**Listing header shown:** **5.0** stars, **157 reviews**.
**Transcription rules:** text is copied exactly as it appears, including typos, spacing and punctuation quirks. Google shows relative dates ("3 months ago"), not exact dates. Where a review is cut off in the screenshot, it is marked and not completed. Reviewer details are as shown by Google.

All 12 reviews visible are **5 stars**. Ten have full text and two are cut off.

#### Full text available (10)

**1. Rocio M Stevens** — 10 reviews · 5 stars · 3 months ago · no owner reply visible
> Dr.Soto provided exceptional care for my mother's hearing needs. From the moment we arrived, he and his team were professional, patient, and compassionate. They took the time to explain every step of the process, making sure my mother fully understood her options and felt comfortable throughout the entire experience.
> The service was outstanding, and my mother is absolutely thrilled with her new hearing aids. The improvement has made a tremendous difference in her daily life.
> I highly recommend Dr. Soto, especially to the Spanish-speaking community. Being able to communicate in Spanish made my mother feel at ease and well cared for. Dr. De Soto is truly amazing, and we are very grateful for his expertise and kindness.
> Thank you

*Themes:* adult child with parent; Spanish-language care; clear explanations. *Caution:* uses "Dr. Soto" and "Dr. De Soto" (Flag 5).

**2. jan bradburn** — 2 reviews · 5 stars · 3 months ago · 1 heart reaction
> Jaysee Soto gave me back my hearing! I have several hearing aids that don' t work and don't fit, but Jaysee found the perfect match for me. To determine my hearing concerns, I had a extensive exam that went far beyond my other hearing exams, leading to hearing aids that are comfortable and actually work. The office staff is professional and accomodating. They worked with my insurance to get me the best price on my hearing aids.
> I highly recommend Altamonte Family Hearing.

*Owner reply (2 months ago):* Love to see when our patients notice our efforts. Thank you for supporting in our family business ♥

*Themes:* thorough exam; hearing aids that previously did not fit; insurance and price help. *Caution:* the insurance and price comment is the patient's own experience, not a clinic claim. Typos in the original: "don' t", "a extensive", "accomodating".

**3. Anthony Valada** — 9 reviews · 5 stars · 8 months ago · no owner reply visible
> Jaysee Soto is a total professional that only wants to do the best. The exam was complete in every way. It wasn't 15 minutes and here's your hearing aids. The hearing aids were set up to fit my needs . The staff in the office was also great. I would recommend Jaycee and the staff at Altamonte Family Hearing to anyone needing hearing help !

*Themes:* thorough exam; hearing aids set up to fit needs; staff. *Note:* the reviewer spells the name "Jaysee" first and "Jaycee" second. Keep as written.

**4. Philip Zeitler** — Local Guide · 13 reviews · 73 photos · 5 stars · 8 months ago · no owner reply visible
> We had an excellent experience with Altamonte Family Hearing, and I can't thank them enough for the care they provided my dad. Jaysee Soto was absolutely wonderful throughout the entire process. He spent a great deal of time performing very thorough hearing tests and, just as importantly, took the time to clearly explain the results in a way that we could all understand.
>
> When it came time to set up and program my dad's new high-end ReSound hearing aids, Jaysee was incredibly patient and detail-oriented, making sure everything was perfectly tuned to my dad's needs. He also went above and beyond by showing my dad how to operate the hearing aids through his phone once they were paired, which gave him a lot of confidence using them.
>
> The level of professionalism, knowledge, and genuine care we experienced by everyone in the office made a huge difference. I highly recommend Altamonte Family Hearing and Jaysee Soto to anyone looking for top-quality hearing care and outstanding service.

*Themes:* adult child with parent; thorough tests and clear results; programming; phone pairing coaching. *Note:* long. A shorter review is better for a compact card.

**5. Emily Palo** — Local Guide · 23 reviews · 10 photos · 5 stars · 5 months ago · 1 heart reaction
> I want to start this review by saying this has by far been the best experience I have had with healthcare. About a month ago, I came across them by googling places that can repair hearing aids. I called them 5 minutes before closing time and they happily answered my call for help and immediately re-assured me that they can help. I came in today during the walk-in hours and showed them the aids and the issue. I was greeted by Jaysee and he re-assured me that things can be fixed, and all the same day! The staff are very friendly and helpful. I had mentioned that getting hearing aids has been hard and they immediately wanted to help with a solution. I really felt heard and cared for by the staff! Thank you so much! Your help has made a HUGE impact on my life. This is absolutely the place to go!!!!

*Owner reply (5 months ago):* Wow Emily, thank you for taking the time to share your experience. Its so satisfying to know we made an impact in your hearing journey ♥

*Themes:* walk-in hours; same-day repair; feeling heard. *Note:* this is a repair visit, not a hearing-loss evaluation.

**6. Steve Marsee** — Local Guide · 28 reviews · 6 photos · 5 stars · 3 months ago · 1 heart reaction
> They have the in the ear measuring capability that allows them to actually see in the device they have in your ear is actually picking up the sounds that you need. That ensured that my monitors were dong their job based upon my specific needs. Jaysee and his staff are personable, professional and really go the extra mile for their clients. You can see their empathy, understanding and dedication to every one of us. You really matter to them and they have invested the training and resources for state-of-the art equipment necessary to provide you with the absolute best care available.

*Themes:* in-ear measurement (matches the clinic's Real Ear Measurement); empathy; equipment investment. *Caution:* the reviewer says "monitors", which appears to mean his own in-ear monitors rather than hearing aids. The meaning is unclear out of context, so treat as a candidate with care. Typos in the original: "have the in the ear", "dong", "state-of-the art". *Check this transcription against the live review before use:* the sentence beginning "You really matter to them" was read from a small screenshot.

**7. Christopher Powell** — 6 reviews · 5 stars · 9 months ago · no heart reaction visible
> I've never before had such an easy, completely enjoyable experience during a healthcare visit as that which is provided by the excellent staff at Altamonte Family Hearing.
> The friendly and inviting treatment is fully backed up a very high level of expertise and personal care.
> The comprehensive and meticulous hearing exam has resulted in a significant improvement in my daily life. And, the best part, the expenses for my new hearing aids were completely covered by my Medicare.

*Owner reply (9 months ago):* Mr. Powell, We're thrilled to know about your improvement. Welcome back to hearing!

*Themes:* comprehensive exam; improvement in daily life; Medicare coverage. *Caution:* the Medicare statement is this patient's own experience. It must not be presented as a clinic claim, and it may raise compliance questions for a healthcare page. Flag for client review. Typo in the original: "fully backed up a very high level".

**8. Pete Zeitler** — 5 reviews · 5 stars · 8 months ago · no owner reply visible
> I received a complete hearing audit on Friday 1/30/26. I found the process to be extremely thorough and I have had 5 audits in the past 4 years this was by far my best experience. The business and everyone there were exceptionally professional. Great detail went into the programming of my new ReSound hearing aids. I would highly recommend Altamonte Family Hearing as a trustworthy and honest provider for hearing aids.

*Themes:* thorough evaluation; programming detail; trust and honesty.

**9. Lena Espana** — 4 reviews · 5 stars · a year ago
> Altamonte family hearing has excellent customer service and Dr. Soto was so attentive and professional. He takes the time to listen to you and hear your needs. He explains things thoroughly and makes you feel comfortable.

*Owner reply (a year ago):* It's important to me that my patients understand all they need to know about their hearing health and not feel rushed. Thank you for noticing my efforts to make that happen ♥
**Legal Disclaimer: Jaysee A. Soto is a Board Certified Hearing Instrument Specialist, not a medical doctor**

*Themes:* listening; clear explanations; unhurried visits. *Caution:* uses "Dr. Soto". The owner's own reply says he is not a medical doctor (Flag 5).

**10. Larry Williams Music** — 6 reviews · 5 stars · a year ago
> My visits to Dr. Jaysee at Altamonte Family Hearing have always been informative, courteous, and friendly. Francesca is always prompt and consistent with all the protocols leading up to each appointment and she (and the good doctor) always recognizes me on sight. A perfect model for any very doctor's office!

*Owner reply (a year ago), cut off in the screenshot:* Thank you so much for your kind words! It means a great deal to me and to Francesca that you've had ...

*Themes:* returning patient; front-desk consistency. *Caution:* uses "Dr. Jaysee" and "the good doctor" (Flag 5). Typo in the original: "any very doctor's office".

#### Visible but text cut off (2)
These reviews appear in the screenshots without readable text. Another screenshot is needed.

| Reviewer | Details shown | Status |
|---|---|---|
| **Jason Hoch** | 1 review · 5 stars · 5 months ago | Text not visible |
| **Teri Yanovitch** | Local Guide · 15 reviews · 5 stars · a year ago | Text not visible |

#### Coverage of the 10 transcribed reviews
| Use on the page | Reviews |
|---|---|
| Thorough evaluation / exam | Anthony Valada, Philip Zeitler, Pete Zeitler, Christopher Powell, jan bradburn |
| Verified fitting / programming (Real Ear Measurement or detailed programming) | Steve Marsee, Pete Zeitler, Philip Zeitler |
| Family bringing a parent | Rocio M Stevens, Philip Zeitler |
| Spanish-language care | Rocio M Stevens |
| Walk-in hours / same-day repair | Emily Palo |
| Insurance / price / coverage (patient statements) | jan bradburn, Christopher Powell |
| Unhurried, listens, explains | Lena Espana, Rocio M Stevens, Philip Zeitler |
| Returning patient / front desk | Larry Williams Music |

#### Review handling cautions (for the build stage)
- **Title wording.** Reviews 1, 9 and 10 use "Dr." or "doctor" (Flag 5). Without alteration, they would put a doctor title on a page whose own owner has publicly said he is not a medical doctor.
- **Insurance and Medicare.** Reviews 2 and 7 describe their own coverage and pricing outcomes. Flag for client review before use.
- **Duplicate surnames.** Philip Zeitler and Pete Zeitler are separate reviewers. Both mention ReSound hearing aids, so showing both would read as repetitive.
- **Owner replies.** These are part of the Google display and can be included or left out. They are not needed by the brief.
- **Ratings display.** All visible reviews are 5 stars, matching the 5.0 average.
- **Dates.** Google shows relative dates only. If the page shows dates, they should be written generically (for example "Google review") or confirmed against the live listing.


---

## 4. LOCATION INFORMATION

| Item | Detail | Source |
|---|---|---|
| **Practice / legal name on listings** | Altamonte Family Hearing (third-party listings show "Altamonte Family Hearing LLC") | Site, Healthgrades |
| **Street address** | **715 Douglas Ave, Suite 45, Altamonte Springs, FL 32714** | Homepage, /llm-info |
| **Building** | **One Senior Place** | Homepage, /about |
| **Directions detail** | "Just north of Central Parkway" | /llm-info |
| **City / area** | Altamonte Springs (Seminole County, per the Chamber membership) | Site |
| **Main phone** | **407-949-6737** (English and Spanish) | Every page. See Flag 1 for the brief's different number. |
| **Fax** | (407) 604-6692 | /llm-info |
| **WhatsApp** | wa.me/14079496737 | /llm-info |
| **Hours** | Mon–Fri 9:00 am–4:30 pm. Closed for lunch 12:00–1:00 pm. **Walk-in cleanings and minor repairs Mon–Fri 1:00–2:00 pm.** Sat and Sun closed. | /llm-info, homepage |
| **Missed-call policy** | Missed calls returned within one business day | Contact blocks site-wide |
| **Appointments** | Online booking (`/schedule`) or phone | /schedule |
| **Booking portal** | myhearingportal.com (same embed as the brief) | /schedule |
| **Practice email** | Not published on the pages fetched. A Nextdoor listing shows a front-desk address, which is third-party and not used here. | n/a |
| **Google Maps (site)** | `https://www.google.com/maps?cid=12379218337608981477` and embed `...&z=15&output=embed` | Homepage |
| **Google Maps (brief)** | Coordinates **28.676125, -81.3896501**. Place hex ID 0x88e771506ecb647d:0xabcbd17d7a2f5be5. | PROJECT_BRIEF |
| **Nearby areas served (drive time per site)** | Lake Mary (~15 min), Winter Park (~15 min), Maitland (~10 min), Casselberry (~10 min), Longwood (<10 min), Winter Springs (~15 min) | /llm-info |
| **Mobile visit area** | "Greater Orlando area", including Lake Mary, Winter Park, Maitland, Casselberry, Longwood, Winter Springs | /services/mobile-hearing-services |
| **Neighborhood pages on site** | /lake-mary, /winter-park, /maitland, /casselberry, /longwood, /winter-springs (linked; **not fetched**) | Mobile services page |

**Local color that is supported.**
- The office sits inside a senior-services building that patients refer to as the Senior Center or Senior Place (reviews). The site's own name for it is One Senior Place.
- The clinic is the building's certified hearing care provider.
- Reviews describe patients driving 30 minutes to 2 hours, and out-of-state visitors using the practice.

**Not supplied / not found:** parking details, entrance or suite wayfinding inside the building, accessibility details, public transit, and building hours.

---

## 5. PATIENT / CUSTOMER PROBLEMS, MOTIVATIONS & OBJECTIONS

*Grounded in the site's own wording and review themes. This is not psychological speculation.*

### 5.1 Problems prospects are trying to solve
- Not catching words in group or noisy settings (restaurants, parties, car).
- Frequently asking people to repeat themselves, and family or friends noticing it (TV volume, mumbling).
- Phone calls getting harder.
- Ringing, buzzing or humming.
- Blocked, full or muffled ears (possible earwax).
- Hearing aids that stopped working, whistle, or never sounded right.
- Hearing aids that are several years old or fitted elsewhere.
- Hard-to-reach care for a parent or loved one who has stopped driving, is recovering at home, or lives in a facility.

### 5.2 Desired outcomes
- Understand what is going on with their hearing, and whether they need aids at all.
- Follow conversation, TV and phone calls again.
- Comfortable, correctly fitted devices.
- A clear explanation of results, and options that fit lifestyle and budget.
- Ongoing support after the fitting.

### 5.3 Concerns and objections, and what the sources say that could reassure

| Concern | What the sources provide |
|---|---|
| **"Do I even need hearing aids?"** | The site says not every concern calls for aids, and the clinic will tell patients so. A baseline record is still useful. The patient can take the information home and decide when ready. |
| **Fear / anxiety about the test** | Each step is explained and results are reviewed in detail. The ear exam is visible on a screen in the earwax service. Reviews mention nervous and claustrophobic patients who were put at ease. The site says to tell the clinic about discomfort during REM or irrigation. |
| **Cost / "free" claims** | The evaluation is complimentary in most cases, so call to confirm. Hearing aid prices are not published. Reviews mention insurance help and budget-aware recommendations. |
| **Insurance** | The site says it accepts many plans and checks benefits for patients (bring the card). Plans are not named. |
| **Trust / sales pressure** | Reviews describe unhurried, thorough visits and honest recommendations. Verification (REM, EAA) is described as the practice's standard. (An older third-party snippet says the practice's focus is "not on selling hearing aids". This is *not* confirmed on the current site, so do not use it.) |
| **"Will they sound right?" / adjustment** | Follow-ups over the first weeks. The site is open about the adjustment period and says the patient's own voice may sound different at first. |
| **Visibility / style** | The six-style guide and quiz are on the site. Discreet IIC/CIC options are discussed, and suitability depends on hearing and ear anatomy. |
| **Handling small devices and tech** | Coaching on insertion, removal, care, and phone and app pairing. Rechargeable options exist. |
| **Time and convenience** | Walk-in hour for minor repairs. Mobile visits. Missed calls are returned within one business day. The length of the first appointment is not stated (it is confirmed when scheduling). |
| **Language** | Spanish evaluations, forms and a Spanish page. |
| **Hearing aids bought elsewhere** | Cleaning, troubleshooting, programming and repairs are offered for most major brands. REM can verify them. |
| **Bringing a family member** | Explicitly welcomed at results reviews and home visits (with the patient's permission). |
| **Medical urgency** | The sudden-hearing-loss warning, referral language, and "seek care now" red flags are on the site. |

---

## 6. FAQ SOURCE MATERIAL

*Approximately 15 candidate questions with the factual material available to answer each. No final answers are written here. All answers must be cleared against the live page named in each source note.*

**Q1. How do I know if I have hearing loss?**
- The five signs on `/hearing-loss`; the extra signs on `/services/hearing-tests`.
- A hearing evaluation clarifies what is happening. Hearing changes are often gradual.
- *Sources: /hearing-loss, /services/hearing-tests*

**Q2. What happens at my first hearing evaluation?**
- Four steps: consultation, ear exam, sound-booth hearing test, results explained. Same-day results explanation.
- Bring a family member or friend, your insurance card, a medication list and any current hearing aids.
- The length of the appointment is not stated.
- *Sources: /services/hearing-tests, /schedule, /about FAQ*

**Q3. Is the hearing test free?**
- Most evaluations are complimentary. Call to confirm any cost for your appointment.
- Homepage CTA uses "complimentary hearing evaluation".
- *Sources: /services/hearing-tests FAQ, homepage*

**Q4. What if I don't need hearing aids?**
- The clinic will say so. Recommendations are based on test results. You leave with a record of your hearing.
- Not every hearing concern calls for hearing aids.
- *Source: /services/hearing-tests FAQ*

**Q5. Can hearing loss be treated or reversed?**
- Sensorineural: usually permanent, and hearing aids may help. Conductive: often treatable (medical care, wax removal, surgery). Mixed: partly treatable.
- Some findings need medical referral.
- *Source: /hearing-loss*

**Q6. Can hearing loss happen suddenly, and what should I do?**
- A sudden drop over hours or days is a medical emergency. Do not wait for a routine appointment. Prompt treatment can improve the chance of recovery.
- *Sources: /hearing-loss, /services/tinnitus, /services/earwax-removal*

**Q7. What is Real Ear Measurement and why does it matter?**
- A probe tube measures the sound in your ear canal with the hearing aid in. It is compared with your prescriptive targets and used to adjust the aid.
- Fitting software uses average ear canal values, and REM measures yours.
- It is a central part of the HearingUp standard.
- *Sources: /services/real-ear-measurement, /about/best-practices*

**Q8. Which hearing aid brands do you offer, and how do you choose?**
- Phonak, Oticon, ReSound, Signia, Starkey, Widex. Not tied to a single manufacturer.
- Recommendations are based on results, daily routine, budget and preferences.
- Most hearing aids come in multiple technology levels, chosen after the evaluation.
- *Sources: /about FAQ, /hearing-aids, /services/hearing-aid-fittings*

**Q9. What's included after I get hearing aids?**
- Five years of professional care at every technology level. Follow-up visits over the first weeks. Cleanings are part of ongoing professional care for aids bought from the office.
- A stated 100% satisfaction guarantee (terms not provided).
- *Sources: homepage, /about, /hearing-aids, /services/hearing-aid-repair*

**Q10. Do you take my insurance? Will insurance cover hearing aids?**
- Many plans accepted. Plans are not named. Coverage varies by plan. Some plans help with part of the cost. The clinic checks benefits if you bring the card or call.
- *Sources: /hearing-aids FAQ, /about FAQ, service-page FAQs*

**Q11. How long does it take to get used to hearing aids?**
- It varies. Familiar sounds and your own voice may seem different at first. Regular use and follow-up visits help.
- *Source: /services/hearing-aid-fittings FAQ*

**Q12. Will hearing aids help in noisy places or with tinnitus?**
- Many have features that make speech easier to follow in noise, but none remove background noise completely.
- For people with hearing loss, tinnitus may become less noticeable. Relief varies. There is no universal cure.
- *Sources: /hearing-aids FAQ, /services/tinnitus FAQ*

**Q13. How are professional hearing aids different from over-the-counter hearing aids or AirPods?**
- OTC aids and certain AirPods Pro models are intended for adults 18+ with perceived mild-to-moderate loss. A hearing evaluation helps compare options. Aids from the office include professional fitting and ongoing care.
- *Source: /hearing-aids FAQ*

**Q14. Can you help with hearing aids I already own, including ones from another provider?**
- Yes for most major brands: cleaning, troubleshooting, reprogramming, repairs. Some repairs need the manufacturer. Walk-in cleanings and minor repairs run Mon–Fri 1–2 pm.
- REM can verify the existing fitting.
- *Sources: /services/hearing-aid-repair, /services/real-ear-measurement, /about/best-practices*

**Q15. Do you offer care in Spanish, and can you come to my home?**
- Spanish: evaluations, patient forms, a Spanish page, a bilingual team.
- Mobile: home or care-facility visits in the greater Orlando area. Call for availability and cost.
- *Sources: /hearingup-jaysee-soto FAQ, /about, /services/mobile-hearing-services*

---

## 7. CONTENT INVENTORY

Existing site content that can feed each landing-page area. Nothing here is compressed, and all of it is source material.

| Landing-page area | Usable existing content (and where) |
|---|---|
| **Hero / value proposition** | Homepage H1 "Hearing Care That Feels Like Family". Descriptor: family-owned, in Altamonte Springs, comprehensive evaluations, personalized hearing aid solutions, ongoing care (homepage). Meta line: hearing evaluations, aids from leading manufacturers, Real Ear Measurement. Hablamos español. The "now accepting new patients" note. The trust badge needs the rating (see Flags 1–2). |
| **Benefits** | §2.5 and §2.11. The homepage "why patients choose us" bullets (small local team, Spanish, walk-in hour, inside One Senior Place). The homepage "best practices" bullets (evaluation, REM verification, ongoing care, six manufacturers, care for aids from other providers). |
| **Symptoms / problems** | `/hearing-loss` five signs. `/services/hearing-tests` "signs it may be time". `/hearing-aids` FAQ "How do I know if I need hearing aids?". The hearing-loss types table (§2.3). |
| **Services / treatments** | The seven services with the one-line descriptions on the homepage and `/llm-info`. Per-service detail pages (§2.6). |
| **Provider / about** | `/about/jaysee-soto`, `/about/toni-trager`, `/about` (credentials block, "How our practice began"), `/hearingup-jaysee-soto`. Grace and Francesca roles on `/about`. |
| **Process / how it works** | Hearing test 4 steps. `/hearing-loss` 3 steps ("what to do next"). Fitting 4 steps. REM 4 steps. First-visit text on `/about` FAQ and `/schedule`. |
| **Technology** | Sound booth, video otoscope, EAA, REM, Earigator. Hearing aid styles and features list (`/hearing-aids`). Six brands with named current models. |
| **Testimonials / reviews** | Supplied Google screenshots are the source of record per the brief: 10 full-text reviews in §3A (2 more cut off). `/reviews` (Google, shown as 155, now known to be out of date) and the homepage and service pages carry additional excerpts. Theme map in §3. |
| **FAQs** | §6, plus the existing FAQ blocks on the homepage-linked pages (`/hearing-aids`, `/about`, `/hearing-loss`, `/hearingup-jaysee-soto`, each service page). |
| **Location** | Address, directions note, hours, nearby-community list and drive times (§4). The map link and embed URL on the homepage. "Get directions" is already a pattern on the site. |
| **Appointment / contact** | Booking embed (identical to `/schedule`). What to bring (insurance card, medication list, current hearing aids; family member welcome). "Missed calls returned within one business day". The site's contact copy pattern: "Book your hearing evaluation online or call". |
| **Final CTA** | "Schedule your hearing evaluation" block (repeated at the bottom of site pages). Walk-in hour as a secondary option for existing aid wearers. |

---

## 8. BRAND EXTRACTION

**Method limit.** The pages were retrieved as text and markup content. The site's CSS, font files and image pixels were not accessible, and the logo files could not be fetched. Everything below is split into *confirmed*, *inferred* and *not determined*.

| Item | Status | Finding |
|---|---|---|
| **Primary color** | **Partially confirmed** | Every page declares `theme-color` **#1A3028** (a very dark forest green). It is a browser-chrome value, so it likely reflects the brand's dominant color but is not proof of the CTA/button color. |
| **Secondary color** | **Not determined** | No second color value is exposed. The brief assigns the secondary color to the mobile sticky call button's text and icon, so this one needs to be sampled. |
| **Supporting colors** | **Not determined** | Visual clues only (alt text): green armchairs in the office, staff in green scrubs and white coats. This suggests green plus neutral/white. Exact values unknown. |
| **Heading font** | **Not determined** | Headings on most pages use an emphasized phrase inside the headline (for example, "Meet the people *behind your care*"), which suggests a two-style heading treatment, likely an italic or accent style. The typeface is unknown. |
| **Body font** | **Not determined** | No font names in the content. |
| **Button style** | **Not determined** | Button labels are sentence-case and action-led (for example "Book your hearing test", "or call 407-949-6737"). Shape, radius and color unknown. |
| **Border radius** | **Not determined** | |
| **Card treatment** | **Not determined** | Content is organized as step lists, tables, FAQ accordions and card-style listings, but the visual treatment is unknown. |
| **General visual characteristics** | **Inferred (weakly)** | Warm, approachable, "family" tone. Real photography. Clean clinical content structure (steps, "what to expect", "before your visit"). Light interactive elements (sound demo slider, style quiz). The site was designed by Audflow (footer credit) and built with Astro, with images served through a Netlify image CDN. |
| **Photography style** | **Confirmed from alt text** | Candid, real photography of the actual team and patients in the actual office: front desk and team group shots, patient care close-ups (video otoscope, sound booth, REM probe, repair bench, Earigator), portraits of the specialists in white coats. No stock-photo descriptions. |
| **Logo** | **Exists, not inspected** | Site logo: `https://altamontefamilyhearing.com/assets/logo-altamonte-626.png`. White version: `.../logo-altamonte-white-626.png`. The brief's logo URL is hosted on filesafe.space and was not retrieved. |

**Recommendation for the next stage:** sample the logo directly and inspect the live site's computed styles (colors, fonts, button radius) before locking the palette. The brief's mobile sticky CTA rule (Primary background, Secondary text and icon) cannot be satisfied until a secondary color is confirmed.

---

## 9. IMAGE / VISUAL SOURCE INVENTORY

*Inventory only. Nothing was downloaded. All assets are on the clinic's own domain unless noted. Descriptions come from the site's alt text. Reuse rights for the clinic's own photos are presumably fine for the clinic's own landing page, but confirm with the client. Manufacturer and HearingUp logos are third-party trademarks.*

### Logos, badges and marks
- Clinic logo (color): `/assets/logo-altamonte-626.png`
- Clinic logo (white): `/assets/logo-altamonte-white-626.png`
- Brief-supplied logo: `assets.cdn.filesafe.space/3o0LBBSuVEkoaohgGtT0/media/6ac7f45989da6e6f9bbdacc8.png` (not retrieved)
- HearingUp "Network by Dr. Cliff" logo: `/assets/logos/hearingup-dr-cliff.webp`
- Hearing aid manufacturer SVGs: `/assets/brands/{phonak,oticon,resound,signia,starkey,widex}.svg`
- Hearing aid style icons: `/assets/styles/{ric,bte,ite,itc,cic,iic}.svg`
- Social share image: `/assets/og/altamonte-family-hearing-og.jpg`

### Clinic interior and equipment
- Patient in headphones in the sound booth, holding the response button (AFH-C-42). Patient in the sound booth smiling (AFH-C-40). Jaysee with thumbs up at his desk while the patient is in the booth (AFH-C-38).
- Real Ear Measurement probe-tube close-ups (AFH-C-196, AFH-C-195, AFH-C-194, AFH-C-60).
- Video otoscope exam (AFH-C-28, AFH-C-27).
- Repair bench / hearing aid cleaning (AFH-C-125, AFH-C-130, AFH-C-138, AFH-B-10).
- Earigator earwax irrigation (AFH-C-122, AFH-C-123, AFH-C-113).
- Patient reading in a green armchair, hand at ear (AFH-C-109).
- Hearing aid being fitted and placed, with mirror (AFH-C-159, AFH-C-156, AFH-B-17).
- Consultation desk shots: audiogram explanation (AFH-B-3), options discussion (AFH-C-173, AFH-C-168, AFH-C-31), features discussion (AFH-C-142).
- Practice exterior or sign: the "Altamonte Family Hearing sign" appears behind the team in several photos. **No dedicated exterior or building photo was identified.**

### Provider / team portraits
- Jaysee portrait in white coat (`jaysee-portrait.webp`, `jaysee-about.webp`). Jaysee in the sound booth in white coat (AFH-B-14).
- Toni portrait in white coat (`staff-AE8A1494.webp`; also on Sanity CDN).
- Grace and Francesca portraits in green scrubs (Sanity CDN: cdn.sanity.io/images/p8cei03q/...).
- Team group photos: all four in front of the sign (`staff-AE8A1554-3.webp`, AE8A1534, AFH-A-27, AFH-C-97 heart-shape, AFH-C-100 laughing with a patient at the front desk, AFH-C-75 hugging a patient, AFH-A-18 celebration with cake).
- Front-desk welcome (AFH-A-16, AFH-C-163).

### Video and audio
- Welcome video (about 2 minutes): `/assets/video/welcome-crop-loop.mp4` with a poster image `welcome-crop-poster.webp`.
- YouTube: @baldhearingguy (channel). A video thumbnail is on the HearingUp page.
- Interactive sound demo (speech-in-noise slider) and style quiz exist on the site but are site-built widgets, not static assets.

### Reviewer assets
- Review avatar/crop images stored at `/assets/reviews/*.webp` for several reviewers. Google profile avatars also appear on `/reviews`. **Reusing reviewer photos needs care. Prefer the supplied screenshots.**

### Local/location photography
- **None found** beyond the in-office imagery above. Google Business Profile photos are to be supplied by the user (not received).

---

## 10. MISSING INFORMATION

Items requested in PROJECT_BRIEF.md, or reasonably needed, that cannot be verified from the available sources.

**From the brief, unresolved**
1. **Google Reviews screenshots/images**: **partly supplied.** 10 reviews have full text (§3A). Jason Hoch and Teri Yanovitch are cut off. Steve Marsee's review should be checked against the live listing (§3A, review 6). More screenshots are welcome, especially short reviews without a "Dr." title.
2. ~~Authoritative Google rating and review count~~ **Resolved:** 5.0 stars, 157 reviews on the live Google listing (Oct 12, 2026). See Flag 2.
3. **GBP/Google Business Profile photos**: still not supplied.
4. **Brand colors and fonts**: placeholders were AUTO-DETECT. Only #1A3028 was found, and only as a theme-color (§8).
5. **Phone 407-809-8154**: not found in any source. The clinic's published number is 407-949-6737 (Flag 1).
6. **`{{location.name}}` value** for the footer (Flag 9).
7. **Privacy Policy and Terms of Use pages**: the URLs in the brief match the site's footer links (`/privacy-policy`, `/terms-of-use`), but the page content was not read.

**Not stated on the clinic's site**
8. **Hearing aid prices, financing or payment plans.** None published. Reviews comment on pricing in opinion only.
9. **Specific insurance plans accepted** (the site says "many"). **Medicare/VA participation** is not stated by the clinic. One review mentions Medicare coverage and another mentions VA-issued aids, but these are patient statements.
10. **Satisfaction guarantee terms**: trial period length, refund conditions, any restocking terms.
11. **What "five years of professional care" includes in detail** (visits, cleanings, adjustments, repairs, loss/damage).
12. **Manufacturer warranty lengths** and loss/damage coverage.
13. **Length of the first appointment** and of a fitting. Both are "confirmed when you schedule".
14. **Practice founding year** (and years at the current location).
15. **Parking, building entrance/wayfinding, accessibility**, and One Senior Place building access hours.
16. **Whether the practice treats patients under 18** (current site: adults).
17. **Any awards, press or media recognition**. None found.
18. **Specific community events or sponsorships.** The site says it shares hearing health education but names nothing.
19. **State license numbers** and a public verification link for the Hearing Aid Specialist licenses.
20. **Cost and fee for mobile visits** (the site says call), and any fee for earwax removal.
21. **A published practice email.** The pages fetched list only phone, WhatsApp, fax and a contact form.
22. **Technical attributes of the supplied booking iframe**: height/width and whether it needs resizing in a popup (the embed code has none).

**Fetch limitations**
- The Healthy Hearing and HearingTracker profile pages appeared only as search snippets and were not fetched in full.
- Six neighborhood pages (`/lake-mary`, `/winter-park`, `/maitland`, `/casselberry`, `/longwood`, `/winter-springs`), `/services`, `/videos`, `/contact`, `/patient-forms`, `/es`, `/about/grace-soto`, `/about/francesca-natal` and the six per-brand pages (`/hearing-aids/{phonak,oticon,resound,signia,starkey,widex}`) were not read. They may contain additional usable facts.
- The reviews page fetch was truncated near the end (reviews back to about Feb 2020 were visible). Older reviews exist beyond that.

---

## SOURCE LOG

**Clinic site (primary)**
- https://altamontefamilyhearing.com/ (homepage)
- /hearing-loss
- /hearing-aids
- /about, /about/best-practices, /about/jaysee-soto, /about/toni-trager
- /hearingup-jaysee-soto
- /services/hearing-tests, /services/hearing-aid-fittings, /services/real-ear-measurement
- /services/tinnitus, /services/earwax-removal, /services/hearing-aid-repair, /services/mobile-hearing-services
- /reviews, /schedule
- /llm-info (practice information page; "Last updated: October 6, 2026")

**Third-party (cross-check only)**
- HearingTracker, Healthgrades, Healthy Hearing, Nextdoor, Seminole County business directory, Yelp (search snippets). These were used for the phone/address cross-check, the Yelp rating and the unverified Healthgrades education line. They are not used as a basis for claims.

**Provided by the user**
- Six Google Reviews screenshots (Google listing, captured Oct 12, 2026), used for §3A, Flag 2 and the phone cross-check.
- PROJECT_BRIEF.md (Altamonte Family Hearing, Hearing Loss).
