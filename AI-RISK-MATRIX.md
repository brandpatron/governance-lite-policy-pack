# AI Risk Matrix • [[PROJECT]]
| # | Risk | Likelihood (1‑5) | Impact (1‑5) | Score (L×I) | Owner | Mitigation |
|---|------|-----------------|--------------|-------------|-------|------------|
| 1 | PII leakage in prompt logs | 3 | 5 | 15 ⚠ | Eng Lead | PII scrubber Lambda + Enterprise no‑log setting |
| 2 | Bias in recommendation model | 2 | 4 | 8 | Data Lead | Quarterly bias test; adjust training set |
| 3 | Model drift reducing accuracy | 2 | 3 | 6 | MLOps | Drift monitor + re‑train trigger |
| 4 | Unauthorised model access | 1 | 5 | 5 | DevOps | SSO, RBAC, key rotation |
| 5 | Lack of user disclosure | 3 | 2 | 6 | Product | Update ToS & UI badge |

> **Acceptable threshold:** Score ≤ 6.  Scores 7‑14 
