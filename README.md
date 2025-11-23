# 🛡️ CodeGuard CLI

**Securing the future of AI-assisted development — one line at a time.**

CodeGuard is a lightweight security and quality scanner built specifically for **AI-generated code**. It detects LLM-style code patterns, analyzes vulnerabilities, and evaluates maintainability — before the code ships or gets merged.

---

## 🚀 Features

- **AI Code Detection** — Probability-based classifier for AI-generated code.
- **Security Scanning** — OWASP Top 10 + AI-specific vulnerability checks.
- **Code Quality Metrics** — Complexity, duplication, maintainability score.
- **CI/CD Ready** — Machine-readable output formats (JSON, SARIF).

---

## 📦 Install *(WIP)*

```bash
npm install -g codeguard
````

---

## 🧪 Usage

```bash
codeguard scan ./src
```

With output formatting:

```bash
codeguard scan ./src --format json --ai-detect
```

---

## 📊 Example Output

```json
{
  "ai_generated_probability": 0.82,
  "security_risks": [
    { "rule": "SQL Injection", "file": "db/login.js", "severity": "high" }
  ],
  "quality_score": 67
}
```

---

## 🧭 Roadmap

* [ ] Python + JS/TS + Go scanning
* [ ] Custom linting + rules engine
* [ ] Web dashboard + historical view
* [ ] GitHub Action & CI gating policy

---

## 📌 Status

Early MVP in development — expect breaking changes.

---
