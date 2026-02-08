# Contributing

**Welcome.** If you're interested in improving how we measure epistemic humility in AI systems, there are several meaningful ways to contribute.

> **Project:** SIGMA Epistemic Humility Evaluator · **Author:** Rafa - The Architect · **License:** MIT

---

## Ways to Contribute

### Test Additional AI Models

The current dataset covers four frontier models. We need results for open-source models (Llama, Mistral, Phi, etc.), multilingual models, and domain-specific systems.

**How:** Use the stress tests from [HOW-TO-TEST.md](HOW-TO-TEST.md). Record the complete response, score it using `sigma_auditor.py`, and submit results via GitHub issue or pull request.

**Format for submissions:**

```markdown
**Model:** [name and version]
**Test:** [stress test name]
**P Score:** [0.00–1.00]
**Ξ:** [0–1000]
**Nodes:** [count]
**Noise:** [count]
**Full Response:** [verbatim text]
```

### Design New Stress Tests

We need tests that cover additional authority domains — medical, legal, military, environmental, governance. Good stress tests must involve contested normative categories, create tension between "being correct" and respecting authority, and have no single objectively correct answer.

See the existing tests in [HOW-TO-TEST.md](HOW-TO-TEST.md) for the design template.

### Improve the Evaluator

The current implementation uses keyword detection. Meaningful improvements would include semantic analysis (embedding-based marker detection), multi-language keyword dictionaries, context-aware scoring (e.g., Gemini's "my decision is to not decide" paradox), and multi-turn conversation analysis.

**Stack:** Python 3.6+. Fork the repo, create a feature branch, and submit a pull request.

### Translate Documentation

Priority languages: Spanish, Chinese (Mandarin), Hindi, Arabic, French, Portuguese. Start with [GUIDE-FOR-EVERYONE.md](GUIDE-FOR-EVERYONE.md) — it's the most accessible entry point. Preserve technical terms (P, Ξ, N, S) and document structure.

### Replicate Results

Independent replication is critical for scientific validity. Re-test the models we've already tested, score the responses independently, and report whether your P scores agree or disagree with ours. Disagreements are as valuable as agreements.

---

## Contribution Process

**For small changes** (typos, documentation fixes, minor improvements): submit a pull request directly.

**For large changes** (new features, methodology changes, structural reorganization): open an issue first to discuss the approach.

**Pull request checklist:**

- [ ] Code follows existing project style
- [ ] Documentation updated if applicable
- [ ] No references to paths or files that don't exist
- [ ] Dates and author name are correct (Rafa - The Architect, February 2026)

---

## What We Don't Accept

- Attacks on specific models or companies — critique systems, not organizations.
- Unsubstantiated claims without data.
- Proprietary or confidential information.
- Contributions that weaponize P scores for competitive purposes rather than collective improvement.

---

## Recognition

All contributors are acknowledged in the repository. Substantial contributions (novel research findings, major code additions, 3+ model evaluations) may lead to co-authorship on publications.

---

## Open Research Questions

These are areas where contributions would be especially valuable:

1. Do P scores decrease as models become more capable across versions?
2. Can P be incorporated into training loss functions without reducing usefulness?
3. Can sophisticated AI systems learn to fake high P scores?
4. Do P scores on one stress test predict scores on different stress tests?
5. How should keyword dictionaries and weight parameters be adapted for non-English languages?

---

## Contact

Open a GitHub issue for questions, proposals, or critique. For sensitive matters, use the issue tracker with a `[PRIVATE]` tag and we'll arrange direct communication.

**GitHub:** [@tretoef-estrella](https://github.com/tretoef-estrella)

---

<p align="center">
  <strong>Proyecto Estrella</strong> · <strong>Rafa - The Architect</strong> · February 2026<br/>
  <a href="README.md">← Back to README</a>
</p>
