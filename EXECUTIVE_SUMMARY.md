# Executive Summary: Model Sourcing Brief — Hub Sourcing Check

**Hub Account:** @lhz7891444 (personal access token, write role, no organization memberships)

## Incumbent Model

- **Model:** google-bert/bert-base-uncased
- **Downloads:** 3,291.4M (3.29 billion)
- **Likes:** 3,066
- **Task:** fill-mask | **Parameters:** 110.1M | **License:** apache-2.0

## Candidate Shortlist (Top 3 BERT-family models, excluding incumbent)

| # | Model Identifier | Downloads | Likes |
|---|---|---|---|
| 1 | google-bert/bert-base-cased | 3.3M | 398 |
| 2 | google-bert/bert-base-multilingual-uncased | 2.0M | 177 |
| 3 | google-bert/bert-base-multilingual-cased | 1.5M | 623 |

## Where Things Live

- **Word brief:** model_sourcing_brief.docx (local workspace: /tmp/mcp_ws/)
- **Snowflake table (fully qualified path):** SEARCH_EVAL_DB.ML_EVALUATIONS.MODEL_SOURCING_EVALUATION
  - One row per model: incumbent + 3 candidates
  - Columns: model_id, downloads, likes
  - Verified row count: 4 rows

## Recommendation

The three shortlisted models have substantial download traction within the BERT family (bert-base-cased leads at 3.3M downloads). Review these candidates against production requirements before the Friday platform review, and refresh the Snowflake table quarterly for ongoing monitoring.
