# Ian Hu

**Financial AI · Quantitative Research · Research Engineering**

MSc Financial Technology student at Nanyang Technological University (NTU).

I build auditable financial research and quantitative systems where evidence, assumptions, and calculations can be inspected independently. My current work spans LLM research workflows, source-backed security research, quantitative risk and derivatives, and production data systems.

[FinResearchOps](https://github.com/IanHu0508/FinResearchOps) · [SOTP valuation engine](https://github.com/IanHu0508/company-research-automation) · [KODA / TRF risk case study](https://github.com/IanHu0508/koda-trf-risk-case-study)

## Current focus

| Workstream | Status | Current focus |
| --- | --- | --- |
| Financial AI | **Active · public flagship** | **FinResearchOps** — native TradingAgents research workflow with independent drafts, counterevidence revision, a fresh final assessment, and separate deterministic filing checks. The lightweight research slice is implemented; reliability and bias-reduction validation remain ongoing. |
| Security research & valuation | **Active · private** | Source-backed research foundation with canonical `ResearchPacket` contracts and evidence provenance. The foundation is implemented; the valuation path is being reviewed before broader publication. |
| Quant / ML | **Active · private** | JPM chooser-option study. The reproducible 2018–2024 market, rates, volatility, and sentiment dataset is in place; analytic/BSM chooser pricing, Monte Carlo validation, and ML volatility modeling are the next implementation layer. |
| Research agents | **Active · private** | Provenance-first, source-constrained multimodal research Agent with traceable citations, replayable run records, and explicit human-review boundaries. |
| Quant research platform | **Stable · private** | A-share ETF/factor research platform with market-microstructure constraints, fee-aware T+1 backtests, walk-forward evaluation, and CSCV/PBO overfitting controls. |
| Production engineering | **Maintained · private** | Production Next.js/PostgreSQL operations system with explicit data-integrity, backup, credential, and deployment controls. |

**Core stack:** Python · TypeScript · LangGraph · Next.js · PostgreSQL · Prisma · NumPy · pytest · GitHub Actions

## Selected public engineering work

### [FinResearchOps](https://github.com/IanHu0508/FinResearchOps) — auditable financial research workflow

**Flagship · Active**  
**Python · LangGraph · TradingAgents · structured research workflows**

Built on the native TradingAgents chain. Independent first drafts are kept separate, each side responds to itemized counterevidence, and the final manager receives original sources plus revised arguments without upstream ratings or trader-authored thresholds. An optional report-review Agent is advisory only; deterministic filing checks remain a separate capability.

[Research workflow](https://github.com/IanHu0508/FinResearchOps/blob/main/docs/thesis-research.md) · [Financial checks](https://github.com/IanHu0508/FinResearchOps/blob/main/docs/cashflow-investigation.md) · [Integration tests](https://github.com/IanHu0508/FinResearchOps/tree/main/integration_tests) · [Status and limits](https://github.com/IanHu0508/FinResearchOps/blob/main/docs/status.md)

*The public implementation is reproducible and testable, but no claim is made that it removes model bias, improves investment returns, or replaces human financial review.*

### [Company Research Automation](https://github.com/IanHu0508/company-research-automation) — explicit SOTP valuation

**Stable portfolio**  
**Python · Decimal · JSON Schema · canonical JSON**

An earnings-based SOTP valuation engine with explicit bear/base/bull assumptions. Decimal-string inputs avoid silent float conversion, source dates enforce the valuation cutoff, and canonical JSON plus SHA-256 support result-packet integrity checks.

[Model](https://github.com/IanHu0508/company-research-automation/blob/main/src/valuation_engine/model.py) · [Packet validation](https://github.com/IanHu0508/company-research-automation/blob/main/src/valuation_engine/packet.py) · [Tests](https://github.com/IanHu0508/company-research-automation/tree/main/tests) · [Runnable example](https://github.com/IanHu0508/company-research-automation/blob/main/examples/run_example.py)

### [KODA / TRF Risk Case Study](https://github.com/IanHu0508/koda-trf-risk-case-study) — path-dependent risk modeling

**Stable portfolio**  
**Python · NumPy · Monte Carlo · pytest · GitHub Actions**

A reproducible 100,000-path FX scenario study comparing a stylized structured payoff with a forward on the same simulated paths. It separates path generation, payoff mechanics, tail-risk metrics, and sensitivity analysis, with fixed-seed artifacts and CI.

[Model](https://github.com/IanHu0508/koda-trf-risk-case-study/blob/main/src/koda_trf/model.py) · [Tests](https://github.com/IanHu0508/koda-trf-risk-case-study/blob/main/tests/test_model.py) · [Results](https://github.com/IanHu0508/koda-trf-risk-case-study/tree/main/artifacts) · [CI](https://github.com/IanHu0508/koda-trf-risk-case-study/actions/workflows/ci.yml)

## Additional public work

[FinOps Ledger](https://github.com/IanHu0508/finops-ledger-demo) is a synthetic, audit-oriented finance event ledger built with Next.js, TypeScript, Prisma, and PostgreSQL. It separates cash movement, recognized revenue, contract liabilities, and receivables, and keeps database writes and audit records inside explicit transaction boundaries.

## Engineering principles

- **Evidence before conclusions.** Source context, provenance, and information cutoffs are part of the system contract.
- **Deterministic financial logic where possible.** Calculations, assumptions, validation rules, and accounting transitions should remain independently testable.
- **Failure modes are first-class.** Future-dated evidence, malformed inputs, duplicated scenarios, provider failures, and asymmetric payoffs deserve dedicated tests.
- **Consequential outputs stay reviewable.** Retrieval, interpretation, calculation, and final business or investment judgment should not collapse into one opaque model call.
