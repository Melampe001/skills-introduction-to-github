# README_COPILOT.md

This document provides instructions for GitHub Copilot and other automated assistants when working with this repository.

## Required Steps Before Committing

Before committing any changes to this repository, ensure the following steps are completed:

1. **Review your changes**: Use `git diff` to review all modifications
2. **Check workflow files**: If modifying `.github/workflows/`, validate YAML syntax
3. **Preview markdown**: Ensure README.md and other documentation renders correctly
4. **Test tutorial flow**: Verify that changes don't break the learning experience

This repository uses GitHub Actions workflows (`.github/workflows/`) for automation. There are no build or test commands since this is a documentation-based tutorial repository.

## Guidance for Proposing Files/Changes

When proposing new files or changes to this repository:

### File Creation
- Place documentation files in the repository root
- Place images in the `/images/` directory
- Place workflow files in `.github/workflows/`
- Follow existing naming conventions (kebab-case for workflows, UPPERCASE for special docs)
- Include proper markdown headers and formatting

### Documentation Changes
- Make minimal, focused changes that address a single concern
- Maintain consistency with existing documentation style
- Keep language simple and beginner-friendly
- Update related documentation if needed
- Verify markdown rendering and links

### Workflow Changes
- Validate YAML syntax before committing
- Test changes thoroughly to avoid breaking the tutorial
- Document what the workflow does and why changes were made
- Consider backward compatibility with existing learner progress

### Pull Requests
- Create descriptive PR titles that summarize the change
- Include a detailed description explaining what changed and why
- Reference any related issues
- Add appropriate labels (e.g., `docs`, `workflows`, `enhancement`)

## Minimal PR Checklist

Before submitting a pull request, verify:

- [ ] Changes are minimal and focused
- [ ] Markdown documentation renders correctly
- [ ] Workflow YAML files are valid (if modified)
- [ ] Tutorial steps flow logically
- [ ] Images and links work properly
- [ ] PR description clearly explains the changes
- [ ] Appropriate labels are added (e.g., `docs`, `workflows`)
- [ ] Reviewers are assigned

## Examples of Good Prompts

When working with GitHub Copilot or other AI assistants, use clear and specific prompts:

### Good Examples

1. **Updating documentation**:
   ```
   "Update README.md step 2 to clarify branch creation instructions."
   ```

2. **Modifying workflows**:
   ```
   "Add a new workflow validation step to check YAML syntax in .github/workflows/."
   ```

3. **Improving tutorial content**:
   ```
   "Add a new section to explain pull request reviews in simple terms for beginners."
   ```

4. **Fixing broken links**:
   ```
   "Fix the broken image link in README.md line 45 that points to /images/example.png."
   ```

### Poor Examples (Avoid)

1. **Too vague**:
   ```
   "Make the tutorial better."
   ```

2. **Too broad**:
   ```
   "Rewrite all the documentation using different examples."
   ```

3. **Unclear intent**:
   ```
   "Fix the workflow that's broken."
   ```

## Best Practices

### When Using Copilot
- Write clear comments describing what you want to accomplish
- Review all generated content before committing
- Don't blindly accept suggestions - understand what they do
- Use Copilot to accelerate, not replace, your thinking

### Documentation Quality
- Prioritize clarity and simplicity for beginners
- Use proper markdown formatting
- Include screenshots and examples where helpful
- Keep language accessible and jargon-free

### Workflow Modifications
- Validate YAML syntax before committing
- Test workflow changes in a fork first if possible
- Document any changes to workflow behavior
- Consider impact on learner experience

## Repository-Specific Notes

This is a GitHub Skills repository designed to teach GitHub fundamentals. When making changes:

- **Tutorial Structure**: This repository uses GitHub Actions workflows in `.github/workflows/` to guide learners through steps
- **No Build Process**: This is a documentation-only repository with no code to compile or test
- **Workflow Files**: Changes to `.github/workflows/*.yml` should be carefully validated for YAML syntax
- **Step Files**: The `.github/steps/` directory contains step metadata used by workflows
- **Educational Focus**: Preserve the educational structure and flow
- **Documentation Style**: Maintain consistency with GitHub's documentation style
- **Simple Examples**: Keep examples simple and easy to understand for beginners
- **Learning Experience**: Ensure changes don't break the tutorial flow or confuse learners

## Getting Help

If you're unsure about something:
- Review existing code for patterns and conventions
- Check the main README.md for project-specific guidance
- Consult GitHub's documentation at https://docs.github.com
- Ask questions in pull request comments

## Version Information

This document is maintained for automated assistants working with the repository. Last updated: 2025-11-18
