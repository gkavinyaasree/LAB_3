# 🎓 Scholarship Advisory System (Rule-Based)

BSD3513 Introduction to Artificial Intelligence, Lab Report 3.
A transparent decision-support tool that recommends a scholarship outcome
(`AWARD_FULL`, `AWARD_PARTIAL`, `REVIEW`, `REJECT`) using an editable JSON rule base.

**Live app:** <PASTE STREAMLIT URL HERE>

## Features
- Evaluate one applicant and see the decision and every matched rule
- Edit rules live in a JSON editor (invalid JSON falls back to the default rules)
- Priority-based conflict resolution; fallback to `REVIEW` when no rule matches

## How it works
Facts → conditions `[field, operator, value]` → action (decision + reason).
A rule fires only if all conditions are true; the fired rule with the highest priority wins.

## Run locally
```bash
pip install -r requirements.txt
streamlit run StudentID_Lab3.py
```

## Screenshots
<ADD SCREENSHOTS HERE>

## Files
| File | Purpose |
|---|---|
| `StudentID_Lab3.py` | Rule engine and Streamlit UI |
| `requirements.txt` | Dependencies |

## Author
<NAME>, <STUDENT ID>, <SECTION>
