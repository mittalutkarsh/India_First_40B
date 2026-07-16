India-First 40B — Research Proposal
A plan to train a 40-billion-parameter language model, from scratch, that matches Gemma 4 on general tasks, is fluent across the top-ten Indian languages, and reasons from an Indian perspective. Published as a small static website.
Author: Utkarsh Mittal
***What this is
The proposal treats data provenance, the tokenizer, and the model's "Indian perspective" as one problem. Native Indic text is scarce — the largest cleaned corpus tops out near ~280B tokens against a 1.32T Indic budget — so most of the corpus is repeated native text plus a bounded amount of manufactured text. The novel part is a from-scratch experiment that measures whether the origin of the training data (native vs. translated) changes the geometry of the model's perspective direction, and whether that direction survives alignment.
It covers the full pipeline: data strategy, cleaning, the tokenizer and fertility targets, the analytical framework (F1–F7), and post-training.
Pages
| File | Section |
|---|---|
| index.html | Overview, visuals, and links to every section |
| problem.html | Problem & Approach — the constraint and the research reversal |
| data.html | Data Strategy — budget, provenance tiers, repetition rule, curriculum |
| cleaning.html | Data Cleaning — the nine objective-mapped stages |
| tokenizer.html | Tokenizer & Fertility — the minimax objective, per-language and per-domain targets, vocabulary, metrics |
| research.html | Research Core — the contrastive perspective corpus and F1–F7 |
| training.html | Post-training — native-first fine-tuning and alignment |
Viewing locally
The site is plain HTML with no build step. Open index.html in any browser. All links between pages are relative, so the folder works wherever it sits.
Deploying
GitHub Pages. Push these files to a public repo, then go to Settings → Pages → Deploy from a branch, set the branch to main and the folder to / (root), and save. The site goes live at https://<username>.github.io/<repo>/, serving index.html as the home page. The included empty .nojekyll file turns off Jekyll so nothing is mishandled.
Netlify Drop. Alternatively, drag the folder (or the zip) onto netlify.com/drop for an instant URL.
Notes
Static HTML and CSS only; fonts load from the Google Fonts CDN, so an internet connection is needed for the intended typography.
Illustrative examples and figures are labelled as such on the pages.
Gemma 4 numbers are vendor-reported and should be verified against the model card.
Several figures (the ~280B native ceiling and the 85/10/5 provenance split) reflect the working estimates in the proposal, not final measurements.
