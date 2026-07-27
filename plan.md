## Solution plan

**Issue:** [issue title and link]

### Understand
What is the root cause of this issue? What behavior is expected vs. actual?

The current API documentation describes the available endpoints, but it does not provide executable `curl` examples that developers can use to test the API from the command line. The expected behavior is for the documentation to include clear, copy-and-paste examples demonstrating how to call the endpoints with the correct HTTP method, headers, and request body.

### Map
Which files, functions, or modules are involved?
List the specific files you expect to touch.
API.md


### Plan
What are the steps to fix this issue?
1. Review `docs/api.md` and identify the endpoints that need `curl` examples.
2. Inspect the API implementation to confirm the correct HTTP methods, URLs, headers, and request body formats.
3. Add complete `curl` examples for the appropriate endpoints using consistent Markdown formatting.
4. Review the updated documentation to ensure the examples are accurate, easy to read, and match the current API implementation.
5. Verify that the documentation renders correctly and that the examples can be copied directly from the page.


### Inputs & outputs
What does your fix take as input? What should it produce or change?
Input :
    - Existing API documentation
    - Endpoint definitions from the backend implementation

Output:
    - Updated API documentation containing complete and accurate `curl` examples for testing the endpoints from the command line.


### Risks & unknowns
What could go wrong? What are you still unsure about?
- Some endpoints may require authentication, so the examples may need placeholder JWT tokens.
- The request body shown in the examples must exactly match the current API schema.
- If endpoint definitions change, the documentation must be updated accordingly.

### Edge cases
What inputs or states should your fix handle gracefully?
- Endpoints that require no request body should have simplified `curl` examples.
- Examples should clearly indicate required headers, such as `Content-Type` and `Authorization`, when applicable.
- Placeholder values (IDs, tokens, usernames, etc.) should be obvious so users know what to replace before running the commands.