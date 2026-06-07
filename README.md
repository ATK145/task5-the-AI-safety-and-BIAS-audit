# 🛡️ AI Safety & Bias Audit Report — DecodeLabs Task 5

> **A comprehensive red-teaming exercise, bias analysis, and guardrail framework for responsible AI deployment.**

![DecodeLabs](https://img.shields.io/badge/DecodeLabs-AI%20Safety%20Audit-4a9eff?style=for-the-badge)
![Task](https://img.shields.io/badge/Task-5%20of%205-ff3b5c?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-2ecc71?style=for-the-badge)

---

## 📋 Overview

This project is **Task 5** of the DecodeLabs AI Bootcamp portfolio. It documents a structured AI Safety & Bias Audit conducted through:

- **Red Teaming** — 47 adversarial prompts across 6 attack categories to test jailbreak resistance
- **Bias Audit** — Systematic evaluation of gender, racial, and cultural bias in AI outputs
- **SHIELD Framework** — A 5-layer guardrail architecture proposal for production deployment

---

## 🚀 Live Demo

**[View the Audit Report →](https://YOUR-USERNAME.github.io/ai-safety-audit/)**

---

## 📂 Project Structure

```
ai-safety-audit/
├── index.html          # Main audit report (single-page)
├── css/
│   └── style.css       # Styling & design system
├── js/
│   └── main.js         # Animations & interactivity
└── README.md           # This file
```

---

## 🔍 Key Findings

| Attack Vector | Success Rate | Severity |
|---|---|---|
| Role-Play Hijack (DAN) | 12% | HIGH |
| Hypothetical Framing | 40% | MEDIUM |
| Prompt Injection via Docs | **67%** | **CRITICAL** |
| Gradual Escalation | 37% | MEDIUM |
| Authority Impersonation | 0% | LOW |
| Token Smuggling / Encoding | **63%** | **CRITICAL** |

**Bias Detection Rates:**
- Gender Stereotyping: **71%** of neutral prompts
- Racial Representation Bias: **64%**
- Occupational Stereotyping: **78%**
- Western Cultural Centrism: **55%**

---

## 🏗️ SHIELD Framework (5-Layer Defense)

```
👤 User → [L1 Input Sanitizer] → [L2 System Prompt] → 🤖 LLM → [L3 Output Filter] → ✅ Safe Output
                   ↕ L4: Conversation Monitor ↕ L5: Bias Audit Pipeline
```

| Layer | Purpose |
|---|---|
| L1 | Input sanitization, encoding detection, prompt injection scanning |
| L2 | System prompt hardening, identity anchoring, permission hierarchy |
| L3 | Output classification, medical/legal filter, bias flagging |
| L4 | Conversation-level risk scoring, escalation detection |
| L5 | Continuous automated bias testing, human review pipeline |

---

## 🛠️ Technologies Used

- **HTML5** — Semantic structure
- **CSS3** — Custom properties, Grid, Flexbox, animations
- **Vanilla JavaScript** — IntersectionObserver animations, typing effects, counter animations
- **Google Fonts** — Syne (display), Space Mono (code), DM Sans (body)

---

## 📚 References

- [OWASP LLM Top 10](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [Universal Adversarial Attacks on LLMs — Zou et al.](https://arxiv.org/abs/2307.15043)
- [Google Responsible AI Practices](https://ai.google/responsibility/responsible-ai-practices/)
- [Fairlearn Toolkit](https://fairlearn.org/)
- [IBM AI Fairness 360](https://aif360.mybluemix.net/)
- [Anthropic Constitutional AI](https://www.anthropic.com/news/constitutional-ai-harmlessness-from-ai-feedback)

---

## 🚀 Deploy to GitHub Pages

```bash
# 1. Create repo on GitHub named: ai-safety-audit
# 2. Push this folder:
git init
git add .
git commit -m "feat: AI Safety & Bias Audit Report — Task 5"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/ai-safety-audit.git
git push -u origin main

# 3. Enable GitHub Pages:
#    Settings → Pages → Source: main branch → / (root) → Save
#    Live at: https://YOUR-USERNAME.github.io/ai-safety-audit/
```

---

## 👤 Author

**[Your Name]** — DecodeLabs AI Bootcamp  
📧 your.email@example.com  
🔗 [LinkedIn](https://linkedin.com/in/yourprofile) | [GitHub](https://github.com/YOUR-USERNAME)

---

## 📄 License

MIT License — Feel free to use and adapt for educational purposes.

---

*© 2025 DecodeLabs · AI Safety & Bias Audit · Task 5*
