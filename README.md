# Merged Group Report — Funding-Rate Arbitrage (MFIN7092)

Single combined LaTeX report merging all four contributions.

## Files
- `report.tex` — the merged document (two-column IEEE style)
- `report_bib.bib` — merged bibliography (Cao's BibTeX + Liang Mengxuan's references)
- `figures/` — all figures: mine (`an_*`, `eda_*`, `final_*`), cja (`cja_*`), lmx (`lmx_fig1..7`)

## Structure
1. **Introduction** — Liang Yingxi (3035771024); includes the two taxonomy
   tables OCR'd from the original images.
2. **Strategy 1: Rule-Based Cross-Exchange Capture** — Chen Junan (3036555025);
   converted from `cja/report/main.typ`.
3. **Strategy 2: Same-Asset Cross-Exchange Funding Strategies** — two
   sub-strategies: **2.1** Payment-Aware Funding Carry, Warren Sim Hong
   (3036555893), from `warren_latex_package` (`warren_*` figures); **2.2**
   No-Arbitrage-Bound Convergence Trade, Wu Zeliang (3036556823), from
   `rma_latex` (`rma_fig*` figures).
4. **Strategy 3: Dual-Engine Funding + Momentum Long/Short** — Deng Xuying
   (3036555556) and Liang Jiarui (3036549789); converted from
   `ljr&dxy/Funding+Momentum.docx`, 3 figures (`ljr_fig*`).
5. **Strategy 4: Cost-Aware Positive Funding-Basis Carry** — Liang Mengxuan
   (3036551495); converted from the `.docx`, redundant intro/lit-review/
   conclusion trimmed, 7 figures placed in original document order.
6. **Strategy 5: Cross-Exchange Spread + Negative Cash-and-Carry** — Cao Zhaoli
   (3036668420); the original `Funding_Arbitrage` body, headings demoted one
   level, intro/conclusion folded into the shared ones. Its two sub-strategies
   are now named **5.1** (cross-exchange spread) and **5.2** (negative
   cash-and-carry), formerly "Strategy A/B".
7. **Conclusion** — unified synthesis of all five strategies.
8. **References** — single merged list (IEEEtran style).

Each part carries its author's name + student ID as a byline under the heading.

## Building
No TeX engine is installed on this machine, so the PDF was **not** compiled
here. Build on Overleaf (or local TeX Live) with:

```
pdflatex report
bibtex   report
pdflatex report
pdflatex report
```

`IEEEtran.bst` is needed for the bibliography (standard on Overleaf).

## Decisions taken (confirmed with the team)
- Unified single report (one shared intro + conclusion + bibliography),
  not four self-contained parts.
- Two-column IEEE layout; wide tables use `table*` (full page width).
- One merged bibliography at the end.
