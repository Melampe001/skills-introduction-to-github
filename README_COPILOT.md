# README_COPILOT.md

This document provides instructions for GitHub Copilot and other automated assistants when working with this repository.

## Required Steps Before Committing

Before committing any changes to this repository, ensure the following steps are completed:

1. **Format your code**: Run `make fmt` to format all code according to the project's style guidelines
2. **Build the project**: Run `make build` to ensure the project builds successfully
3. **Run tests**: Run `make test` to verify all tests pass

These steps help maintain code quality and prevent breaking changes from being introduced.

## Guidance for Proposing Files/Changes

When proposing new files or changes to this repository:

### File Creation
- Place new files in the appropriate directory based on their purpose
- Follow the existing naming conventions
- Include proper file headers and documentation
- Ensure new files are added to relevant build configurations

### Code Changes
- Make minimal, focused changes that address a single concern
- Maintain consistency with existing code style
- Add or update tests to cover new functionality
- Update documentation to reflect changes
- Consider backward compatibility

### Pull Requests
- Create descriptive PR titles that summarize the change
- Include a detailed description explaining what changed and why
- Reference any related issues
- Add appropriate labels (e.g., `docs`, `bugfix`, `enhancement`)

## Minimal PR Checklist

Before submitting a pull request, verify:

- [ ] `make fmt` passes with no further changes
- [ ] `make build` completes successfully
- [ ] `make test` passes all tests
- [ ] Code changes are minimal and focused
- [ ] Documentation is updated if needed
- [ ] PR description clearly explains the changes
- [ ] Appropriate labels are added
- [ ] Reviewers are assigned

## Examples of Good Prompts

When working with GitHub Copilot or other AI assistants, use clear and specific prompts:

### Good Examples

1. **Adding a new feature**:
   ```
   "Add a function to validate email addresses using regex. Include unit tests."
   ```

2. **Refactoring code**:
   ```
   "Refactor the getUserData function to use async/await instead of callbacks."
   ```

3. **Documentation**:
   ```
   "Add JSDoc comments to all public methods in the UserService class."
   ```

4. **Bug fixes**:
   ```
   "Fix the off-by-one error in the pagination logic on line 45 of utils.js."
   ```

### Poor Examples (Avoid)

1. **Too vague**:
   ```
   "Make the code better."
   ```

2. **Too broad**:
   ```
   "Rewrite the entire application using a different framework."
   ```

3. **Unclear intent**:
   ```
   "Fix the thing that's broken."
   ```

## Best Practices

### When Using Copilot
- Write clear comments describing what you want to accomplish
- Review and test all generated code before committing
- Don't blindly accept suggestions - understand what they do
- Use Copilot to accelerate, not replace, your thinking

### Code Quality
- Prioritize readability over cleverness
- Keep functions small and focused
- Use meaningful variable and function names
- Add comments for complex logic, not obvious code

### Testing
- Write tests before or alongside new code
- Aim for meaningful test coverage, not just high percentages
- Test edge cases and error conditions
- Keep tests independent and reproducible

## Repository-Specific Notes

This is a GitHub Skills repository designed to teach GitHub fundamentals. When making changes:

- Preserve the educational structure and flow
- Maintain consistency with GitHub's documentation style
- Keep examples simple and easy to understand
- Ensure changes don't break the learning experience

## Getting Help

If you're unsure about something:
- Review existing code for patterns and conventions
- Check the main README.md for project-specific guidance
- Consult GitHub's documentation at https://docs.github.com
- Ask questions in pull request comments

## Version Information

This document is maintained for automated assistants working with the repository. Last updated: 2025-11-18
