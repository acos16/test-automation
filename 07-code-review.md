## Code Review: A Standard Practice in Software Development

Code review is a standard procedure in software development, aimed at improving code quality, sharing knowledge, and maintaining good practices. When done effectively, it fosters collaboration, catches potential issues early, and enhances team learning.

However, if not approached with commitment and genuine engagement, code reviews can become a superficial checkbox exercise, providing little value. In such cases, alternative practices like pair programming, mob programming, or automated code analysis may be more effective in achieving the same goals while ensuring active participation.

### Goals of Code Review

The primary goal of code review is learning—both for the reviewer and the author. It provides an opportunity to:
 
- Share knowledge about the codebase and practices.
- Identify and fix potential bugs or inefficiencies.
- Ensure code consistency and maintainability.
- Foster team collaboration and mentorship.

Ultimately, the effectiveness of code review depends on the mindset of the team. When done with a focus on learning and improvement, it becomes a powerful tool for building better software and stronger engineering teams.

Tips you can apply when conducting a code review:
- Read the PR description or Jira/issue ticket to understand the purpose of the changes.
- Review code in small chunks: Focus on one section at a time instead of skimming through everything.
- Advocate for smaller PRs that involve changes into just one particular area
- Check for edge cases and unhandled scenarios
- Verify logic and business rules:
  - Ask: "Does this match the expected behavior?"
- Look for nested loops, excessive conditionals, or redundant calculations.
- Suggest simplifications or breaking down large functions into smaller ones.
- Look for sensitive data exposure (e.g., logging passwords, storing secrets in code).
- Verify naming conventions: Suggest better variable/method names.
- Look for robust locators.
- Test the code yourself if possible 
  - Run the code in your local environment. 
  - Experiment with different inputs and scenarios. 
  - Use debugging tools to trace execution and variable values.
- Ensure proper logging and error handling
- Ensure tests follow AAA (Arrange-Act-Assert) and are clear and maintainable.
- Look for errors reported.
  - Static code analysis: code duplication, missing null checks, hardcoded values, uncaught exceptions, race conditions
- Leave comments with explanations, not just “fix this.”
- Use polite language.
- Avoid using commands, offer suggestions
- Avoid offering the exact implementation one should take, offer suggestions.
- If unsure about something, discuss it with the author or team instead of assuming.