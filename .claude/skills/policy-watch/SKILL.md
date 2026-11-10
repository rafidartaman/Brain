---
name: policy-watch
description: Use monthly, before any one-way decision that depends on an Indonesian rule, or when the founder says "policy watch", "any new MBG rules", "update regulations", "what changed in BGN / LKPP / BUMN". Searches the web for recent changes in MBG, procurement, BUMN, construction, OJK, labour, data, and tax rules, then updates the Regulasi and Ekosistem brains with dated, sourced entries.
argument-hint: "[topic, e.g. MBG | procurement | BUMN | construction | OJK | tax | all]"
---

## Steps

1. Read `.claude/skills/roast-room/brains/regulasi-indonesia/sources.md` and `.claude/skills/roast-room/brains/ekosistem-indonesia/sources.md`. List every entry tagged MED or VERIFY that matches the topic (default: all).
2. Search the web (load the WebSearch tool if needed). Run the searches in parallel, in Indonesian and English. Good queries: "peraturan BGN terbaru", "juknis SPPG", "Perpres MBG", "anggaran MBG realisasi", "SLHS SPPG", "Perpres pengadaan barang jasa perubahan", "e-katalog LKPP", "Danantara BUMN Karya", "BP BUMN", "OJK investasi ilegal Satgas PASTI", "PP perizinan berusaha berbasis risiko", "pajak UMKM PP 55". Prefer primary sources: peraturan.go.id, jdih of each agency, bgn.go.id, lkpp.go.id, ojk.go.id, kemenkeu.go.id, then reputable national media.
3. For each finding, record: instrument or fact, date, what changed, source URL, and the new confidence tag. Only mark HIGH when a primary source confirms it.
4. Update the brains:
   - Edit the matching row in `sources.md` (or add a new `R`/`E` id). Update the "Last full review" date.
   - If a rule changed how a decision should be made, update `_hot.md`, `frameworks.md`, or `positions.md` in plain English.
   - Never paste long legal text; summarise in one or two lines and link the source.
5. Report to the founder (under 200 words): what changed, which businesses it touches (construction, equipment, consulting, head hunting, supply chain, investments), and one action per material change. Flag anything that affects an open commitment or a pending decision.
6. Commit and push.

## Rules

- If a search returns nothing reliable, leave the tag as VERIFY and say so. Never upgrade confidence on a news headline alone.
- Do not include the founder's name, company names, or numbers in search queries.
