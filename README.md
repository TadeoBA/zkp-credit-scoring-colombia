# ZKP-Based Credit Scoring — Colombia

## Research Overview
Master's thesis — Universidad de La Sabana  
**Research Question:** Can a predictive analytics pipeline for credit scoring 
substitute raw personal data with Zero-Knowledge Proof attestations, maintaining 
acceptable precision, and under what conditions would this configure functional 
equivalence under Colombian data protection law (Law 1581/2012)?

**Researcher:** Tadeo Bayona Araque — Lawyer (7 yrs) + MSc Applied Analytics (in progress)  
**Institution:** Universidad de La Sabana, Bogotá, Colombia  

---

## PoC Status — Semester 1
| Milestone | Status | Date |
|---|---|---|
| ZoKrates 0.8.8 environment verified | ✅ Complete | 2026-03-25 |
| Income threshold circuit compiled (763 constraints) | ✅ Complete | 2026-03-25 |
| Client-side proof generation verified | ✅ Complete | 2026-03-25 |
| Verification result | ✅ PASSED | 2026-03-25 |
| Full scoring pipeline (Pipeline A vs B) | 🔨 Semester 2 | — |
| Legal equivalence framework | 🔨 Semester 2 | — |

---

## Architecture
**Client-side proving** — the prover (data subject) generates the ZKP locally.  
The receiving entity (financial institution) never processes raw personal data.  
Only the attestation is transmitted.

---

## Stack
- **ZKP:** ZoKrates 0.8.8 (Docker)
- **ML:** Python / Scikit-learn (Semester 2)
- **Legal framework:** Law 1581/2012 + Law 527/1999 (functional equivalence)
- **Regulator:** Superintendencia de Industria y Comercio (SIC)

---

## Legal Framework
This research applies the **functional equivalence** principle — established in 
Colombian Law 527/1999 for electronic signatures — to argue that ZKP attestations 
can satisfy the same regulatory function as raw personal data under Law 1581/2012.
