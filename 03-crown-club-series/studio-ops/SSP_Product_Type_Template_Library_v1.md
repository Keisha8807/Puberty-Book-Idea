# Sunray Story Press — Product Type Template Library v1.0

**Version:** 1.0  
**Date:** May 2026  
**Status:** Cleaned support reference for SSP production system  
**Recommended Drive Location:** `Sunray Story Press / 02_Template_Engines / Template_Docs/`  
**Recommended Project Status:** Support reference, not required in the active Core Binder unless actively building product templates.

---

## 1. Purpose

This document is the cleaned master library for reusable **Sunray Story Press product-type templates**. It translates raw template notes into a structured production reference that agents can use to choose product formats, assign page structures, map teacher/support pages, and prepare product build packets.

The goal is to make production more plug-and-play by separating:

- **Product type structure**: what pages a product should include
- **Theme variables**: season, subject, cultural focus, palette, icons, and clipart
- **Grade-level expectations**: writing-line style, directions length, page complexity, and response depth
- **Preview strategy**: which 4 listing images best sell the product
- **Reusable teacher/support pages**: which support pages are standard for that product type

This document should work alongside:

- `SSP_Product_Config_Template.json`
- `SSP_Preview_Manifest_Template.md`
- `SSP_Asset_System.md`
- `SSP_Teacher_Page_System.md`
- `SSP_Preview_Mockup_Copy_System.md`
- `SSP_Platform_Compliance_Upload_System.md`

---

## 2. How Agents Use This Library

### Agent 1C — Resource Type + Store Shelf Mapper
Uses this library to decide which product family an opportunity belongs to.

Example:

- “Kindness Bingo” → Bingo / Interactive Game Pack
- “Hygiene Picture Sorts” → Cut-and-Paste Sort Pack or Hygiene / Life Skills Mini-Pack
- “Fall Scissor Skills” → Fine Motor / Scissor Skills Pack
- “Special Person Writing” → Writing Craft + Keepsake Pack

### Agent 2 — Offer + SEO Architect
Uses the selected template to define the product promise, title, what’s included, preview image plan, price band, and bundle path.

### Agent 3 — Curriculum + Product Content Designer
Uses the page architecture to draft student pages, teacher guide text, directions, differentiation, extension ideas, and answer keys when applicable.

### Agent 4 — Creative Production + Design System Agent
Uses template rules to create design directions, required assets, product config fields, teacher page layouts, and preview manifest details.

### Agent 5 — Packaging + QA + Upload Prep Agent
Checks that the final product includes the right files, page types, preview images, naming conventions, and buyer-facing assets.

### Mira — Metrics + Productization Logger
Tracks which template family was used, how long production took, what became a brand variable, what became an engine rule, and whether the template improved speed.

---

## 3. Global Template Rules

These apply to all product-type templates unless a stricter template-specific rule is provided.

### 3.1 Page Size and Export Rules

| Asset Type | Required Size | Notes |
|---|---:|---|
| Printable student pages | 8.5 × 11 in | US Letter, portrait |
| Printable teacher/support pages | 8.5 × 11 in | Full color unless otherwise noted |
| Marketplace listing images | 1200 × 1200 px | Exactly 4 required TPT listing images |
| Preview/sample PDF | Built from listing images | Uses the same 4 listing images unless product-specific exception is approved |
| Worksheet PNG previews | 2550 × 3300 px | Optional raster preview of printable page |

### 3.2 Footer Rule

Every printable page should include:

`© Sunray Story Press • For single classroom use only • Not for redistribution`

For future productized versions, this becomes a brand variable:

`© [Store Name] • For single classroom use only • Not for redistribution`

### 3.3 Typography Rule

Use the locked SSP font system unless the product config overrides it with an approved brand setup value.

- **Headline font:** Fredoka One
- **Body font:** Nunito
- **Student directions:** Nunito or Nunito Sans
- **Internal system docs:** clean readable font; does not need to be kid-friendly

### 3.4 Writing Line Rules by Grade Band

| Grade Band | Writing Line Style | Response Expectation |
|---|---|---|
| PreK | large drawing spaces, minimal tracing or name line | draw, color, trace, circle |
| Kindergarten | primary dashed middle-line writing lines | words, sentence frames, short phrases |
| Grade 1 | dashed middle-line primary writing lines | 1–3 sentence frames |
| Grades 2–3 | single solid lines | 2–4 complete sentences |
| Grades 4–5 | single solid lines or paragraph boxes | paragraphs, reasoning, text evidence |
| Grades 6–8 | academic boxes / paragraph response areas | evidence, analysis, CER, synthesis |

### 3.5 Student Page Design Rules

- Student pages should be black-and-white unless intentionally designed as full-color student materials.
- Keep writing areas white or cream.
- Use generous spacing.
- Avoid clutter near writing lines.
- Use thick black outlines for coloring, cutting, tracing, and visual clarity.
- Use print-safe margins.
- Do not place heavy backgrounds behind student writing areas.

### 3.6 Teacher and Support Page Design Rules

Teacher/support pages should feel polished and branded, not plain.

Use:

- bold title headers
- section cards or content boxes
- icon accents
- footer branding
- theme-appropriate decorative accents
- real logo in safe zone
- full-color layout

Avoid:

- plain text walls
- excessive empty lower-third whitespace
- emoji graphics
- unapproved fonts
- overly busy borders on standard Tier 1 products

### 3.7 Character Representation Rule

When people, children, families, teachers, or community members appear:

- **Black-focused products:** Black children/families with varied natural hairstyles and a range of warm brown skin tones.
- **Spanish/Latino-focused products:** Latino children/families with respectful, varied representation.
- **Asian-focused products:** East, South, and/or Southeast Asian children represented appropriately based on product focus.
- **Indigenous/Native-focused products:** respectful, non-stereotyped representation; avoid generic or pan-tribal symbols unless approved.
- **Multiracial products:** blended family contexts and varied features.
- **General products:** diverse mix of children across skin tones, hair textures, cultures, body types, and abilities.

Never default to one skin tone in group scenes. Representation should be intentional, respectful, and age-appropriate.

### 3.8 Cultural / Heritage Style Rule

Kente-inspired borders or rich cultural borders should be used **only** for relevant cultural products such as Juneteenth, Black History Month, African heritage products, or approved Tier 2 cultural products.

Do not apply cultural borders to generic evergreen products just because they look visually rich.

### 3.9 Sensitive Topic Flag

Any product touching hygiene, puberty, body changes, body safety, personal boundaries, health education, SEL emotions, family structure, identity, trauma, or mental health must pause before content or images are generated.

Owner approval is required before proceeding.


### 3.11 Combined Final Support Page Rule

Thank You, Credits, and Terms of Use are always combined into one final support page.

Default page name: **Thank You / Credits / Terms**

This page should include a warm thank-you message, review/follow request, Terms of Use, credits for fonts/graphics/clipart/assets, copyright line, and related products or store connection when applicable.

Do not list Thank You and Terms of Use as two separate required pages unless Keisha explicitly approves a product-specific exception. This is an Engine Rule.

### 3.10 Answer Key Rule

Only include an answer key if the product genuinely has correct/incorrect responses.

Examples:

- Sorting pack → likely needs answer key or sample sort.
- Math pack → likely needs answer key.
- Cutting practice → answer key does not apply.
- Writing craft → answer key does not apply unless rubric is included.

---

## 4. Product Type Families

Each family below includes the recommended use case, page range, price band, preview strategy, bundle path, standard pages, and optional variations.

---

### 4.1 Fine Motor / Scissor Skills Pack

**Best For:** Tracing, cutting, pre-writing, grip practice, line practice, shape cutting, cut-and-glue packs  
**Typical Page Count:** 8–20  
**Price Band:** $3–$6  
**Bundle Path:** Single theme → seasonal bundle → fine motor mega bundle  
**Primary Grade Bands:** PreK–K, PreK–1, K–2  
**Style Tier:** Tier 1 Standard

#### Standard Outputs

1. Cover page
2. Teacher guide
3. How to use page
4. Skill progression chart
5. Student worksheet pages
6. Thank You / Credits / Terms page
7. 4 listing images
8. Preview/sample PDF
9. Buyer product PDF or ZIP

#### Standard Student Page Types

- Straight line practice
- Curved line practice
- Zigzag line practice
- Shape cutting practice
- Cut-and-glue picture pages
- Mixed skill review page
- Optional certificate or cutting mat

#### Required Design Rules

- Large clear dashed lines
- Thick black outlines
- White space around each cutting shape
- Clipart must not touch or overlap dotted cutting lines
- Line spacing must support early scissor practice
- Right- and left-handed versions when applicable

#### Default 4 Listing Images

1. **Cover** — what the product is
2. **What’s Included** — number of pages, versions, teacher pages
3. **Right + Left Versions** — buyer benefit and differentiation
4. **Use It Your Way** — Color → Cut → Glue → Display workflow

#### Notes

Skill progression should appear in the teacher/support pages and can be referenced in What’s Included. It does not need to consume one of the 4 required listing image slots unless the owner approves a product-specific exception.

---

### 4.2 Cut-and-Paste Sort Pack

**Best For:** SEL, hygiene, life skills, sequencing, categories, healthy habits, community helpers, science sorts  
**Typical Page Count:** 10–18  
**Price Band:** $3–$5  
**Bundle Path:** mini packs → topic bundle → life skills/SEL mega bundle  
**Primary Grade Bands:** PreK–2, K–3  
**Style Tier:** Tier 1 Standard unless culturally specific or sensitive topic review applies

#### Standard Outputs

1. Cover page
2. Teacher guide
3. How to use page
4. Sorting mats
5. Picture cards
6. Recording sheets
7. Answer key or sample sort when applicable
8. Thank You / Credits / Terms page
9. Listing images and preview PDF

#### Standard Student Page Types

- Sorting mat A/B
- Sorting mat with 2–4 categories
- Cut-out picture cards
- Recording sheet
- Reflection response sheet
- Optional home connection activity

#### Required Design Rules

- Extra thick dashed cut lines on cards
- Clear category labels
- Large visuals for young learners
- Picture cards should include word labels when grade-appropriate
- If there is one correct sort, include answer key or sample sort

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Sorting Mats + Cards
4. Use It Your Way / Centers + Whole Group

---

### 4.3 Coloring + Writing Craft Pack

**Best For:** Gratitude, kindness, family, special person, peace day, self-esteem, holiday writing, keepsakes  
**Typical Page Count:** 8–16  
**Price Band:** $3–$5  
**Bundle Path:** single theme → seasonal series → appreciation/SEL bundle  
**Primary Grade Bands:** K–5, with line style adjusted by grade  
**Style Tier:** Tier 1 Standard or Tier 2 if cultural/heritage focus

#### Standard Outputs

1. Cover
2. Teacher guide
3. Planning page
4. Coloring/writing pages
5. Craft or assembly page
6. Final keepsake page
7. Reflection page
8. Thank You / Credits / Terms page
9. Listing images and preview PDF

#### Standard Student Page Types

- Coloring page with writing prompt
- Gratitude / kindness / family sentence frame page
- Main writing page
- Craft assembly page
- Reflection page
- Certificate or keepsake page

#### Required Design Rules

- Thick outlines for coloring
- Writing spaces adjust by grade band
- Craft pieces must have clear cut lines
- Assembly directions must be simple and visual
- Family/special person prompts should be inclusive of varied family structures

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Student Page Samples
4. Finished Keepsake / Use It Your Way

---

### 4.4 Bingo / Interactive Game Pack

**Best For:** SEL, vocabulary, seasonal review, classroom games, life skills practice  
**Typical Page Count:** 12–25  
**Price Band:** $4–$7  
**Bundle Path:** theme bingo → category bundle → game bundle  
**Primary Grade Bands:** K–5  
**Style Tier:** Tier 1 Standard

#### Standard Outputs

1. Cover
2. Teacher guide
3. How to play page
4. Bingo boards
5. Calling cards
6. Markers/tokens page
7. Optional winner certificate
8. Optional blank board
9. Answer/calling key if applicable
10. Listing images and preview PDF

#### Standard Page Types

- 6–8 unique bingo boards
- Color version and/or black-and-white version
- Calling cards with picture + word
- Tokens / markers
- Extension ideas
- Blank customizable board

#### Required Design Rules

- High contrast board design
- Large readable words
- Clear card borders
- Consistent board grid
- Calling cards must match board content exactly

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Sample Boards + Calling Cards
4. Ways to Play / Centers / Whole Group

---

### 4.5 Emergent Reader / Mini Book Pack

**Best For:** Decodable/emergent readers, guided reading, sight words, take-home readers  
**Typical Page Count:** 6–12  
**Price Band:** $3–$6  
**Bundle Path:** leveled reader → skill series → reading bundle  
**Primary Grade Bands:** PreK–1, K–2  
**Style Tier:** Tier 1 Standard or Tier 2 for cultural/heritage reader

#### Standard Outputs

1. Cover
2. Teacher guide
3. Mini book pages
4. Comprehension extension
5. Black-and-white student version
6. Assembly directions
7. Sight word or phonics list
8. Thank You / Credits / Terms page
9. Listing images and preview PDF

#### Standard Page Types

- Title page
- 6–10 mini book pages
- Repetitive text pages
- Picture-supported vocabulary
- Simple comprehension questions
- Favorite part drawing/writing page
- Assembly page

#### Required Design Rules

- Large early-reader font
- Strong picture support
- Repetitive sentence patterns
- Predictable page structure
- Optional 2-up printing/folding layout if specified

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Sample Reader Pages
4. Teacher Notes / Take-Home Use

---

### 4.6 Phonics / Decodable Pack

**Best For:** Phonics patterns, word families, decodable sentences, fluency practice  
**Typical Page Count:** 8–20  
**Price Band:** $3–$6  
**Bundle Path:** single phonics pattern → phonics series → decodable bundle  
**Primary Grade Bands:** K–2  
**Style Tier:** Tier 1 Standard

#### Standard Outputs

1. Cover
2. Teacher guide
3. Phonics anchor page
4. Word work pages
5. Decodable sentence/passage pages
6. Fluency/comprehension page
7. Bonus game or certificate
8. Answer key if needed
9. Thank You / Credits / Terms page

#### Standard Page Types

- Target sound/pattern anchor
- Tap-and-blend boxes
- Word sort
- Build-a-word
- Read and highlight
- Fluency pyramid
- Simple comprehension questions
- Roll and read / bingo / word hunt

#### Required Design Rules

- Heavy picture support for K–1
- Large readable type
- Clear target phonics pattern emphasis
- Avoid clutter around word work areas

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Word Work + Decodable Pages
4. Fluency / Use It Your Way

---

### 4.7 Reading Mini-Pack

**Best For:** Picture books, read-alouds, poems, nonfiction texts, seasonal texts, book companion packs  
**Typical Page Count:** 12  
**Price Band:** $4–$7  
**Bundle Path:** single book companion → author/theme bundle → reading comprehension bundle  
**Primary Grade Bands:** 1, 2–3, 4–5  
**Style Tier:** Tier 1 Standard or Tier 2 if cultural/heritage book focus

#### Standard Outputs

1. Cover
2. Teacher guide
3. Vocabulary page
4. Character page
5. Setting page
6. Sequencing page
7. Comprehension questions
8. Character feelings/SEL page
9. Identity or connection page
10. Writing prompt
11. Exit ticket
12. Bonus vocabulary flashcards or extension

#### Grade-Level Adaptation

**1st Grade:** dashed middle-line primary writing lines, sentence frames, picture support.  
**2nd–3rd Grade:** solid lines, 2–4 sentence responses, more text evidence.  
**4th–5th Grade:** paragraph responses, inference, theme, point of view, and evidence.

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Student Pages / Reading Skills
4. 5-Day Use / Teacher Support

---

### 4.8 SEL Mini-Pack

**Best For:** emotions, identity, friendship, kindness, growth mindset, resilience, gratitude, self-awareness  
**Typical Page Count:** 8–15 or 12-page universal structure  
**Price Band:** $3–$5  
**Bundle Path:** single SEL theme → SEL series → social-emotional bundle  
**Primary Grade Bands:** K–5  
**Style Tier:** Tier 1 Standard; sensitive topic review may apply

#### Standard Outputs

1. Cover
2. Teacher guide
3. SEL vocabulary
4. Feelings check-in
5. Identity page
6. Belonging/pride/community page
7. Scenario or role-play page
8. Kindness/community activity
9. Writing or reflection prompt
10. Exit ticket
11. Bonus affirmation or keepsake page
12. Thank You / Credits / Terms page

#### Required Design Rules

- Trauma-informed, dignity-first language
- Avoid shaming or deficit framing
- Use diverse representation
- Emotion faces should be clear and respectful
- Sensitive topics pause for owner approval

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. SEL Activities / Reflection Pages
4. Use It Your Way / Morning Meeting / Centers

---

### 4.9 Science Mini-Pack

**Best For:** plants, weather, animals, magnets, states of matter, force/motion, science inquiry  
**Typical Page Count:** 12  
**Price Band:** $4–$7  
**Bundle Path:** single concept → science unit bundle → cross-curricular science series  
**Primary Grade Bands:** K–2, 3–5  
**Style Tier:** Tier 1 Standard or Tier 2 cultural/premium science when applicable

#### Standard Outputs

1. Cover
2. Teacher guide
3. Science vocabulary
4. Concept anchor
5. Observe activity
6. Record activity
7. Predict and observe
8. Data collection
9. Compare and analyze
10. Science + SEL reflection
11. Exit ticket
12. Thank You / Credits / Terms page

#### Grade-Level Adaptation

**K–2:** drawing, labeling, simple observation, picture support.  
**3–5:** data analysis, variables, conclusions, compare/contrast, claim-evidence-reasoning.

#### Required Design Rules

- Student pages mostly black-and-white
- Cover and teacher guide full color
- Clear diagram spaces
- Graphs/tables must be large enough for students
- Align to NGSS when applicable

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Science Activities / Student Pages
4. Use It Your Way / Inquiry Flow

---

### 4.10 Math Mini-Pack

**Best For:** number sense, operations, fractions, geometry, measurement, data, seasonal math  
**Typical Page Count:** 10–12  
**Price Band:** $3–$7  
**Bundle Path:** single skill → skill series → math bundle  
**Primary Grade Bands:** K–1, 2–3, 4–5  
**Style Tier:** Tier 1 Standard

#### Standard Outputs

1. Cover
2. Teacher guide
3. Math vocabulary
4. Concept anchor
5. Core skill page 1
6. Core skill page 2
7. Word problems
8. Patterns/shapes/measurement page
9. Data page
10. Math + SEL reflection
11. Exit ticket
12. Bonus page / math tools / certificate

#### Grade-Level Adaptation

**K–1:** visuals, tracing, drawing, circling.  
**2–3:** show your work, short explanations.  
**4–5:** multi-step problems, reasoning, written explanations.

#### Required Design Rules

- Plenty of workspace
- Clear math models
- Answer key when responses are objective
- Avoid tiny tables/graphs

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Skill Practice Pages
4. Use It Your Way / Centers / Independent Practice

---

### 4.11 Social Studies Mini-Pack

**Best For:** community, identity, traditions, citizenship, symbols, maps, timelines, heritage topics  
**Typical Page Count:** 10–12  
**Price Band:** $4–$7  
**Bundle Path:** single topic → social studies unit bundle → heritage/civic learning series  
**Primary Grade Bands:** K–5  
**Style Tier:** Tier 1 Standard or Tier 2 cultural/heritage

#### Standard Outputs

1. Cover
2. Teacher guide
3. Vocabulary
4. Community/identity page
5. Symbols/key concepts page
6. Then-and-now or traditions page
7. Fairness/rules/citizenship page
8. Timeline or map page
9. Heroes/helpers page
10. Reflection/connection page
11. Exit ticket
12. Bonus celebration/keepsake page

#### Required Design Rules

- Agency-centered representation
- Avoid trauma-first framing
- Use respectful historical language
- Sensitivity review for cultural, identity, or historical oppression topics

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Student Activities / Social Studies Skills
4. Use It Your Way / Cross-Curricular Connections

---

### 4.12 STEM / Hands-On Mini-Pack

**Best For:** STEM challenges, engineering projects, science experiments, makerspace, design thinking  
**Typical Page Count:** 12  
**Price Band:** $4–$8  
**Bundle Path:** single challenge → STEM challenge series → makerspace bundle  
**Primary Grade Bands:** K–5  
**Style Tier:** Tier 1 Standard

#### Standard Outputs

1. Cover
2. Teacher guide
3. STEM vocabulary
4. Problem anchor
5. Plan page
6. Build/create page
7. Test and observe page
8. Improve/try again page
9. Compare designs page
10. STEM + SEL reflection
11. Exit ticket
12. Engineer certificate / take-home challenge

#### Required Design Rules

- Generous planning/drawing space
- Design process visual
- Clear success criteria
- Reflection on iteration and teamwork
- Grade-level writing expectations adjusted

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. STEM Challenge Pages
4. Use It Your Way / Design Process

---

### 4.13 Hygiene / Life Skills Mini-Pack

**Best For:** personal hygiene, handwashing, dental care, healthy habits, routines, self-care  
**Typical Page Count:** 10–12  
**Price Band:** $3–$6  
**Bundle Path:** single skill → healthy habits series → life skills bundle  
**Primary Grade Bands:** K–5  
**Style Tier:** Tier 1 Standard; sensitive topic review required

#### Standard Outputs

1. Cover
2. Teacher guide with dignity note
3. Vocabulary
4. Concept anchor
5. Step-by-step visual routine
6. Practice/sort page
7. Reflection/feelings page
8. Scenario page
9. Family connection
10. Affirmation/pride page
11. Exit ticket
12. Reminder card / take-home page

#### Required Design Rules

- Dignity-first language
- Body-positive, non-shaming visuals
- Sensitive topic pause required
- Clear routine icons
- Family connection should avoid assumptions about family structure

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Routine / Activity Pages
4. Use It Your Way / Home + Classroom Use

---

### 4.14 Bulletin Board / Classroom Decor Kit

**Best For:** seasonal displays, classroom culture, affirmations, student work displays, heritage displays  
**Typical Page Count:** 15–30 pieces  
**Price Band:** $5–$9  
**Bundle Path:** single display → seasonal classroom decor bundle → full-year decor bundle  
**Primary Grade Bands:** K–5  
**Style Tier:** Tier 1 Standard or Tier 2 for cultural/heritage displays

#### Standard Outputs

1. Cover
2. Teacher/setup guide
3. Bulletin board banner
4. Border trim options
5. Large title letters or posters
6. Student work headers
7. Themed accents/cutouts
8. Nameplates or editable-style labels
9. Quote posters
10. Black-and-white coloring versions when useful
11. Assembly guide

#### Required Design Rules

- Strong full-board mockup
- Pieces must be printable and cuttable
- Clear assembly instructions
- Large lettering must be readable from distance
- Include size notes when possible

#### Default 4 Listing Images

1. Cover / Full Board Mockup
2. What’s Included
3. Individual Pieces
4. Display Ideas / Use It Your Way

---

### 4.15 Task Cards / Centers Pack

**Best For:** review, centers, independent practice, stations, spiral review  
**Typical Page Count:** 24–48 cards plus guide/recording pages  
**Price Band:** $3–$7  
**Bundle Path:** skill pack → centers bundle → yearly review bundle  
**Primary Grade Bands:** K–5  
**Style Tier:** Tier 1 Standard

#### Standard Outputs

1. Cover
2. Teacher guide
3. Center sign
4. Task cards
5. Recording sheets
6. Answer key when applicable
7. Completion/self-assessment page
8. Storage labels when useful
9. Thank You / Credits / Terms page

#### Standard Page Types

- 4 cards per page
- numbered task cards
- recording sheet
- center sign
- answer key
- storage label

#### Required Design Rules

- Cards must be numbered
- Cut lines must be clear
- Visuals should not crowd the task text
- Answer key must match card numbers

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Sample Task Cards
4. Center Setup / Use It Your Way

---

### 4.16 Writing Craft + Keepsake Pack

**Best For:** family, special person, heritage, gratitude, peace day, teacher appreciation, community, publishing projects  
**Typical Page Count:** 6–12 or 8–16  
**Price Band:** $3–$5  
**Bundle Path:** single keepsake → holiday series → writing craft bundle  
**Primary Grade Bands:** K–5  
**Style Tier:** Tier 1 Standard or Tier 2 cultural/heritage

#### Standard Outputs

1. Cover
2. Teacher guide
3. Planning or interview page
4. Drafting/writing pages
5. Feature story or main message page
6. Memory/celebration/gratitude page
7. Publishing/final copy page
8. Craft or assembly page
9. Reflection/affirmation page
10. Certificate or keepsake page
11. Thank You / Credits / Terms page

#### Required Design Rules

- Inclusive family language
- Adapt writing space by grade band
- Provide drawing/illustration spaces
- Assembly instructions must be clear
- Keepsake pages should feel special and giftable

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Writing + Craft Pages
4. Finished Keepsake / Use It Your Way

---

### 4.17 Heritage Month / Tier 2 Ecosystem Pack

**Best For:** Juneteenth, Black History Month, Hispanic Heritage, AAPI Heritage, Indigenous Peoples Heritage, Women’s History, cultural celebration units  
**Typical Page Count:** 12+  
**Price Band:** $6–$10+ depending on depth  
**Bundle Path:** single heritage pack → heritage month bundle → cross-curricular ecosystem  
**Primary Grade Bands:** K–5, cross-grade variations possible  
**Style Tier:** Tier 2 Cultural / Heritage / Premium

#### Standard Outputs

1. Cover
2. Teacher guide with cultural note
3. Vocabulary
4. Historical/context page
5. Symbolism page
6. Reading/comprehension page
7. SEL/identity/pride page
8. Writing/creative response
9. Art/music/creative expression page
10. Cross-curricular activity
11. Family/community connection
12. Celebration/keepsake page
13. Thank You / Credits / Terms page
14. Listing images and preview PDF

#### Required Design Rules

- Cultural note required
- Sensitivity review required
- Avoid stereotypes or tokenized visuals
- Use rich themed style only when culturally appropriate
- Include joy, agency, pride, and accuracy
- Avoid trauma-only framing

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Cultural / Cross-Curricular Pages
4. Use It Your Way / Classroom Celebration

#### Tier 2 Badge Notes

Tier 2 badge text should be product-type specific. For science products, approved direction includes:

`CULTURALLY AFFIRMING SCIENCE PRACTICE`

Other Tier 2 product types require owner approval before locking badge text.

---

### 4.18 6–8 Cross-Curricular Mastery Pack

**Best For:** ELA, Social Studies, Science, integrated units, source analysis, project-based learning, middle school mastery work  
**Typical Page Count:** 14  
**Price Band:** $6–$10+  
**Bundle Path:** single unit → cross-curricular unit series → middle school mastery bundle  
**Primary Grade Bands:** 6–8  
**Style Tier:** Tier 1 Academic or Tier 2 Premium depending on topic

#### Standard Outputs

1. Cover
2. Teacher guide
3. Academic vocabulary
4. Background knowledge/context builder
5. Essential question page
6. Source/text/artifact analysis
7. Claim-evidence-reasoning page
8. SEL / identity / agency reflection
9. Cross-curricular connection
10. Evidence-based writing prompt
11. Project/performance task
12. Exit ticket/unit reflection
13. Concept map or organizer
14. Extension/reflection page

#### Required Design Rules

- More academic and professional visual style
- Minimal decoration
- Strong structure and generous response space
- Solid writing lines or open response boxes
- Emphasis on evidence, analysis, perspective, and synthesis

#### Default 4 Listing Images

1. Cover
2. What’s Included
3. Analysis + Writing Pages
4. Performance Task / Use It Your Way

---

## 5. Template Selection Rules

Agent 1C should select the product template using these rules.

| Opportunity Type | Recommended Template |
|---|---|
| Cutting, tracing, pre-writing, scissor skills | Fine Motor / Scissor Skills Pack |
| Sorting, sequencing, categorizing | Cut-and-Paste Sort Pack |
| Gratitude, special person, family, keepsake | Writing Craft + Keepsake Pack |
| Classroom game, vocabulary game, SEL bingo | Bingo / Interactive Game Pack |
| Simple reader, take-home book, decodable mini book | Emergent Reader / Mini Book Pack |
| Phonics pattern, word family, decoding | Phonics / Decodable Pack |
| Picture book companion, comprehension pack | Reading Mini-Pack |
| Emotions, friendship, identity, kindness | SEL Mini-Pack |
| Science concept, observation, experiment | Science Mini-Pack |
| Math skill, math centers, seasonal math | Math Mini-Pack or Math Centers Pack |
| Community, history, citizenship, maps | Social Studies Mini-Pack |
| STEM challenge, design/build/test | STEM / Hands-On Mini-Pack |
| Hygiene, routines, self-care | Hygiene / Life Skills Mini-Pack |
| Classroom display, decor, bulletin board | Bulletin Board / Classroom Decor Kit |
| Cards, stations, independent review | Task Cards / Centers Pack |
| Cultural/heritage cross-curricular unit | Heritage Month / Tier 2 Ecosystem Pack |
| Middle school integrated unit | 6–8 Cross-Curricular Mastery Pack |

If a product matches more than one template, Agent 1C should recommend a primary template and an optional secondary extension path.

Example:

- Hygiene picture sort → Primary: Cut-and-Paste Sort Pack; Extension: Hygiene / Life Skills Mini-Pack
- Juneteenth science activity → Primary: Science Mini-Pack; Style Tier: Tier 2 Heritage/Premium
- Peace Day writing craft → Primary: Writing Craft + Keepsake Pack; Secondary: SEL Mini-Pack

---

## 6. Variables Per Template

These are common variables that should appear in `product_config.json`.

### 6.1 Universal Variables

- product title
- subtitle
- product type template
- style tier
- target platform
- grade band
- theme token
- palette
- product code
- store name
- logo file path
- copyright line
- output folder
- answer key status
- sensitive topic flag
- cultural review flag

### 6.2 Content Variables

- skill focus
- standards alignment
- page count target
- teacher guide sections
- student page list
- directions text
- vocabulary list
- writing prompts
- answer key content
- differentiation notes
- extension ideas
- home connection note

### 6.3 Design Variables

- primary color
- secondary color
- accent color
- background color
- headline font
- body font
- border style
- icon set
- decorative asset set
- mockup style
- thumbnail/page assets
- completed sample style

### 6.4 Asset Variables

- asset library path
- asset index file
- required clipart
- universal icons needed
- section icons needed
- decorative assets needed
- background textures needed
- missing assets list

---

## 7. Fixed Engine Rules Per Template

These are engine-level rules that should not change per brand unless the platform changes.

| Rule | Fixed Value |
|---|---|
| TPT required listing image count | 4 |
| Listing image dimensions | 1200 × 1200 px |
| Printable page dimensions | 8.5 × 11 in |
| Printable raster page size | 2550 × 3300 px at 300 DPI |
| Preview PDF default | same 4 listing images in order |
| Buyer ZIP default | full product files only, not preview PDF |
| Student worksheet mode | black-and-white unless product requires color |
| Teacher/support pages | full color |
| Unicode symbol rule | draw icons/shapes or use assets; do not rely on Unicode stars/checkmarks/scissors |
| Thumbnail rule | contain, never crop or stretch |
| Asset rule | check asset index before generating new asset |
| Approval rule | owner approval before next stage |

---

## 8. Preview Layout Assignments

### 8.1 Universal 4-Image Logic

| Slot | Buyer Question Answered | Default Purpose |
|---|---|---|
| Image 1 | What is this? | Main cover / product identity |
| Image 2 | What do I get? | What’s included |
| Image 3 | What options/versions are included? | Versions, variants, cards, mats, levels, differentiated options |
| Image 4 | How can I use this? | Use It Your Way, workflow, classroom implementation |

### 8.2 Fine Motor / Scissor Skills Assignment

1. `01_Cover_1200x1200.png`
2. `02_Whats_Included_1200x1200.png`
3. `03_Right_Left_Versions_1200x1200.png`
4. `04_Use_It_Your_Way_1200x1200.png`

### 8.3 Optional Bonus Assets

Some products may generate extra marketing images beyond the required 4 TPT thumbnails.

Examples:

- How to Use square graphic
- Pinterest pin
- Etsy extra listing image
- Instagram square post
- video preview storyboard frame

These are optional bonus assets and are not part of the locked 4-image TPT system unless explicitly approved.

---

## 9. Teacher Page Assignments

### 9.1 Universal Teacher/Support Pages

Most products should include some or all of these pages:

1. Teacher Guide
2. How to Use
3. Skill Progression or Implementation Guide
4. Thank You / Credits / Terms

### 9.2 Product-Type Teacher Page Map

| Product Type | Required Teacher/Support Pages |
|---|---|
| Fine Motor / Scissor Skills | Teacher Guide, How to Use, Skill Progression, Thank You / Credits / Terms |
| Cut-and-Paste Sorts | Teacher Guide, How to Use, Answer Key/Sample Sort, Thank You / Credits / Terms |
| Coloring + Writing Craft | Teacher Guide, Assembly/Display Ideas, Thank You / Credits / Terms |
| Bingo / Game Pack | Teacher Guide, How to Play, Variations, Thank You / Credits / Terms |
| Emergent Reader | Teacher Guide, Assembly Instructions, Reading Tips, Thank You / Credits / Terms |
| Phonics / Decodable | Teacher Guide, Skill Notes, Answer Key if needed, Thank You / Credits / Terms |
| Reading Mini-Pack | Teacher Guide, Pacing Guide, Answer Key if applicable, Thank You / Credits / Terms |
| SEL Mini-Pack | Teacher Guide with Dignity/Trauma-Informed Note, How to Use, Thank You / Credits / Terms |
| Science Mini-Pack | Teacher Guide, Materials/Setup Notes, Safety Note if needed, Thank You / Credits / Terms |
| Math Mini-Pack | Teacher Guide, Answer Key, Differentiation Notes, Thank You / Credits / Terms |
| Social Studies | Teacher Guide, Cultural/Sensitivity Note if needed, Thank You / Credits / Terms |
| STEM / Hands-On | Teacher Guide, Materials/Setup, Safety/Management Notes, Thank You / Credits / Terms |
| Hygiene / Life Skills | Teacher Guide with Dignity Note, Family Connection Note, Thank You / Credits / Terms |
| Bulletin Board Kit | Setup Guide, Assembly Ideas, Printing Tips, Thank You / Credits / Terms |
| Task Cards / Centers | Teacher Guide, Center Setup, Answer Key, Storage Tips, Thank You / Credits / Terms |
| Heritage / Tier 2 Ecosystem | Teacher Guide with Cultural Note, Sensitivity Note, Thank You / Credits / Terms |
| 6–8 Cross-Curricular | Teacher Guide, Implementation Tips, Standards, Rubric/Answer Key if applicable |

---

## 10. Notes for Future Expansion

### 10.1 Add Template Specs as the System Proves Itself

This library should grow only when a new product type is used at least once or clearly belongs in the roadmap.

Avoid over-building templates before the first 5–10 products prove which structures are actually useful.

### 10.2 Build Product-Type Templates Before Theme Templates

Do not create a separate template for every season or holiday.

Use product-type templates first, then apply theme tokens.

Correct model:

`Product Type Template + Theme Token + Grade Band + Asset Pack = Product Build`

Example:

`Fine Motor / Scissor Skills + Winter + PreK-K + Winter Clipart = Winter Scissor Skills Pack`

### 10.3 Use the Asset Library to Reduce Cost

Every product build should check the asset index before generating new art.

If an asset is generated during production, it should be saved to the asset library using the correct naming convention and logged in `asset_index.json`.

### 10.4 Track Metrics by Template Family

Mira should log:

- product type used
- time to create build packet
- time to render files
- number of revisions
- assets reused
- assets newly generated
- quality issues
- upload readiness
- estimated manual time saved

This data helps prove which templates are fastest, cheapest, and most profitable.

### 10.5 Future Productization

When SSP becomes a sellable system, this library can become part of the user-facing setup:

- buyer chooses product type
- buyer chooses grade band
- buyer chooses theme
- buyer uploads logo/brand colors
- system generates product config
- system produces build packet and output files

This document is therefore both a production reference and an early productization asset.

---

## Appendix A — Suggested First 5 Template Families to Prove

These should be prioritized before expanding the full library.

1. Fine Motor / Scissor Skills Pack
2. Cut-and-Paste Sort Pack
3. Coloring + Writing Craft Pack
4. Bingo / Interactive Game Pack
5. Mini Unit / Teacher-Supported Pack

These families are reusable, high-volume, and likely to support the first scalable product catalog.

---

## Appendix B — Deprecated / Removed From Raw Draft

The raw draft contained repeated sections, chat continuation prompts, and duplicate template descriptions. These were removed or consolidated.

Removed:

- “Would you like me to continue...” chat residue
- repeated Writing Craft + Keepsake duplicate sections
- duplicate global rules repeated under every template
- unsupported “all templates ready for production” language
- unnecessary repeated character representation blocks

Consolidated:

- reading mini-pack grade variations
- science K–2 and 3–5 versions
- writing craft and keepsake versions
- SEL mini-pack structures
- task card and centers references

---

**End of Document**
