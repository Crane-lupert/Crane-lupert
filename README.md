# Hyun Ahn — quantitative research portfolio

Systematic disclosure- and event-driven equity signals. Each study is pre-registered before the outcome data is opened, and reported with its out-of-sample result whichever way it came out.

[SSRN author page](https://papers.ssrn.com/sol3/cf_dev/AbsByAuth.cfm?per_id=11481608) · [GitHub](https://github.com/Crane-lupert)

---

## Published research

Seven working papers on SSRN, each paired with a public replication repository.

| Paper | Result | Code |
|---|---|---|
| **[Reading the Insider Cluster](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7178138)** (Jul 2026) — do multi-insider open-market buy clusters still inform once the concurrently filed disclosure's own language is classified? | 38,261 clusters screened from 1.93M SEC filings, 2015–2025. Classified cohort earns **+1.68% five-day FF5+UMD-residual CAR** (n = 32,098). | [repo](https://github.com/Crane-lupert/us-insider-form4-cluster-intent-llm) |
| **[Reading the Bylaws](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7149641)** (Aug 2026) — 8-K Item 5.03 bylaw amendments classified by governance direction, tracked for repeat amenders. | **+3.65% 63-day CAR, t = 5.0** (n = 1,491 events, 15-year sample). Reported as a mechanism result — the paper declines to claim a tradable strategy. | [repo](https://github.com/Crane-lupert/us-8k-bylaws-amend-llm) |
| **[Earnings-Announcement Cadence Variance](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6965838)** (Jul 2026) — second-moment extension of Bagnoli–Kross–Watts (2002): the rolling volatility of a firm's reporting lag. | 620,290 firm-quarters, 1999–2024. In-sample net Sharpe **1.01**; out-of-sample **11/12 cells sign-correct but 0/12 clear the Bonferroni bar** — published as a documented out-of-sample miss. | [repo](https://github.com/Crane-lupert/us_compustat_rdq_recognition_timing_xs) |
| **[Reading the Late-Filing Notification](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6932478)** (Jul 2026) — Form NT 12b-25 narratives classified into three causes, tested against subsequent restatement disclosures. | **10/12 pre-registered cells pass Bonferroni.** Net Sharpe **0.46 → 0.59** once entry is re-anchored to a point-in-time tradable timestamp. | [repo](https://github.com/Crane-lupert/us_sec_form_nt_late_filing_xs) |
| **[Hedger Positioning to Producer Equity](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6730238)** (May 2026) — CFTC producer-hedger positioning shocks mapped onto the equity of the producers themselves. | Best deployable cell **net Sharpe 1.15**, cluster-bootstrap 95% CI **[0.50, 1.83]**, across 36 producers in 12 commodities. | [repo](https://github.com/Crane-lupert/cot_producer_cross_section) |
| **[Cross-Country Validation of Bank Lending Shocks](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6729904)** (May 2026) — a US sector-response finding re-tested on Eurozone and UK lending surveys. | Sector ordering replicates in the Eurozone (**rank ρ = +0.76, p = 0.007** vs US at 6 months); the UK arm fails on universe power and is reported as a null. | [repo](https://github.com/Crane-lupert/sloos_sector_external_validation) |
| **[Zero-Shot Replication of SEC Comment-Letter Returns](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6729618)** (May 2026) — out-of-sample reproducibility test of a published comment-letter result under zero-shot classification. | **+11.9%/yr residual alpha, t = 2.86** on 1,014 letter pairs (2015–2024; out-of-sample window 2022–2024). | [repo](https://github.com/Crane-lupert/sec-comment-letter-alpha) |

## In the pipeline

**Recurring special dividends and post-announcement drift** — locked July 2026 after clearing its pre-registered gates (orthogonality to earnings surprise; net-of-cost cluster-robust t of 2.8–3.7 ex-microcap). Preprint submitted to SSRN; [code already public](https://github.com/Crane-lupert/us-special-dividend-recurring-drift-xs).

## How the research is run

- **Pre-registration.** Hypothesis, sample, primary cells, multiple-comparison correction and kill conditions are written and committed before the outcome data is opened; the commit history is the timestamp.
- **Selection ledger.** Every candidate that entered the funnel is recorded, not only the ones that survived, so the search cost behind a published result is on the record rather than implied.
- **Tooling.** I designed and operate a multi-agent execution stack that runs the data, testing and reporting pipeline end to end; hypotheses, gates and verdicts are mine. The governance layer is itself open: [quant-research-process](https://github.com/Crane-lupert/quant-research-process).

## Negative results

Projects that fail their gates get a written post-mortem rather than a quiet deletion — **11 published so far**, alongside **31 public repositories that carry an explicit FROZEN / RETRACTED / TERMINAL marker** in place of a result. Where a later audit finds a claimed contribution does not hold, the work is withdrawn rather than reframed.

<sub>Sources: CRSP, Compustat, SEC EDGAR, CFTC Commitments of Traders, OptionMetrics, and central-bank bank-lending surveys (Fed SLOOS, ECB BLS, BoE CCS). Repositories hold code and derived outputs, not vendor data.</sub>

<sub>_Last updated: August 2026_</sub>
