# SSP START HERE + CURRENT STATE HANDOFF
**Condensed active Project file.** This file combines related SSP control documents so the ChatGPT Project stays under file-count limits while preserving operating rules.

## Purpose
First file to read in the Project. Establishes the current state, locked rules, product focus, and how to navigate the rest of the binder.

## Binder Notes / Locked Decisions
Read this before opening any other SSP file. If a rule conflicts, the newest correction log and locked visual standards take precedence.

## Source Documents Included
- `SSP_Start_Here_Handoff.md`
- `SSP_Correction_Change_Log.md`

---

# SOURCE: SSP_Start_Here_Handoff.md

# SSP START HERE — CURRENT STATE HANDOFF
## Read this entire document before accessing any other file. Do not begin work until you have read everything here.

---

## WHO WE ARE

**Sunray Story Press (SSP)** is a culturally inclusive, affirming K–5 educational publishing brand. We create printable and digital resources for teachers, homeschool families, and classroom communities. Products are sold primarily on TPT (Teachers Pay Teachers), with Etsy being set up and TES planned for future expansion.

**Owner:** Solo creator with ADHD. All work is structured around sequential execution, clear batch approvals, external scaffolding, and minimal context-switching. Do not present multiple open-ended options simultaneously. Do not ask "what would you like to do next?" — present one clear next step with a defined approval gate.

**Brand values:** Inclusive representation · Joyful learning · Teacher-friendly · Low-prep · Culturally affirming · Not tokenized

---

## SISTER BRANDS — KEEP SEPARATE

These brands share an owner but are entirely separate projects. Never mix their content, aesthetics, or assets into SSP work.

- **Truth & Treasure Co.** — Faith and healing content (devotionals, grief planners, Bible journals)
- **Chapel Couture** — Editorial luxury faith aesthetic (spoken word, social media, content brand)

If a session accidentally contains work from these brands, stop and clarify before proceeding.

---

## WHAT THE PIPELINE DOES

We are building a fully autonomous AI production pipeline for SSP. The pipeline:

1. Receives a product idea
2. Produces an intelligent Product Brief for owner approval
3. Generates all product content, images, teacher pages, and support pages
4. Assembles 4 listing images at 1200x1200px and a preview PDF
5. Assembles the full buyer download PDF
6. Produces listing copy for TPT, Etsy, and TES
7. Packages everything into a ZIP ready for upload
8. Holds everything in **Approval Mode** — owner approves before anything goes live

**Key tools in the system:**
- Manus — autonomous production execution
- Claude Project — strategy, document creation, design decisions
- ChatGPT — scheduled daily briefs and TPT store audits
- Google Drive — asset library master storage
- Telegram — mobile interface to agents

**System reads from:**
- `product_config.json` — per-product configuration and pipeline status
- `asset_index.json` — master library of all available assets
- All uploaded SSP Project Knowledge files

**System outputs:**
- Printable PDFs at 8.5×11, 300 DPI
- Preview listing images at exactly 1200×1200px PNG
- Preview sample PDF (4 listing images compiled)
- Buyer download ZIP with correct naming convention
- Platform-specific listing copy

---

## AGENT TEAM ROSTER

All agents operate in **Approval Mode**. Agents prepare. Owner approves. Nothing goes live without explicit owner sign-off.

| Agent | Role |
|-------|------|
| **Sunny** | Chief of Staff — daily briefing, bottleneck map, brain dump sorter |
| **Scout** | Product research, trend analysis, keyword research, Product Brief |
| **Cora** | Curriculum content writer — student pages, teacher guides |
| **Dani** | Design and prompt director — image generation, preview image planning |
| **Sophie** | SEO listing copywriter — brand voice guide, content repurposing |
| **Penny** | Pricing and offer strategist |
| **Parker** | Cross-posting and platform ops — asset library sync |
| **Quinn** | Quality control — QA reports, sensitive topic review |
| **Rex** | Content repurposing engine (SSP product content only) |

**Trigger phrase:** Say **"Sunny, brief me"** to activate the daily standup summary.

---

## LOCKED SYSTEM RULES

### Production Order — Mandatory, Cannot Be Reordered

1. Generate blank B&W student worksheets
2. Generate colored versions for marketing use
3. Generate completed student sample with grade-appropriate rendering
4. Generate teacher pages
5. Generate support pages (thank you, terms of use)
6. Build 4 listing images using real worksheet files from steps 1–3
7. Assemble preview PDF from 4 listing images
8. Assemble full product PDF (cover → teacher pages → worksheets → support pages)
9. Run thumbnail contrast check at 100×100px
10. Package buyer ZIP

### Fonts — Locked

- **Fredoka One** — headlines, badge titles, cover titles (Google Fonts, commercial use confirmed)
- **Nunito** — body text, card content, teacher page text (Google Fonts, commercial use confirmed)

No other fonts may be used in any SSP product without explicit owner approval.

### Brand Palette — Locked

| Name | Hex |
|------|-----|
| Sunray Yellow | `#F7C948` |
| Sky Blue | `#4DA9E9` |
| Coral | `#FF7A6E` |
| Sage | `#A8C3A0` |
| Navy | `#1F2A44` |
| Cream | `#FFF7E8` |

### Seasonal Palettes — Locked

| Season | Color 1 | Color 2 | Color 3 | Background |
|--------|---------|---------|---------|------------|
| Fall | `#E8821A` | `#4A8C3F` | `#5C3317` | `#FFF7E8` |
| Winter | `#1F2A44` | `#C9D1D9` | `#9B1C2C` | `#F8F9FA` |
| Spring | `#C8A2C8` | `#A8D8B9` | `#FFC1A1` | `#FFFEF0` |
| Summer | `#008080` | `#F7C948` | `#FF7A6E` | `#FFF5E0` |

### Style Tiers

- **Tier 1 Standard:** 80% of products — seasonal, skill-based, evergreen. Clean cream backgrounds, structured layouts, subtle seasonal accents.
- **Tier 2 Cultural Heritage Premium:** Juneteenth, Black History Month, heritage months — rich themed borders, custom illustrated covers, Cultural Note section, premium pricing. Requires owner confirmation before any cultural pattern elements are generated.

### Preview Listing Images

- Exactly **4 per product** at **1200×1200px**
- Never more, never fewer for standard products
- Universal slot names (permanent, content adapts per product type):
  - `01_Main_Listing_Image_1200x1200.png`
  - `02_Whats_Included_1200x1200.png`
  - `03_Options_Versions_1200x1200.png`
  - `04_Use_It_Your_Way_1200x1200.png`
- Deprecated names (do not use): ~~04_Skill_Progression_1200x1200.png~~ / ~~04_Closeup_Student_Pages_1200x1200.png~~

### Asset Rules

1. Check `asset_index.json` before generating anything
2. If asset exists in the index → pull it
3. If asset does not exist → generate it using the standard clipart prompt template, save to the correct library folder, update the index
4. Never generate a duplicate of an existing asset without flagging it

### Symbol Rendering Rule

**Never** use unicode symbols (★ ✂ ✓ • etc.) for visual design elements. Draw shapes programmatically or use PNG/SVG icon assets from the library.

### Sensitive Topic Flag

Any product touching hygiene, puberty, body safety, SEL, family structure, or identity **must pause and route to owner** before any content or images are generated.

---

## CURRENT PIPELINE STATUS

*This section must be updated at the end of each session. Agents read this to know what is in progress and what stage each product is at.*

### Products Currently In Production

| Product Code | Product Title | Grade | Status | Current Stage |
|-------------|--------------|-------|--------|--------------|
| SSP-JK-001 | Juneteenth Science Pack | K | Live | Complete |
| SSP-J1-001 | Juneteenth Science Pack | Gr. 1 | Live | Complete |
| SSP-J2-001 | Juneteenth Science Pack | Gr. 2 | In Progress | Review |
| SSP-J3-001 | Juneteenth Science Pack | Gr. 3 | In Progress | Review |
| SSP-J4-001 | Juneteenth Science Pack | Gr. 4 | In Progress | Review |
| SSP-J5-001 | Juneteenth Science Pack | Gr. 5 | In Progress | Review |
| SSP-JB-001 | Juneteenth Science Bundle | K–5 | Planned | Awaiting individual products |
| SSP-LT-001 | The Love & Thanks Times (Sp. Ed., Gr. 3–5) | 3–5 | In Progress | Preview pages |
| SSP-MG-001 | Mom's Day Gazette | K–2 | In Progress | Review |

### Session Focus

This session: **Document Build** — creating the 25 control layer documents that all agents and the production engine read from. No code or images are generated until all Priority 1 and Priority 2 documents are complete.

---

## WHAT NOT TO DO

The following actions are prohibited in every SSP session without explicit owner override:

- **Never publish or upload anything** to TPT, Etsy, or TES — even if it's ready. Owner executes all uploads manually.
- **Never invent assets** — if an asset doesn't exist in the library, flag it and follow the Asset Request Decision Tree. Do not generate a substitute silently.
- **Never fabricate competitor data** — Scout pulls real research only. Never invent prices, review counts, or product titles.
- **Never generate content for sensitive topics** without routing to owner first — this includes any product touching hygiene, puberty, body safety, SEL, family structure, or identity.
- **Never use a font other than Fredoka One or Nunito** without explicit owner approval.
- **Never use unicode symbols** as visual design elements — draw shapes programmatically.
- **Never crop or stretch worksheet thumbnails** in listing images — always use object-fit contain.
- **Never overwrite existing library files** — use `_deprecated` suffix before saving a replacement.
- **Never proceed past a stop rule** — if a stop rule triggers, document what happened and present it to the owner before continuing.
- **Never ship a product with empty space in the lower 30% of any teacher page** — fill space before marking batch complete.

---

## DOCUMENT LIBRARY INDEX

*Reference list of all SSP control documents. Agents check this to locate the document they need.*

| Doc # | File Name | Purpose |
|-------|-----------|---------|
| 01 | SSP_Start_Here_Handoff.md | This file — session orientation |
| 02 | SSP_Product_JSON_Config_Template.json | Per-product configuration template |
| 03 | SSP_Preview_Manifest_Template.md | Listing image layout rules by product type |
| 04 | SSP_Asset_Index_Template.json | Asset library schema and sample entries |
| 05 | SSP_Batch_Approval_Rubric.md | Exact criteria for approving each production batch |
| 06 | SSP_Teacher_Page_Style_Tier_Map.md | Visual treatment rules by product tier |
| 07 | SSP_Teacher_Page_Layout_Template_Bank.md | Layout specs for all 5 teacher/support page types |
| 08 | SSP_Preview_Image_Copy_Map.md | What each of the 4 listing images must communicate |
| 09 | SSP_Product_Assembly_Manifest.md | Exact page order for buyer PDF and preview PDF |
| 10 | SSP_Asset_Request_Decision_Tree.md | Step-by-step process when an agent needs an asset |
| 11 | SSP_Asset_Quality_Standards.md | Minimum technical/visual requirements for library assets |
| 12 | SSP_Asset_Naming_Convention.md | Permanent naming rules for all library assets |
| 13 | SSP_TPT_Upload_Field_Map.md | Every TPT listing field with specs |
| 14 | SSP_Platform_Compliance_Checklist.md | Pre-upload verification by platform |
| 15 | SSP_Credit_Budget_Stop_Rules.md | Credit cost estimates and stop rules |
| 16 | SSP_Error_Debug_Protocol.md | Known failure modes and resolution steps |
| 17 | SSP_Design_QA_Checklist.md | Quinn's comprehensive visual QA checklist |
| 18 | SSP_SEO_Research_Evidence_Log.md | Scout's keyword research and competitor evidence log |
| 19 | SSP_Product_Family_Bundle_Logic_Map.md | Product families, expansion paths, bundle logic |
| 20 | SSP_Evergreen_100_Product_Slate.md | Strategic 100-product catalog plan |
| 21 | SSP_Asset_Library_Folder_Structure.md | Google Drive folder tree for asset library |
| 22 | SSP_Asset_License_Source_Tracker.md | Source and license tracking for all non-SSP assets |
| 23 | SSP_Product_Brief_Template.md | Scout's pre-production brief template |
| 24 | SSP_Mockup_Assignment_Map.md | Mockup style assignments by product type and page |
| 25 | SSP_Clipart_Generation_Prompt_Template.md | Standardized clipart prompt format |

---

*Last updated: May 2026 | Sunray Story Press | Owner approval required before any product goes live*

---

# SOURCE: SSP_Correction_Change_Log.md

# SSP DOCUMENT CORRECTION CHANGE LOG
## Applied: May 2026 — Pre-Priority 3 batch corrections
## Status: All 10 fixes and 5 final decisions applied. Ready for owner confirmation.

---

| Document | Section changed | Fix # applied | What was changed |
|----------|----------------|---------------|-----------------|
| SSP_Visual_Standards_Analysis_LOCKED.md | File rename | Fix 7 | Renamed from SSP_Visual_Standards_Analysis.md to SSP_Visual_Standards_Analysis_LOCKED.md. All documents updated to reference new filename. |
| SSP_Visual_Standards_Analysis_LOCKED.md | File header | Fix 7 | Internal `## File:` line updated to reflect new filename. |
| SSP_Visual_Standards_Analysis_LOCKED.md | Open Items table | D (OI-01, OI-03) | OI-01 closed: Skill Progression no longer a listing image slot; Tier 2 badge to be defined at first Tier 2 scissor skills Batch C. OI-03 closed: 5th "How to Use" image is optional bonus marketing asset only, not a replacement for any locked slot. OI-02 and OI-04 remain open. |
| SSP_Visual_Standards_Analysis_LOCKED.md | Page Structure by Page Number section | Fix 1, D (OI-01, OI-03) | Entire section replaced with "Universal 4-Image Slot Structure — LOCKED" table. Old Page 1–4 structure removed. Universal slot names, file names, content-by-product-type table, deprecated names, Skill Progression rule, and 5th image rule all documented. |
| SSP_Start_Here_Handoff.md | Pipeline status table | Fix 10 | SSP-MD-001 renamed to SSP-LT-001 (Love & Thanks Times family code = LT). SSP-MDK-001 renamed to SSP-MG-001 (Mom's Day Gazette family code = MG). |
| SSP_Start_Here_Handoff.md | Preview Listing Images section (Locked System Rules) | Fix 1 | Old single file name reference replaced with full universal 4-slot names list. Deprecated names marked. |
| SSP_Product_JSON_Config_Template.json | Full document | Fix 1, 2, 3, 4, 5 | Full rewrite. Changes: (1) listing_images section rebuilt with universal slot names (slot_01 through slot_04), deprecated names noted, Skill Progression and 5th image rules documented; (2) tpt_listing tags section restructured — removed "_tag_limit: 20 tags maximum," added format_tags (max 3), theme_audience_language_tags (max 6), note that grade/subject/resource type are separate upload fields, grade level max 4 recommended; (3) grade_level field updated with PreK, PreK-K, PreK-1, K-1 valid values, prek_k_blend rendering style added; (4) preview_pdf nested under assets with rule "TPT preview field only, NOT in buyer ZIP, 5MB max," video preview time limit 5 minutes noted; (5) asset rights schema updated — removed source: ai_generated_ssp with auto commercial_use_confirmed: true, added source_tool / rights_status / license_notes fields to assets block, commercial_use_confirmed removed from auto-confirm. Schema version bumped to 1.1. |
| SSP_Preview_Manifest_Template.md | Full document | Fix 1, D (OI-03), Skill Progression | Full rewrite. Changes: Universal 4-slot system table at top. Deprecated names listed. Skill Progression rule documented. 5th image rule documented (OI-03 closed). All 4 slot layout specs rewritten using universal slot names (Slot 01 Main Listing Image, Slot 02 What's Included, Slot 03 Options/Versions, Slot 04 Use It Your Way). Slot 03 content-by-product-type table added with locked badge text per product type. Slot 04 workflow content confirmed (Color→Cut→Glue for scissor skills, assembly for writing craft). Product Type Slot Assignment Table added. Preview PDF 5MB limit and "not in buyer ZIP" rule documented. |
| SSP_Asset_Index_Template.json | Full document | Fix 5, Fix 6 | Full rewrite. Changes: (5) Rights schema corrected — all asset entries now require source_tool (ChatGPT/Manus/Gemini/commercial_library/owner_created), rights_status (pending_verification/confirmed/restricted/rejected), license_notes (blank field for Quinn), commercial_use_confirmed defaults to false. Old "source: ai_generated_ssp" with auto true removed. Schema definitions updated. (6) All 5 sample entries marked status: example_only and commercial_use_confirmed: false. Critical rule added at top: example_only entries are never used to resolve production asset lookups. Schema version bumped to 1.1. |
| SSP_Batch_Approval_Rubric.md | Header reference | Fix 7 | SSP_Visual_Standards_Analysis.md → SSP_Visual_Standards_Analysis_LOCKED.md |
| SSP_Batch_Approval_Rubric.md | Entire Batch C section (C0–C5) | Fix 1, Badge fix (C3-03) | C0-03: File naming updated to universal slot names. C0-14 added: deprecated names must be absent. C1 section renamed from "Listing Image 1 — Cover/Hero" to "Slot 01 — Main Listing Image," rubric items updated to be product-type neutral. C2 section renamed "Slot 02 — What's Included," items updated. C3 section replaced: renamed "Slot 03 — Options/Versions," 5 items rewritten. C3-03 specifically: OLD was "'ONE PURCHASE SUPPORTS BOTH' circular badge present" → NEW is "For scissor skills: main badge reads 'RIGHT + LEFT VERSIONS INCLUDED' (locked phrase). 'ONE PURCHASE SUPPORTS BOTH' is NOT the standard badge." C4 section replaced: renamed "Slot 04 — Use It Your Way," 5 items rewritten including C4-05 which explicitly fails any Skill Progression grid appearing as primary slot 04 content. C5 updated: page order uses slot names, C5-06 (5MB max) added, C5-07 (not in buyer ZIP) added. |
| SSP_Teacher_Page_Style_Tier_Map.md | Header | Fix 7 | SSP_Visual_Standards_Analysis.md → SSP_Visual_Standards_Analysis_LOCKED.md |
| SSP_Teacher_Page_Style_Tier_Map.md | Cross-reference table | Fix 7 | SSP_Visual_Standards_Analysis.md → SSP_Visual_Standards_Analysis_LOCKED.md |
| SSP_Teacher_Page_Layout_Template_Bank.md | Header | Fix 7 | Added reference to SSP_Visual_Standards_Analysis_LOCKED.md |
| SSP_Preview_Image_Copy_Map.md | Full document | Fix 1, D (OI-01, OI-03) | Full rewrite. Changes: Universal 4-slot names throughout. Deprecated names documented. Skill Progression removed as listing slot — noted as feature badge option in Slot 02 only. OI-01 closed (Slot 04 badge to be defined at first Tier 2 Batch C). OI-03 closed (5th image is optional marketing asset). Slot 03 section updated with locked badge text table: scissor skills = "RIGHT + LEFT VERSIONS INCLUDED" (locked). Badge clarification added: "ONE PURCHASE SUPPORTS BOTH" is NOT the locked primary phrase. Slot 04 confirmed as Use It Your Way — not Skill Progression. Product type copy adaptation table updated for all 4 slots. What Never Appears list updated: Skill Progression as primary slot 04 content and "ONE PURCHASE SUPPORTS BOTH" as primary badge both added as prohibited. |
| SSP_Product_Assembly_Manifest.md | Preview PDF section | Fix 1, Fix 4 | File names updated to universal slot names (01_Main_Listing_Image through 04_Use_It_Your_Way). Rule added: "Preview PDF uploaded to TPT preview field only. NOT included in buyer download ZIP." |
| SSP_Product_Assembly_Manifest.md | Buyer ZIP contents section | Fix 4 | Section rewritten: preview PDF explicitly excluded from ZIP contents. Listing image table updated with universal slot names. Preview PDF row updated: "TPT preview file field only — NOT in buyer ZIP." |
| SSP_Product_Assembly_Manifest.md | Assembly checklist | Fix 1, Fix 4 | Checklist updated: "Listing image slot 02 count badge" (was "listing image 2"). New checks added: Preview PDF under 5MB; Preview PDF NOT in buyer ZIP. Universal slot names used throughout. |
| SSP_Asset_Request_Decision_Tree.md | Step 5b — After successful generation | Fix 5 | Removed: `source: ai_generated_ssp` and `commercial_use_confirmed: true (SSP-generated assets are owned by SSP)`. Added: `source_tool: [tool used]`, `rights_status: pending_verification`, `license_notes: [blank — Quinn completes]`, `commercial_use_confirmed: false`. Critical rights rule paragraph added: AI-generated assets not automatically confirmed for commercial use; Quinn must verify before ready_for_publish. |
| SSP_Asset_Quality_Standards.md | No change needed | Fix 7 | No references to old VSA filename found in this document. No changes required. |
| SSP_Asset_Naming_Convention.md | No change needed | Fix 7 | No references to old VSA filename found in this document. No changes required. |

---

## FIX STATUS SUMMARY

| Fix # | Description | Status |
|-------|-------------|--------|
| Fix 1 | Universal slot names throughout all documents | APPLIED — 8 documents updated |
| Fix 2 | TPT section-based tag logic (not universal 20-tag limit) | APPLIED — Product Config JSON rewritten |
| Fix 3 | PreK grade levels and prek_k_blend rendering style | APPLIED — Product Config JSON rewritten |
| Fix 4 | Preview PDF to TPT field only, not in buyer ZIP, 5MB max | APPLIED — Product Config JSON, Preview Manifest, Assembly Manifest updated |
| Fix 5 | AI asset rights schema corrected (source_tool, rights_status, license_notes, commercial_use_confirmed: false default) | APPLIED — Asset Index, Asset Request Decision Tree updated |
| Fix 6 | Asset Index sample entries marked status: example_only | APPLIED — Asset Index rewritten |
| Fix 7 | VSA renamed to LOCKED; all references updated | APPLIED — File renamed; 5 documents updated |
| Fix 8 | TPT Upload Field Map prep requirements for Doc 13 | NOTED — Requirements documented in owner's correction message; will be applied when Doc 13 is built in Priority 3. No Priority 1–2 changes required. |
| Fix 9 | Video preview 5 minutes maximum | APPLIED — Noted in Product Config JSON preview_pdf block. No Priority 1–2 docs referenced video preview time limits. Will be applied explicitly in Doc 13. |
| Fix 10 | Product family codes: LT for Love & Thanks Times, MG for Mom's Day Gazette | APPLIED — Start Here Handoff pipeline table updated |

## DECISION STATUS SUMMARY

| Decision | Status |
|----------|--------|
| Universal 4-image slot names (D-slot) | APPLIED — All documents updated |
| Skill Progression to teacher pages only | APPLIED — Removed from listing image slots in all documents |
| Badge text for Slot 03: RIGHT + LEFT VERSIONS INCLUDED (locked for scissor skills) | APPLIED — Rubric C3-03, Copy Map, Preview Manifest all updated |
| OI-01 closed | APPLIED — VSA, Copy Map updated |
| OI-03 closed | APPLIED — VSA, Preview Manifest, Copy Map, Product Config updated |

## OPEN ITEMS REMAINING

| # | Item | Status |
|---|------|--------|
| OI-02 | Non-Juneteenth Tier 2 heritage pattern approval process | Still open — no owner input yet |
| OI-04 | Quinn terms verification for Tier 2 combined Thank You + Terms page | Still open — Quinn action required before first Tier 2 ready_for_publish clearance |

---

*Change log produced: May 2026 | Awaiting owner confirmation before Priority 3 begins | Sunray Story Press*

---

