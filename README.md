# Ian Hu

**Quantitative Research · Financial Machine Learning · Research Engineering**

MSc Financial Technology student at Nanyang Technological University (NTU) and Quantitative Research Intern at Morgan Stanley.

Current work centers on volatility modeling, derivatives, financial ML, and LLM-based research workflows. Most projects are built in Python and focus on turning a financial question into a clean dataset, a testable model, and an evaluation that can be reproduced.

[FinResearchOps](https://github.com/IanHu0508/FinResearchOps) · [KODA / TRF risk case study](https://github.com/IanHu0508/koda-trf-risk-case-study) · [SOTP valuation engine](https://github.com/IanHu0508/company-research-automation)

## Current focus

| Area | Current work |
| --- | --- |
| Quantitative Research | JPM volatility forecasting and chooser-option research using 2018–2024 market, rates, VIX, and timestamp-aligned news data. Current experiments compare RV20 forecasts from EWMA, Ridge, Random Forest, XGBoost, and LSTM on annual walk-forward splits, with the 2024 period kept held out. |
| Financial AI | **FinResearchOps** combines an LLM-based investment-research workflow with a separate A-share quantitative research module. Current quant work is focused on market-data quality, universe construction, 20-session cross-sectional targets, and walk-forward evaluation. |
| Derivatives & Risk | Option pricing and structured-payoff research using analytic pricing, Monte Carlo validation, sensitivity analysis, and tail-risk diagnostics. |

## Selected work

### [FinResearchOps](https://github.com/IanHu0508/FinResearchOps) — Financial Research & Quant Infrastructure

**Python · LangGraph · TradingAgents · Quantitative Research**

FinResearchOps combines a modified TradingAgents research workflow with a separate quantitative research module.

On the research side, models work from source material, opposing arguments, and explicit revisions before a final assessment is produced. On the quant side, the project defines 60-session market inputs, 20-session forward-return targets, purged splits, Rank IC evaluation, and versioned research signals.

The first real A-share panel also surfaced a historical ticker-identity problem that changed universe membership and labels. Those results were invalidated and retained for audit rather than presented as investment performance.

[Research workflow](https://github.com/IanHu0508/FinResearchOps/blob/main/docs/thesis-research.md) ·
[Quant research](https://github.com/IanHu0508/FinResearchOps/blob/main/quant/README.md) ·
[Current status](https://github.com/IanHu0508/FinResearchOps/blob/main/docs/status.md)

### JPM Volatility & Chooser Option Research

**Python · Time-Series ML · XGBoost · LSTM · Derivatives**

A private 2018–2024 JPM study covering volatility forecasting and chooser-option pricing.

The pipeline combines market data, interest rates, VIX, and timestamp-aligned news sentiment. Forward RV20 is compared across EWMA, Ridge, Random Forest, XGBoost, and LSTM using annual expanding-window evaluation, with separate market-only, news-activity, and sentiment feature groups.

The 2024 period remains held out while model stability and the incremental contribution of news and sentiment are still being evaluated.

### [KODA / TRF Risk Case Study](https://github.com/IanHu0508/koda-trf-risk-case-study)

**Python · NumPy · Monte Carlo · Derivatives**

A 100,000-path Monte Carlo study of a path-dependent FX structured payoff.

The project compares the structured payoff with a conventional forward under the same simulated scenarios and examines downside risk, tail behavior, and parameter sensitivity.

[Model](https://github.com/IanHu0508/koda-trf-risk-case-study/blob/main/src/koda_trf/model.py) ·
[Tests](https://github.com/IanHu0508/koda-trf-risk-case-study/tree/main/tests) ·
[Results](https://github.com/IanHu0508/koda-trf-risk-case-study/tree/main/artifacts)

## Other projects

### [Company Research Automation](https://github.com/IanHu0508/company-research-automation)

Python SOTP valuation model with bear/base/bull scenarios, valuation-date controls, and reproducible output packets.

### [FinOps Ledger](https://github.com/IanHu0508/finops-ledger-demo)

Synthetic finance event ledger built with Next.js, TypeScript, Prisma, and PostgreSQL, with transaction-level accounting and audit records.

## Tools

**Python · SQL · TypeScript · NumPy · XGBoost · LangGraph · PostgreSQL · Git · GitHub Actions**
