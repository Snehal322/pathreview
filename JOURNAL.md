## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/117 

**Issue title:** API docs don't include example curl commands

**Tier:** [Y] Tier 1  [ ] Tier 2  [ ] Tier 3

**Problem summary:**
The issue is requesting that the API documentation include a working `curl` example so developers can easily test the endpoint from the command line. Currently, the documentation explains the endpoint but does not provide a complete example request, making it harder to verify the API without using another tool. The change affects the project's documentation. A successful fix will add a clear, correct `curl` example that users can copy and run directly.


**Branch name:** fix/117-curl-eg-missing--API-testing

**Setup confirmation:** [Y] App runs locally at localhost:5173

**Cohort ledger:** [Y] Issue added to cohort ledger


## Week 8 — Reproduction & solution planning

**Reproduction commit link:** https://github.com/Snehal322/pathreview/commit/974c7ae

**Reproduction summary:**
I reproduced the documentation issue by reviewing docs/api.md and confirming that it lists API endpoints but provides no executable curl examples. This matches Issue #117 because developers currently cannot copy and run example requests directly from the documentation.

**PLAN.md link:**
https://github.com/Snehal322/pathreview/blob/fix/117-curl-eg-missing--API-testing/PLAN.md

**Walkthrough video (recommended):** Not recorded

**Blockers or open questions:**
None

## Week 9 - Solution building & PR submission

Check-in 1 (mid-week)

Current progress:
Implemented the API documentation updates for Issue #117. The documentation now covers the available API endpoints, authentication requirements, request examples, successful responses, and error responses. I also ran the existing test suite and identified pre-existing failures unrelated to the API documentation work.

Next steps:
Run make check and make test-unit after the documentation changes, compare the results with the baseline, complete the self-review, and request peer feedback on the draft PR.

Blockers:
The existing unit-test suite contains pre-existing failures in unrelated application components. These are outside the scope of Issue #117.