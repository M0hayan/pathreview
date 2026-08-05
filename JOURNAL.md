## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/117

**Issue title:** API docs don't include example curl commands
 

**Tier:** [ O ] Tier 1  [  ] Tier 2  [  ] Tier 3

**Problem summary:**
[the api.md file contains information about the endpoints but there is no mention of examples to call it. This issue causes users to be unable to easily test that the api is working as intended. After I fix the issue the documentation should have the updated curl commands so that users can validate the api easily.]

**Branch name:** [docs/117-add-example-curl]

**Setup confirmation:** [ O ] App runs locally at localhost:5173

**Cohort ledger:** [ O ] Issue added to cohort ledger

## Reproducing issue Locally
After reading the api.md file in the docs file, I confirmed that the issue persisted as there is no examples of any curl commands.

## Week 8 — Reproduction & solution planning

**Reproduction commit link:** [https://github.com/M0hayan/pathreview/commit/d95b4aae625c89353e658bca3fb8526dd8915f03]

**Reproduction summary:**
[I had to clone the repo locally and take the steps so that the app was working as intended. Then I read through the documentation and confirmed that there are no example curl commands in the api.md file.]

**PLAN.md link:** [https://github.com/M0hayan/pathreview/blob/docs/117-add-example-curl/PLAN.md]

**Walkthrough video (recommended):** []

**Blockers or open questions:**
[]

## Week 9 — Solution building & PR submission

### Check-in 1 (mid-week)

**Current progress:**
Updated `docs/API.md` to include example `curl` commands for the documented API endpoints. Reviewed the FastAPI route implementations to verify the correct request formats, authentication requirements, and endpoint behavior.

Completed sub-tasks:
- Reviewed existing API documentation and identified missing invocation examples.
- Verified endpoint methods, paths, and request formats against the API implementation.
- Added examples for Health, Authentication, Profiles, and Reviews endpoints.
- Documented required placeholders such as `<token>`, `<profile_id>`, and `<review_id>`.

**Next steps:**
- Review the updated documentation for formatting and accuracy.
- Run any required project checks before opening the PR.
- Submit the pull request and address any reviewer feedback.

**Blockers:**
None.

### Check-in 2 (end of week)

**PR link:** [(https://github.com/ascherj/pathreview/pull/931)]

**Branch:** `docs/117-api-example-invocations`

**What you built:**
Updated `docs/API.md` with runnable `curl` examples for the API endpoints so new developers can quickly verify the service is working. The examples were aligned with the actual FastAPI implementation, including OAuth2 form-based login, multipart profile creation, and authenticated requests using bearer tokens.

**Tests added or updated:**
None. This was a documentation-only change, so no application behavior was modified and no unit tests were required.

**Self-review confirmation:**  
[ O ] make check passes  
[ O ] make test-unit passes  

**Draft PR feedback received from:** none
