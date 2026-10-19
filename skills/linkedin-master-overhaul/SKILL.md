---
name: linkedin-master-overhaul
description: End-to-end LinkedIn profile overhaul combining PDF intake, design-tree grilling, de-AI-ified copywriting, and bilingual step-by-step guides. Use when optimizing a LinkedIn profile for inbound opportunities, personal branding, or recruiter search visibility.
---

# LinkedIn Master Overhaul

Transform a LinkedIn profile into a 10/10 inbound recruiter magnet through four sequential phases: **Fact Discovery → Design-Tree Grilling → Step-by-Step 10/10 Guide → Bilingual Localization**.

---

## Phase 1: Fact Discovery (No User Labor)

Before asking the user any questions, gather ground truth from the environment:

1. Search the workspace and `~/Downloads` for LinkedIn PDF exports (`Profile*.pdf`) and resumes (`*cv*.pdf`, `*resume*.pdf`). If the user has not exported their LinkedIn PDF yet, instruct them: *"On your LinkedIn profile, click **Resources / More → Save to PDF** and drop `Profile.pdf` in `~/Downloads`."*
2. Extract text from both the LinkedIn PDF and resume PDF.
3. Audit for **Recruiter Boolean Traps**:
   - Compare the Headline role against the official **Experience** titles (e.g., Headline says `Software Engineer` while Experience says `Data Analyst`).
   - Identify missing metrics, buried institutional prestige (university rank, research labs, awards), self-deprecating sentences, broken spacing, and empty Featured sections.

**Phase 1 Completion Criterion:** Both PDF sources (or user-supplied profile text) are parsed and every discrepancy between actual scope and listed Experience titles is cataloged.

---

## Phase 2: Design-Tree Grilling

Invoke the `grilling` methodology. Work the decision tree in rounds of numbered questions (`❓ **Q1** ... ➡️ **Recommended Answer**`), phrasing each so "yes" accepts the recommendation. Wait for the user's response after each round.

Cover these branches across rounds until the frontier is empty:

1. **Title Realignment:** Aligning formal HR titles in Experience with functional search titles recruiters filter by (`Software Engineer`, `AI Engineer`, `Tech Lead`).
2. **Positioning Niche & High-Compensation Tier:** Selecting the highest-leverage specialization supported by their ground truth (e.g., AI Systems & Infrastructure vs. generic generalist).
3. **Geography, Remote & Relocation:** Targeting global remote markets (US/EU timezones) and relocation vs. domestic roles.
4. **Visibility & Notification Preferences:** Framing copy around subject-matter authority, managing network update notifications during bulk edits, and configuring LinkedIn's backend recruiter preferences.
5. **Role Scope Verification:** Confirming the exact day-to-day reality of the current role so zero metrics or claims are fabricated.

**Phase 2 Completion Criterion:** Every branch of the design tree is settled and the user confirms the shared understanding summary. Do not generate profile copy before this confirmation.

---

## Phase 3: Step-by-Step 10/10 Master Guide

Write a complete, copy-paste-ready Markdown guide saved to `~/Downloads/LinkedIn_10_of_10_Master_Guide.md` (and summarized in chat) structured in **8 ordered execution steps**:

1. **Step 1 — Notification Toggle:** Instructions to disable `Share profile updates with your network` before bulk-editing sections so contacts aren't spammed with edit notifications.
2. **Step 2 — Intro Card & Headline:** Primary and conservative Headline variants (<220 chars) combining Role + Niche + Hard Metric + Core Stack.
3. **Step 3 — About Section & Top 5 Pinned Skills:** Full About section (~200–220 words) plus the exact 5 skills to pin inside the About modal.
4. **Step 4 — Complete Experience Overhaul (Every Role):** Provide the exact `Title`, `Location`, `Description` bullets, and `Stack` line for **every single role** on the user's profile (current role, prior roles, research positions, student leadership, and early internships). Never skip or leave older roles without copy-paste text.
5. **Step 5 — Featured Section:** Exact titles, descriptions, and links for 2–3 high-proof engineering/portfolio artifacts.
6. **Step 6 — Education & Honors:** Translated degree titles, GPA/class rank, and capstone awards.
7. **Step 7 — Backend Recruiter Preferences:** Exact 5 job titles, work types, and global target locations (`United States`, `European Union`, `United Kingdom`, `Canada`, plus local country) to match international search filters.
8. **Step 8 — Cross-Platform Entity Sync:** 1-line bio update for GitHub/portfolio so AI search engines (ChatGPT, Perplexity, Claude) triangulate identity.

### Voice & De-AI-ify Rules (Mandatory Across All Copy)

- **First-person voice after the hook:** Open the About section with a one-sentence industry bottleneck statement, then write the rest of the About and Experience sections in natural **first-person ("I")**.
- **Explicit topic transitions:** Connect separate career chapters (current role, academic pedigree, prior roles, research) with clear transition phrases (`In my current role at...`, `My foundation in... started during...`, `Previously at...`, `During my research at...`).
- **Clean human punctuation:** Separate clauses with commas, parentheses, or periods. Never use em-dashes (`—`) inside copy-paste blocks.
- **Direct verb-led bullets:** Start Experience bullets directly with strong action verbs or metrics (`• Cut turnaround by 98.9%...`, `• Lead the technical and economic feasibility...`) rather than bold title-case labels (`• Turnaround Reduction: Cut...`).

**Phase 3 Completion Criterion:** `LinkedIn_10_of_10_Master_Guide.md` is written to disk with zero em-dashes in copy blocks, every Experience entry included in full, and verified 10/10 scores across all 5 audit dimensions (50/50) and 8/8 AI Visibility checks.

---

## Phase 4: Bilingual Localization (When Requested or Multi-Language Profile)

When the user maintains a secondary language tab on LinkedIn (e.g., Portuguese `PT-BR`):

1. Generate a matching companion file (`~/Downloads/LinkedIn_10_of_10_Master_Guide_<LANG>.md`) translating Steps 2, 3, 4 (all roles), and 6.
2. Preserve standard English technical terms used in that market (`LLMOps`, `open-weight`, `on-premises`, `serverless`, `RAG`, `HPC`, `benchmark`, `CI/CD`, `churn`) while writing natural native syntax with zero em-dashes.
3. Include instructions on switching the language tab in the top-right corner of the LinkedIn profile before clicking the edit pencil on each section.

**Phase 4 Completion Criterion:** The localized guide file is saved to disk with every role translated and natural native transitions preserved.

---

## Credits & Referenced Skills

This workflow orchestrates concepts from and pairs with the following community skills (install from their upstream repositories):

- **`grilling`** & **`writing-for-agents`** by Matt Pocock ([`mattpocock/skills`](https://github.com/mattpocock/skills))
- **`linkedin-profile-optimizer`** by Brian Wagner ([`BrianRWagner/ai-marketing-skills`](https://github.com/BrianRWagner/ai-marketing-skills))
- **`de-ai-ify`** by theflohart
- **`resume-quantifier`** & **`resume-bullet-writer`** by Param Choudhary ([`paramchoudhary/resumeskills`](https://github.com/paramchoudhary/resumeskills))
