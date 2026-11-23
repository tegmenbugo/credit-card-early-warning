# Credit Card Early Warning & Limited Review Capacity Optimization

> **Graduation Project** — Management Information Systems (English), Istanbul University
> Course: *From Idea to MVP* (Sept 2026 – Mar 2027)

[![Status](https://img.shields.io/badge/status-field%20validation%20complete-blue)]()
[![License](https://img.shields.io/badge/license-TBD-lightgrey)]()

---

## 👤 Author

**Battal Buğra Karataş**

- 📧 [karatasbugra26@gmail.com](mailto:karatasbugra26@gmail.com)
- 💼 [LinkedIn](https://www.linkedin.com/in/battalbugrakaratas/)

**Advisor:** Assoc. Prof. Dr. Gökhan Övenç

---

## 📌 Project Status

| Phase | Status |
|---|---|
| Field validation & value proposition | ✅ Complete |
| Solution design | 🔜 Starts December 2026 |
| Prototyping & MVP | ⬜ Planned |
| Code / model / dashboard | ⬜ Not started |

> **Note:** This repository currently contains only project documentation. No code, model, or dashboard exists yet. Development will begin after the solution design phase.

---

## 🔍 The Problem

Credit monitoring and early collections teams in banks receive more early-warning signals every day than they can review or call. Existing risk scores rank customers by **probability of default (PD)**, not by the **value of intervening**.

As a result:

- Limited staff time goes to customers who would **pay anyway** (self-cure) or **cannot be recovered regardless**, while high-exposure accounts slip into later delinquency buckets (1–30 → 31–60 → 61–90 → 90+ days).
- A delayed **limit freeze** lets customers draw the remaining credit limit as cash, increasing **exposure at default (EAD)**.
- This drives up **credit losses**, **IFRS 9 provisions**, and **legal costs**.

---

## 🎤 Field Validation

> *All findings are anonymized. No individuals, banks, or companies are identified.*

**7 interviews** were conducted with professionals across banking, credit risk, fintech, internal audit, and insurance recovery.

### Key Findings

1. **The real user is the Credit Monitoring / Early Collections team**, not the risk-modeling department.
2. **Static PD scores are insufficient** — they cannot distinguish customers who will self-cure from those who will not pay regardless, so effort is wasted on both groups.
3. **Delayed limit freezes increase exposure** — customers can draw remaining credit as cash advances before the freeze takes effect, raising EAD.
4. **Capacity bottlenecks are cyclical** — they recur at month-end, salary periods, and after statement cut-off dates.
5. **The same capacity problem exists in insurance recovery teams**, where it is currently handled on an ad-hoc basis.

---

## 💡 Planned Solution

> ⚠️ **Everything described below is planned, not built.** Solution design starts in December 2026.

A **transparent decision-support dashboard** that tells the early collections team *whom to contact first*, *through which channel*, and *how much exposure that protects*.

### Planned Features

| Feature | Description |
|---|---|
| **Daily contact list** | Capped at team capacity (e.g., 200 files/day), ranked by **expected exposure protected** (PD × exposure), not by PD alone. |
| **Channel routing** | Likely self-cure, low-balance accounts → automated SMS/IVR; staff calls reserved for high-exposure accounts. |
| **Limit-freeze alerts** | Flags accounts with high unused credit limit and rising utilization for proactive limit action. |
| **What-if capacity simulator** | Lets team leads test scenarios: *"What if we add 2 FTEs?"* or *"What if call volume doubles at month-end?"* |

### How It Differs from Existing Approaches

```
Traditional approach:    Rank by PD → Call the "riskiest" customers
                         ❌ Wastes effort on self-cure and unrecoverable accounts

Planned approach:        Rank by expected exposure protected → Call where intervention matters most
                         ✅ Maximizes recovered exposure per unit of staff capacity
```

---

## 🗓️ Roadmap

| Period | Milestone |
|---|---|
| Sept – Nov 2026 | Field validation & value proposition |
| Dec 2026 | Solution design |
| Jan – Feb 2027 | Prototyping & MVP development |
| Mar 2027 | Final presentation |

---

## 📄 License

TBD

---

<sub>Istanbul University · Management Information Systems · 2026–2027</sub>
