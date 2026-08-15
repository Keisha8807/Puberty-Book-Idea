# SSP — Brand Variable vs Engine Rule Tracker
**Purpose:** Every decision made while building your 20 products gets logged here.
Brand Variables = what buyers customize during setup.
Engine Rules = what stays identical for every user of the system.
**Update this during every build session.**

---

## HOW TO USE THIS

When you make any decision during production, ask:
- Would another seller's brand need a DIFFERENT answer here? → Brand Variable
- Would every seller using this system follow the SAME rule? → Engine Rule

Log it below. By product 20 you have your productization blueprint.

---

## BRAND VARIABLES
*These become fields in the Brand Setup Wizard when you sell the system.*

| # | Decision | SSP Value | Sellable Version |
|---|----------|-----------|-----------------|
| BV-01 | Store name | Sunray Story Press | [Buyer inputs their store name] |
| BV-02 | Primary color | #E8821A (Fall Orange) | [Buyer inputs hex code or uses color picker] |
| BV-03 | Secondary color | #4A8C3F (Fall Green) | [Buyer inputs hex code] |
| BV-04 | Accent color | #5C3317 (Fall Brown) | [Buyer inputs hex code] |
| BV-05 | Background color | #FFF7E8 (Cream) | [Buyer inputs hex code] |
| BV-06 | Headline font | Fredoka One | [Buyer selects from approved free commercial use font list] |
| BV-07 | Body font | Nunito | [Buyer selects from approved list] |
| BV-08 | Logo file | SSP sun logo PNG | [Buyer uploads transparent PNG] |
| BV-09 | Primary platform | TPT | [Buyer selects TPT / Etsy / TES / all three] |
| BV-10 | Product niche | K-5 culturally affirming educational resources | [Buyer defines their niche] |
| BV-11 | Grade levels served | PreK through Grade 5 | [Buyer selects grade range] |
| BV-12 | Product type focus | Writing crafts, coloring, science, fine motor, SEL | [Buyer selects their product categories] |
| BV-13 | Seasonal palette set | Fall/Winter/Spring/Summer locked hex sets | [Buyer approves or customizes seasonal palettes] |
| BV-14 | Tier 2 cultural focus | Juneteenth, Black History Month, heritage months | [Buyer defines their Tier 2 products if any] |
| BV-15 | Copyright line text | © Sunray Story Press | [Buyer inputs their store name] |
| BV-16 | TPT store URL | teacherspayteachers.com/Store/Sunray-Story-Press | [Buyer inputs their store URL] |
| BV-17 | Product code prefix | SSP | [Buyer inputs their 2-3 letter prefix] |
| BV-18 | Target audience niche | Diverse, inclusive, culturally affirming focus | [Buyer defines their audience angle] |
| BV-19 | Pricing philosophy | Mid-range $5-6, premium Tier 2 $6-10 | [Buyer defines their price points] |
| BV-20 | Agent team names | Sunny, Scout, Cora, Dani, Sophie, Penny, Parker, Quinn, Rex | [Buyer can rename or keep defaults] |

*Add new rows as you make brand-specific decisions during your 20-product build.*

---

## ENGINE RULES
*These stay identical for every user of the system. Never modified during Brand Setup.*

| # | Rule | Value | Why It's Fixed |
|---|------|-------|---------------|
| ER-01 | Number of listing images | Exactly 4 | TPT supports 4 thumbnail slots — this is platform logic |
| ER-02 | Listing image slot 1 | Main Listing Image — answers "what is this" | Buyer conversion logic — universal |
| ER-03 | Listing image slot 2 | What's Included — answers "what do I get" | Buyer conversion logic — universal |
| ER-04 | Listing image slot 3 | Options/Versions — answers "what are my choices" | Buyer conversion logic — universal |
| ER-05 | Listing image slot 4 | Use It Your Way — answers "how do I use this" | Buyer conversion logic — universal |
| ER-06 | Listing image dimensions | Exactly 1200x1200px PNG | TPT specification |
| ER-07 | Printable page dimensions | 8.5x11 inches, 300 DPI | Print standard |
| ER-08 | Student page color mode | Black and white, ink-friendly | Classroom printing reality |
| ER-09 | Teacher/cover page color mode | Full color | Visual quality standard |
| ER-10 | Production order | Worksheets → colored versions → completed sample → teacher pages → support pages → listing images → preview PDF → product PDF → ZIP | Dependency logic — cannot be reordered |
| ER-11 | Preview PDF contents | Same 4 listing images compiled in order | TPT preview field specification |
| ER-12 | Preview PDF placement | Uploaded to preview field only — not in buyer ZIP | TPT platform rule |
| ER-13 | Buyer ZIP contents | Full product files only — not preview PDF | Clean separation of preview vs product |
| ER-14 | Unicode symbol prohibition | Never use ★ ✂ ✓ as design elements — draw shapes | Rendering reliability across all systems |
| ER-15 | Thumbnail scaling rule | Object-fit contain — never crop or stretch | Visual accuracy standard |
| ER-16 | Thumbnail consistency | All thumbnails same displayed size within one listing image | Visual professionalism standard |
| ER-17 | Logo presence | Present on every page and listing image | Brand protection |
| ER-18 | Copyright line | Present on every page | Legal protection |
| ER-19 | Empty page space rule | No empty white space in lower 30% of any teacher page | Quality standard |
| ER-20 | Sensitive topic flag | Any product touching hygiene, puberty, body safety, SEL, family structure must pause for owner routing | Brand protection — universal |
| ER-21 | Approval mode | Agents prepare, owner approves, nothing goes live without sign-off | Business protection — universal |
| ER-22 | Asset index check first | Always check asset_index.json before generating — pull existing, generate only if missing | Credit/cost conservation |
| ER-23 | File naming convention | theme_subject_style_colormode_sizepx.ext | System readability |
| ER-24 | Buyer ZIP naming | StoreName_ProductName_GradeLevel.zip | Platform professionalism |
| ER-25 | Batch approval structure | Batch A (worksheets) → Batch B (teacher pages) → Batch C (listing images) | Quality gate logic |
| ER-26 | Answer key rule | Never claim answer key unless one actually exists in the product | Platform accuracy rule |
| ER-27 | Video preview max | 5 minutes | TPT specification |
| ER-28 | TPT format tags max | 3 as of spring 2025 | TPT specification |
| ER-29 | TPT theme/audience/language tags max | 6 as of spring 2025 | TPT specification |
| ER-30 | Grade targeting | Max 4 grade levels per product for clear buyer targeting | TPT best practice |
| ER-31 | Combined final support page | Thank You, Credits, and Terms of Use are always one final support page, not two separate pages | Universal page-count, QA, and product packaging rule |

*Add new rows as you identify universal rules during your 20-product build.*

---

## DECISIONS STILL PENDING
*Log decisions you haven't made yet so nothing falls through.*

| # | Decision Needed | Blocking What | Target Date |
|---|----------------|---------------|-------------|
| PD-01 | Tier 2 corner badge text for Use It Your Way listing image | Tier 2 Batch C production | When first Tier 2 product reaches Batch C |
| PD-02 | Commercial clipart library sources and licenses | Asset license tracker | Before sourcing any non-AI assets |
| PD-03 | Quinn terms verification for combined Thank You / Credits / Terms page | Final support page QA gate | Before any product is marked ready_for_publish |

---

## PRODUCTIZATION READINESS SCORE
*Track this as you build. Update after each product.*

| Milestone | Status |
|-----------|--------|
| Brand variables fully identified | 20 listed, adding as discovered |
| Engine rules fully documented | 31 listed, adding as discovered |
| 5 products built using the system | ⬜ |
| 10 products built — patterns confirmed | ⬜ |
| 20 products built — system proven | ⬜ |
| Brand Setup Wizard designed | ⬜ |
| Brand-agnostic version of all docs drafted | ⬜ |
| Python renderer tested by someone else | ⬜ |
| First beta tester runs it successfully | ⬜ |
| Sellable package assembled | ⬜ |

---

*Last updated: May 2026 | Add a row every time you make a decision during production*
