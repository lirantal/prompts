## Prompt for pasting instructions manually via interactive session

Your purpose is to build a an instructions files for AI agents (also known as a "rules file", like Cursor rules, and CLAUDE.md files) that will be exclusively used for the topic of generating test code for modern Node.js applications.

Your guideline for building the rules file is as follows:
- The rules file should be written in Markdown format.
- The rules file should be descriptive, repeatable, and helpful.

Your guideline for test code style is as follows:
- Test code should explicitly be focused on generating test code for modern Node.js runtime version v22 and above.
- Test code should explicitly be based on the latest JavaScript standards, including ES2022 and beyond.
- Test code should explicitly and solely rely only on the built-in Node.js test runner and testing framework which is `node:test` and `node:assert`, and any built-in Node.js APIs as needed such as `node:util`.
- You can and *should* invoke the `nodejs-api-docs` MCP tools available for you to retrieve up-to-date information about the Node.js APIs.
- You should extract meaningful testing strategy insights from the test code you analyze such as test structure, naming conventions, assertions, mocking and stubbing practices, the use of setup and teardown methods, and the use of test fixtures.
- You do not need to replace or favor just one test code style over another when both (or more) are valid test code mechanisms and do not conflict with each other. For example, asserting on a strict text and asserting on text by using a regex are complementary
- When categorization is applicable, you should categorize instructions into sections such as "Testing Web Servers and APIs", "Testing Commands and CLI Tools". Categorize everything else that is high-level testing principles into the category "General Testing Principles".
- DO NOT rely on project specific helpers or utils for test code, instead your instructions should focus on higher-level testing strategy.
- The rules file should include canonical code snippets for examples and references as needed.

To perform the above, you will need this context and action to follow on:
- Context: The current directory already contains a basic `INSTRUCTIONS.md` file as a starting point, which you should enhance and refine.
- Action: Review, analyze and then apply all of the test code style, testing principles and test code insights that you can extract from the test code that I will provide you in the next step.

Tell me when you are ready to proceed and I will begin pasting the test code for you to analyze and extract insights from.


## Prompt for using directory as reference

Your purpose is to build a an instructions files for AI agents (also known as a "rules file", like Cursor rules, and CLAUDE.md files) that will be exclusively used for the topic of generating test code for modern Node.js applications.

Your guideline for building the rules file is as follows:
- The rules file should be written in Markdown format.
- The rules file should be descriptive, repeatable, and helpful.

Your guideline for test code style is as follows:
- Test code should explicitly be focused on generating test code for modern Node.js runtime version v22 and above.
- Test code should explicitly be based on the latest JavaScript standards, including ES2022 and beyond.
- Test code should explicitly and solely rely only on the built-in Node.js test runner and testing framework which is `node:test` and `node:assert`, and any built-in Node.js APIs as needed such as `node:util`.
- You can and *should* invoke the `nodejs-api-docs` MCP tools available for you to retrieve up-to-date information about the Node.js APIs.
- You should extract meaningful testing strategy insights from the test code you analyze such as test structure, naming conventions, assertions, mocking and stubbing practices, the use of setup and teardown methods, and the use of test fixtures.
- You do not need to replace or favor just one test code style over another when both (or more) are valid test code mechanisms and do not conflict with each other. For example, asserting on a strict text and asserting on text by using a regex are complementary.
- When categorization is applicable, you should categorize instructions into sections such as "Testing Web Servers and APIs", "Testing Commands and CLI Tools". Categorize everything else that is high-level testing principles into the category "General Testing Principles".
- DO NOT rely on project specific helpers or utils for test code, instead your instructions should focus on higher-level testing strategy.
- The rules file should include canonical code snippets for examples and references as needed.

To perform the above, you will need this context and action to follow on:
- Context: You are currently within a directory for a Node.js application code repository that uses good testing practices. The `INSTRUCTIONS.md` file in this directory is already well-structured and contains useful information that is your base starting point and you should enhance and refine it as required.
- Action: Review, analyze and then apply all of the test code style, testing principles and test code insights that you can extract from the test code in this directory (hint: test files exist in `test` directory) to build the rules file.
