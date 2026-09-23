# Paolo Cudrano review comments — executive summary

Scope: Paolo's 23 active review threads on `executive_summary.tex` in the Overleaf executive-summary project, checked on 23 September 2026. The threads contain 24 Paolo messages because one thread has a reply. Overleaf showed no resolved comments at the time of extraction. Anchors below were checked against the highlighted source in Overleaf. Status records local source changes, not the Overleaf review-panel state. R numbers identify messages, including the reply.

## `executive_summary.tex`

- Anchor: Title page — thesis title
  Time: 18 September, 11:26 am
  Paolo comment:
    remember to fix as in the thesis

  Needed change [R001]: Match the title used in the main thesis.
  Status: ✅ Addressed
  Change made: Set the title to “Discrete Image Tokenizers under Perturbations and Distribution Shift.”

- Anchor: Motivation and Scope — section heading
  Time: 18 September, 11:26 am
  Paolo comment:
    Introduction

  Needed change [R002]: Name the opening section “Introduction.”
  Status: ✅ Addressed
  Change made: Renamed the section without changing its label.

- Anchor: Introduction — study objective
  Time: 18 September, 11:27 am
  Paolo comment:
    the robustness properties of

  Needed change [R003]: State explicitly that the thesis studies tokenizer robustness properties.
  Status: ✅ Addressed
  Change made: Added “studies the robustness properties of discrete image tokenizers” to the introduction.

- Anchor: Introduction — “as behavioral components rather than only as compression modules”
  Time: 18 September, 11:27 am
  Paolo comment:
    remove

  Needed change [R004]: Remove the highlighted comparison phrase.
  Status: ✅ Addressed
  Change made: Replaced that wording with a direct statement of the study objective.

- Anchor: Introduction — “concerns”
  Time: 18 September, 11:28 am
  Paolo comment:
    focuses on

  Needed change [R005]: Use “focuses on” for the two-tokenizer comparison.
  Status: ✅ Addressed
  Change made: The introduction now says it focuses on VQGAN and LlamaGen.

- Anchor: Introduction — “the tokenizer released with” before VQGAN
  Time: 18 September, 11:28 am
  Paolo comment:
    remove

  Needed change [R006]: Remove the highlighted lead-in before VQGAN.
  Status: ✅ Addressed
  Change made: Named VQGAN directly with its citation.

- Anchor: Introduction — “the tokenizer released with” before LlamaGen
  Time: 18 September, 11:29 am
  Paolo comment:
    remove (it's clear we refer to the tokenizer component of LlamaGen and not to the AR model, and the literature calls them both as "LlamaGen" depending on context)

  Needed change [R007]: Name LlamaGen directly without the qualifier.
  Status: ✅ Addressed
  Change made: Named LlamaGen directly with its citation.

- Anchor: Introduction — comparison beyond reconstruction
  Time: 18 September, 11:30 am
  Paolo comment:
    not only their reconstruction capabilities, but also their stability, spatial response and off-distribution degradation without conflating ...

  Needed change [R008]: Name the other behaviors examined alongside reconstruction.
  Status: ✅ Addressed
  Change made: Listed reconstruction quality, code stability, spatial response, and behavior under distribution shift.

- Anchor: Introduction — “without conflating them”
  Time: 18 September, 11:31 am
  Paolo comment:
    possible differences

  Needed change [R009]: Make clear that possible differences are not caused by interface size.
  Status: ✅ Addressed
  Change made: Rephrased the comparison around possible behavioral differences and the shared sequence length and vocabulary size.

- Anchor: Introduction — numbered research-question list
  Time: 18 September, 11:36 am
  Paolo comment:
    I would make this more discoursive, borrowing from the thesis intro.

  Needed change [R010]: Explain the sequence of research questions in prose.
  Status: ✅ Addressed
  Change made: Replaced the enumeration with four connected paragraphs covering the five questions and their motivation.

- Anchor: Introduction — “The central distinction is between fidelity and behavior” paragraph
  Time: 18 September, 11:36 am
  Paolo comment:
    remove

  Needed change [R011]: Remove the repeated closing explanation.
  Status: ✅ Addressed
  Change made: Removed that paragraph after rewriting the research-question overview.

- Anchor: Experimental Design — tokenizer architecture and training details
  Time: 18 September, 12:15 pm
  Paolo comment:
    not needed in the summary

  Needed change [R012]: Remove code dimensions and training-objective details.
  Status: ✅ Addressed
  Change made: Removed the two detailed tokenizer descriptions; retained only the released-checkpoint setup.

- Anchor: Experimental Design — pretrained checkpoints and inference-time perturbations
  Time: 18 September, 12:09 pm
  Paolo comment:
    this goes at the end in limitations

  Needed change [R013]: Move the causal caveat to Limitations.
  Status: ✅ Addressed
  Change made: Kept the setup factual and placed the architecture/training caveat in Limitations.

- Anchor: Experimental Design — pretrained checkpoints and inference-time perturbations
  Time: 18 September, 12:10 pm
  Paolo comment:
    here just say the fact: we focus on pretrained tokenizers and just run inference with perturbations

  Needed change [R014]: State the inference-only protocol directly.
  Status: ✅ Addressed
  Change made: Said the released checkpoints run inference with controlled perturbations and are not retrained.

- Anchor: Experimental Design — “Common tokenizer interface and evaluation data” table
  Time: 18 September, 12:14 pm
  Paolo comment:
    Not needed in the summary

  Needed change [R015]: Remove the setup table.
  Status: ✅ Addressed
  Change made: Removed the table; kept the essential interface and dataset descriptions in prose.

- Anchor: Experimental Design — “Measurements and interventions” heading
  Time: 18 September, 12:19 pm
  Paolo comment:
    In general, it's better to show less metrics in the summary than to overwhelm the reader. For sure, only present metrics you actually show in the rest of the summary. Double check and evaluate whether we need to remove some (not necessarily, your call)

  Needed change [R016]: Keep the summary to metrics used in its results.
  Status: ✅ Addressed
  Change made: Kept PSNR, SSIM, LPIPS, FID, active-code count, perplexity, and concentration; removed descriptions of sFID, precision, recall, and Inception Score. The RQ1 figure now shows only its four discussed reconstruction metrics.

- Anchor: Experimental Design — paired subsections
  Time: 18 September, 12:20 pm
  Paolo comment:
    i would not put them together. Either split or don't have subsections here

  Needed change [R017]: Avoid grouping tokenizers/data and measurements under two subsections.
  Status: ✅ Addressed
  Change made: Removed both subsection headings and kept a short Experimental Design section.

- Anchor: Experimental Design — effective-active threshold explanation
  Time: 18 September, 12:16 pm
  Paolo comment:
    slop, not needed in the summary

  Needed change [R018]: Remove the effective-active threshold detail.
  Status: ✅ Addressed
  Change made: Removed the threshold definition and its matching “effectively active” figures from RQ1.

- Anchor: Experimental Design — intervention protocol paragraph
  Time: 18 September, 12:17 pm
  Paolo comment:
    Too technical for the sumary, remove

  Needed change [R019]: Remove the dense advance description of intervention methods and formulas.
  Status: ✅ Addressed
  Change made: Removed the protocol paragraph; each result section introduces its own intervention.

- Anchor: Experimental Design — intervention protocol paragraph
  Time: 18 September, 2:34 pm
  Paolo comment:
    You can explain the details in the respective sections, don't spoiler here the method.

  Needed change [R020]: Explain methods where their results appear.
  Status: ✅ Addressed
  Change made: Kept the image-noise, local-patch, and token-edit descriptions in RQ2–RQ4, and removed their advance summary.

- Anchor: Experimental Design — “token flips”
  Time: 18 September, 2:33 pm
  Paolo comment:
    a bit informal

  Needed change [R021]: Avoid that informal phrase in the method overview.
  Status: ✅ Addressed
  Change made: Removed the overview sentence containing “token flips”; RQ2 describes changed token assignments directly.

- Anchor: Experimental Design — section length after protocol cuts
  Time: 18 September, 2:34 pm
  Paolo comment:
    Consider whether this section is left with enough material or if we should just put it somewhere else

  Needed change [R022]: Check whether Experimental Design still warrants a section.
  Status: ✅ Addressed
  Change made: Retained a compact section because it now covers the checkpoint protocol, reference datasets, and metrics without duplicating the RQ methods.

- Anchor: Global Robustness (RQ2) — token-flip figure
  Time: 18 September, 12:12 pm
  Paolo comment:
    too big, there's a bunch of blank space wasted in this page

  Needed change [R023]: Reduce the RQ2 figure's footprint and inspect the page layout.
  Status: ✅ Addressed
  Change made: Reduced its width from 0.92 to 0.76 of the text width. The local PDF now fits six pages with readable axes.

- Anchor: Bibliography — citation and reference ordering style
  Time: 18 September, 11:35 am
  Paolo comment:
    Suggestion on bib style (both here and in the thesis): it's a matter of style so pick what you like best.
    Personally, with numeric [i] like IEEE style, I would order the entries by first appearance in the text and not alphabetically. This means the text reports in order [1], [2], etc, which looks nicer.
    Otherwise I like a lot NeurIPS style with \setcitestyle{authoryear,round,citesep={;},aysep={,},yysep={;}}, but I don't know if it's allowed in the thesis, you should check the guidelines

  Needed change [R024]: Choose a consistent citation style for this summary.
  Status: ✅ Addressed in the executive summary
  Change made: Kept numeric citations and changed the bibliography to `unsrtnat`, so entries follow first appearance. Paolo also suggested considering this in the separate thesis; its style is unchanged here.
