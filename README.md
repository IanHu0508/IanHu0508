# Yiqi Hu

**Financial Machine Learning · Quantitative Research · Research Engineering**

MSc Financial Technology student at Nanyang Technological University (NTU), with an undergraduate background in Financial Engineering. Quantitative Strategy Intern at Morgan Stanley Securities (China).

I use Python to study volatility, derivative payoffs and financial research workflows.

## Selected work

### JPM Volatility & Chooser Option Research — private

A 2018–2024 study of forward realized volatility and simple European chooser-option pricing.

- Compares historical RV and EWMA with Ridge, Random Forest, XGBoost and LSTM under annual expanding-window evaluation.
- Separates market-only, news-activity and sentiment features, with repeated-seed checks for stochastic models; 2024 remains held out.
- Implements analytical and Monte Carlo chooser pricing separately from the ML forecasting work.

### [FinResearchOps](https://github.com/IanHu0508/FinResearchOps)

A TradingAgents-based research workflow with independent drafts, explicit counterevidence revisions and financial calculations performed in Python. Report figures are bound to recalculated results rather than copied model numbers.

A separate A-share module defines 60-session inputs, 20-session forward-return targets, purged splits and Rank IC evaluation. The first real-data run was withheld after a ticker-identity issue changed universe membership and labels.

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
