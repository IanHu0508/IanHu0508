# Ian Hu

**Quantitative finance · Research engineering · Financial AI**

I build research software with reproducible calculations, traceable evidence, and explicit assumptions. My work focuses on quantitative risk models and the engineering foundations of financial research systems.

MSc Financial Technology student at Nanyang Technological University (NTU).

[Valuation engine](https://github.com/IanHu0508/company-research-automation/tree/main/src/valuation_engine) · [Quantitative risk model](https://github.com/IanHu0508/koda-trf-risk-case-study)

## Selected engineering work

### [Company Research Automation](https://github.com/IanHu0508/company-research-automation)

**Python · Decimal · JSON Schema**

An earnings-based SOTP valuation engine with explicit bear/base/bull assumptions. Decimal-string inputs avoid float conversion; source dates enforce the valuation cutoff; canonical JSON and SHA-256 support result-packet integrity checks.

[Model](https://github.com/IanHu0508/company-research-automation/blob/main/src/valuation_engine/model.py) · [Packet validation](https://github.com/IanHu0508/company-research-automation/blob/main/src/valuation_engine/packet.py) · [Tests](https://github.com/IanHu0508/company-research-automation/tree/main/tests) · [Runnable example](https://github.com/IanHu0508/company-research-automation/blob/main/examples/run_example.py)

*Public scope: runnable synthetic valuation; news-monitoring architecture is documented separately.*

### [KODA / TRF Risk Case Study](https://github.com/IanHu0508/koda-trf-risk-case-study)

**Python · NumPy · Monte Carlo · pytest · GitHub Actions**

A 100,000-path FX scenario model comparing a stylized structured payoff with a forward on the same simulated paths. Separates path generation, payoff mechanics, and tail-risk metrics; includes volatility/leverage sensitivity, reproducible artifacts, and CI.

[Model](https://github.com/IanHu0508/koda-trf-risk-case-study/blob/main/src/koda_trf/model.py) · [Tests](https://github.com/IanHu0508/koda-trf-risk-case-study/blob/main/tests/test_model.py) · [Results](https://github.com/IanHu0508/koda-trf-risk-case-study/tree/main/artifacts) · [CI](https://github.com/IanHu0508/koda-trf-risk-case-study/actions/workflows/ci.yml)

*Public scope: illustrative scenario stress testing, with assumptions and limitations in the report.*

## How I approach AI engineering

- **Trace evidence before generating answers.** Source context and provenance are part of the system design.
- **Keep financial logic in explicit code.** Calculations, model assumptions, and input validation should be independently testable.
- **Test failure modes.** Future-dated sources, malformed inputs, duplicate scenarios, and asymmetric payoffs deserve dedicated checks.
- **Make consequential actions reviewable.** Evidence selection, interpretation, and business decisions have distinct responsibilities.
