# Responsible‑AI Policy • [[PROJECT]]
_Last updated: {{DATE}}_

## 1 Purpose
Ensure all AI‑driven features of **[[PROJECT]]** are fair, transparent, privacy‑preserving and aligned with EU AI Act & NDPA 2023.

## 2 Principles
1. **Human Oversight** – A qualified reviewer (see §5) can override or roll back any automated decision.
2. **Data Minimisation** – Process the least personally identifiable data necessary.
3. **Explainability** – Provide end‑users a concise explanation of how AI outputs are generated or used.
4. **Bias Mitigation** – Run bias tests every major release; thresholds defined in Risk Matrix.
5. **Security by Design** – All prompts, logs and model artefacts encrypted in transit and at rest.

## 3 Governance Roles
| Role | Name | Responsibility |
|------|------|----------------|
| Data Protection Officer | [[DPO_NAME]] | DPIA, breach notification |
| AI Risk Lead | [[PM_NAME]] | Maintains risk matrix |
| Incident Commander | [[ENG_MANAGER]] | Triggers incident plan |

## 4 Data Flow & Storage
Refer to `docs/data-flow.svg`. All user PII stored in AWS eu-west‑3; model prompts scrubbed of PII.

## 5 Human Oversight Procedure
1. Flag from API / user report → Slack `#ai-review`.<br>2. Reviewer checks logs + user context.<br>3. If output harmful, rollback release via CI and note in ChangeLog.<br>4. File lessons learned in Retrospective doc.

## 6 Review Cycle
- Weekly: automated metric scan (drift, bias).  
- Quarterly: full policy refresh & stakeholder
