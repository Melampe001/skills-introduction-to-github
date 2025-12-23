# README for GitHub Copilot and Automated Assistants

This document provides guidance for GitHub Copilot and other automated assistants when working with this repository.

## Repository Context

This is a GitHub Skills learning repository designed to teach users about GitHub fundamentals including branches, commits, and pull requests. The repository is primarily educational and contains:

- Tutorial content in README.md
- GitHub Actions workflows for course progression
- Educational images and resources

## Guidelines for Automated Assistants

### Before Making Changes

1. **Understand the Educational Purpose**: This repository is designed for learning. Any changes should maintain the educational value and not interfere with the learning experience.

2. **Review Existing Structure**: 
   - Check the current step in the README.md
   - Review .github/workflows for automation
   - Understand the tutorial flow before proposing changes

3. **Minimal Changes**: Make only the changes necessary to address the specific issue or task. This is a learning repository, so simplicity is key.

### Proposing Changes

When suggesting files or code changes:

1. **Documentation Changes**:
   - Keep language simple and beginner-friendly
   - Maintain the existing tutorial structure
   - Use clear, concise explanations

2. **Workflow Changes**:
   - Test workflows carefully to avoid breaking the learning experience
   - Ensure new workflows don't interfere with existing course progression
   - Document any new automation clearly

3. **Content Changes**:
   - Maintain consistency with GitHub's educational materials
   - Use appropriate markdown formatting
   - Include helpful images or examples where relevant

### Pull Request Checklist

Before submitting a pull request:

- [ ] Changes align with the educational purpose of the repository
- [ ] Documentation is clear and beginner-friendly
- [ ] No breaking changes to existing tutorials or workflows
- [ ] Commit messages are descriptive and follow conventions
- [ ] Changes are minimal and focused on the specific task

### Example Prompts for Good Interactions

**Good prompts:**
- "Add a new section to README.md explaining how to create a pull request"
- "Fix the typo in the branch creation instructions"
- "Update the workflow to support a new learning step"

**Less helpful prompts:**
- "Rewrite the entire tutorial" (too broad)
- "Add complex CI/CD pipelines" (not aligned with educational purpose)
- "Remove all images" (breaks the tutorial experience)

## Repository-Specific Notes

- This repository uses GitHub Actions to automatically progress users through the course
- The README.md file is dynamically updated by workflows based on user actions
- Images are stored in the `images/` directory and referenced in tutorials
- The repository follows a step-by-step learning progression

## Getting Help

For questions or issues:
- Review the [GitHub Skills discussions](https://github.com/orgs/skills/discussions)
- Check the [GitHub documentation](https://docs.github.com)
- Open an issue in this repository for course-specific problems

## License

This repository follows the MIT License. See LICENSE file for details.

---

**Note to Automated Assistants**: When in doubt, prioritize the learning experience of users going through this tutorial. Keep changes simple, well-documented, and aligned with GitHub's educational goals.
