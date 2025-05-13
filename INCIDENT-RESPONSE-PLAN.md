# AI & Data Incident Response Plan • [[PROJECT]]

### 1 Trigger Criteria
- PII exposure OR
- Harmful or unlawful model output in production OR
- Security breach of model weights / prompts.

### 2 Response Timeline (aligned to GDPR/NDPA 72‑h rule)
| T + | Action | Owner |
|-----|--------|-------|
| 0 h | Detect & log incident in Jira “AI‑INC” project | Detector |
| 1 h | Notify Incident Commander & DPO | Auto bot |
| 4 h | Contain: disable endpoint / feature flag | IC |
| 12 h | Root‑cause analysis started | IC + Eng |
| 24 h | Draft regulator & stakeholder notice | DPO |
| 72 h | Final notice sent; mitigation plan approved | Exec sponsor |

### 3 Communication Channels
- Slack `#incident-warroom` (private)  
- Email alias: incident@brandxpatron.com  
- Status page: status.brandxpatron.com

### 4 Post‑Mortem
Within 5 business days: write doc, tag “prevent‑
