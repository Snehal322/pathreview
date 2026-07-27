## Week 7 — Issue selection

**Issue link:**  https://github.com/ascherj/pathreview/issues/117

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
I reproduced Issue by reviewing `docs/api.md` and confirming that the API documentation lists the available endpoints but does not include any executable `curl` examples. This matches the issue description, as developers currently have no ready-to-run command-line examples for testing the API.

**PLAN.md link:**
https://github.com/Snehal322/pathreview/blob/fix/117-curl-eg-missing--API-testing/PLAN.md

**Walkthrough video (recommended):** Not recorded

**Blockers or open questions:**
None