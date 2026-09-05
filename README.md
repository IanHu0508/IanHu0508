# Ian Hu

**Financial AI · Research engineering · Full-stack systems**

I build software that makes financial calculations reproducible, evidence traceable, and business rules explicit. My work spans Python research models, TypeScript applications, and the evidence workflows that support reliable AI systems.

MSc Financial Technology student at Nanyang Technological University (NTU).

[Valuation code](https://github.com/IanHu0508/company-research-automation/tree/main/src/valuation_engine) · [Full-stack application](https://github.com/IanHu0508/finops-ledger-demo) · [Risk model](https://github.com/IanHu0508/koda-trf-risk-case-study) · [Live evidence demo](https://ianhu0508.github.io/evidencefinder-synthetic-demo/)

## Selected engineering work

### [Company Research Automation](https://github.com/IanHu0508/company-research-automation)

**Python · Decimal · JSON Schema**

An earnings-based SOTP valuation engine with explicit bear/base/bull assumptions. Decimal-string inputs avoid float conversion; source dates enforce the valuation cutoff; canonical JSON and SHA-256 support result-packet integrity checks.

[Model](https://github.com/IanHu0508/company-research-automation/blob/main/src/valuation_engine/model.py) · [Packet validation](https://github.com/IanHu0508/company-research-automation/blob/main/src/valuation_engine/packet.py) · [Tests](https://github.com/IanHu0508/company-research-automation/tree/main/tests) · [Runnable example](https://github.com/IanHu0508/company-research-automation/blob/main/examples/run_example.py)

*Public scope: runnable synthetic valuation; news-monitoring architecture is documented separately.*

### [FinOps Ledger](https://github.com/IanHu0508/finops-ledger-demo)

**TypeScript · Next.js · Prisma · PostgreSQL**

A financial operations prototype that separates cash, recognized revenue, deferred revenue, and receivables. Typed events and integer cents express the domain rules. Fixture and database repositories share an interface; database writes pair ledger events with audit records in one transaction.

[Architecture](https://github.com/IanHu0508/finops-ledger-demo/blob/main/docs/architecture.md) · [Domain rules](https://github.com/IanHu0508/finops-ledger-demo/tree/main/lib/accounting) · [Persistence](https://github.com/IanHu0508/finops-ledger-demo/blob/main/lib/repository/prisma-finance-repository.ts) · [Tests](https://github.com/IanHu0508/finops-ledger-demo/tree/main/tests)

*Public scope: standalone prototype using synthetic business data.*

### [KODA / TRF Risk Case Study](https://github.com/IanHu0508/koda-trf-risk-case-study)

**Python · NumPy · Monte Carlo · pytest · GitHub Actions**

A 100,000-path FX scenario model comparing a stylized structured payoff with a forward on the same simulated paths. Separates path generation, payoff mechanics, and tail-risk metrics; includes volatility/leverage sensitivity, reproducible artifacts, and CI.

[Model](https://github.com/IanHu0508/koda-trf-risk-case-study/blob/main/src/koda_trf/model.py) · [Tests](https://github.com/IanHu0508/koda-trf-risk-case-study/blob/main/tests/test_model.py) · [Results](https://github.com/IanHu0508/koda-trf-risk-case-study/tree/main/artifacts) · [CI](https://github.com/IanHu0508/koda-trf-risk-case-study/actions/workflows/ci.yml)

*Public scope: illustrative scenario stress testing, with assumptions and limitations in the report.*

### [EvidenceFinder](https://ianhu0508.github.io/evidencefinder-synthetic-demo/)

**Evidence retrieval · Source context · Human review**

A browser workflow for **search → inspect context → select → save → reopen**. Source locations stay attached to evidence, while personal notes remain separate from the original text.

[Try the demo](https://ianhu0508.github.io/evidencefinder-synthetic-demo/) · [Demo repository](https://github.com/IanHu0508/evidencefinder-synthetic-demo)

*Public scope: static demo with synthetic data; implementation source is private. The demo covers retrieval and evidence handling, without LLM inference.*

## How I approach AI engineering

- **Trace evidence before generating answers.** Source context and provenance are part of the system design.
- **Keep financial logic in explicit code.** Calculations, accounting rules, and input validation should be independently testable.
- **Test failure modes.** Future-dated sources, malformed inputs, duplicate events, and asymmetric payoffs deserve dedicated checks.
- **Make consequential actions reviewable.** Evidence selection, interpretation, and business decisions have distinct responsibilities.
