# Yiqi Hu

**Financial Machine Learning · Quantitative Research · Research Engineering**

MSc Financial Technology student at Nanyang Technological University (NTU), with an undergraduate background in Financial Engineering. Quantitative Strategy Intern at Morgan Stanley Securities (China).

I use Python to study volatility, derivative payoffs and financial research systems.

## Selected work

### JPM Volatility & Chooser Option Research

A forward-RV20 forecasting and simple-European-chooser study using matched 7/10/15-year histories.

- Compared EWMA with Ridge, Random Forest, XGBoost and LSTM across market-only, news-activity and sentiment feature sets under expanding-window evaluation and repeated-seed experiments.
- Completed **2,196 development fits and 549 locked 2024 test fits**. The predeclared 15-year Ridge market-only candidate reduced MAE/RMSE versus EWMA by **10.17% / 10.01%**. The lowest observed test means came from 10-year RF C, while its MAE gain over market-only RF A was only about **0.21%**.
- Implemented analytical and two-stage risk-neutral Monte Carlo pricing for a simple European chooser option, including decision-boundary, sensitivity, convergence and estimator-comparison studies.

### [FinResearchOps](https://github.com/IanHu0508/FinResearchOps)

A Python / LangGraph financial research agent with independent long/short drafts, structured counterevidence revisions and financial calculations performed outside the language model. Forecast assumptions are stored in structured contracts, recalculated in Python and bound to the final report.

A separate A-share quant module defines 60-session inputs, 20-session forward-return targets, purged splits and Rank IC evaluation. A real-data run was invalidated after a historical ticker-identity issue changed universe membership and labels.

[Research workflow](https://github.com/IanHu0508/FinResearchOps/blob/main/docs/thesis-research.md) ·
[Quant module](https://github.com/IanHu0508/FinResearchOps/blob/main/quant/README.md) ·
[Current status](https://github.com/IanHu0508/FinResearchOps/blob/main/docs/status.md)

### [KODA / TRF Risk Case Study](https://github.com/IanHu0508/koda-trf-risk-case-study)

A 100,000-path Monte Carlo study comparing a stylized FX target-redemption payoff with a vanilla forward, focusing on tail losses and sensitivity to downside leverage and volatility.

## Other work

[FinOps Ledger](https://github.com/IanHu0508/finops-ledger-demo) — synthetic financial-event ledger separating cash receipts, recognized revenue, contract liabilities and receivables.

**Local Source Research Agent — private** — local Qwen3.5-9B workflow with allowlisted document/image tools, replayable source windows and bounded model/tool budgets.

[Scenario Valuation](https://github.com/IanHu0508/company-research-automation) — runnable synthetic SOTP model with explicit scenario assumptions and reproducible outputs.

## Tools

Python · NumPy · pandas · scikit-learn · XGBoost · PyTorch · LangGraph · SQL · PostgreSQL · TypeScript
