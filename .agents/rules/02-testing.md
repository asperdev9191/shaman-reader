# CRITICAL RULE: TEST-DRIVEN DEVELOPMENT (TDD)
1. NO BLIND CODE: You must write a failing unit test in the `test/` directory BEFORE implementing the production logic.
2. VERIFICATION GATE: After writing production code, you MUST execute `flutter test <filename>` in the terminal.
3. FAILURE PROTOCOL: If the test fails, you are authorized to read the logs and rewrite the code. Do NOT prompt the user for help unless the test fails 3 times in a row.
4. ARTIFACT REQUIREMENT: You cannot mark a task as "Complete" without attaching the terminal output showing passing tests.
