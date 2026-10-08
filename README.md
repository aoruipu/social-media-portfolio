# Social Media Partner — application page

**Deliverable:** `social-media-portfolio/index.html` (single self-contained page, 17 images in `assets/images/`)

## What this is

A revised, employer-facing version of the Word draft, built as a one-page scrolling portfolio for an
**internal IKEA move into the Social Media Partner role**. All 14 screenshots from the original document
are embedded in the section they belong to.

## Structure

| # | Section | Purpose |
|---|---|---|
| — | Hero | Portrait, name, one-line proposition, live links (recruitment work · LinkedIn), key figures (11,952 LinkedIn followers · 4 platforms · 5,415 followers on an employer channel · ~2,600 records) |
| 01 | How I approach social media | Four working habits + the questions asked before and after publishing |
| 02 | IKEA Employer Branding | Role, approach, what would be measured; film-day photo (portrait, shown whole) + campaign reference side by side |
| 03 | Life at Truecaller | Channel build, contribution list, follower/post figures |
| 04 | Personal content lab | LinkedIn (full-width), Instagram, Rednote, Tradera — focus / format / tool / why / learned |
| 05 | AI in practice | Deliberately prominent: three dreams turned into visuals (two AI stills + one AI film on TikTok, linked), a "I direct the model like a photographer" card, and the Dream → Prompt → Generate → Direct → Publish flow |
| 06 | From content to insight | Recruitment analytics dashboard, rounded metrics, what is tracked, tools |
| 07 | What I bring | Four blocks mapped to the role + a first-30/60/90 view |
| — | Footer | Contact links (currently placeholders) |

## Editorial changes vs. the draft

- Fixed typos and grammar throughout ("succuesfull camipan", "attact pepple", "visulizaiton", "follower" etc.).
- Added a clear proposition and a summary of relevance for the role instead of leaving the reader to infer it.
- Turned each case into the same repeatable structure: the idea → my role → what I did → what I measure → what I learned.
- Made the AI section genuinely prominent, with a workflow and a guardrails statement (it was flagged as high priority).
- Reframed the "What I would bring" list from four nouns into four role-relevant statements with evidence.
- Labeled non-owned material honestly: the IKEA "Taste the Future" news item is marked as a reference, and the
  Truecaller figures are marked as channel-level numbers.
- Softened the recruitment data per instruction: rounded figures, no candidate-identifiable data.

## Technical notes

- No external dependencies — opens straight from the file, works offline, prints cleanly to PDF.
- Light/dark theme toggle with system-preference default, persisted in localStorage.
- Scroll-reveal animations respect `prefers-reduced-motion`; images open in a lightbox for detail.
- Photos are placed at their native aspect ratio (`.frame.nat`) rather than cropped into a fixed frame, so portrait
  shots are shown whole; the film-day still was upscaled 2x with sharpening so it stays crisp on retina displays.
- Live links: `https://aoruipu.github.io/` (recruitment work) in the topbar, hero and footer;
  `https://www.linkedin.com/in/aorui/` in the hero and footer.
- Verified: 18/18 assets resolved, no broken references, no horizontal overflow at 485 / 545 / 605 / 753 / 885 / 1025 / 1345 px.

## Open items for AoRui

1. Confirm the exact scope of the Truecaller contribution (the page says "one of the content creators behind the channel").
2. Decide how to treat the dashboard screenshot — it still shows exact internal figures
   (2,639 / 124.7 / 66.3 / 46.7) even though the copy is rounded. Options: keep, blur the numbers, or swap for a simplified version.
3. Add an email address (the footer still has one placeholder link).
4. Add the years of experience at IKEA if a specific figure is available.
5. Optional: Rednote follower count (currently only post view counts are shown).
6. Optional: should TikTok (`@aoruisamuel`) also get a card in section 04? Needs follower / view numbers to be worth it.
