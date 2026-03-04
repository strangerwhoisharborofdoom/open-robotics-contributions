# Contributing to Open Robotics Projects

This guide provides step-by-step instructions for contributing to Open Robotics repositories (Gazebo, OSRF, etc.) based on my successful contribution journey.

---

## 🚀 Quick Start Guide

### Step 1: Find Issues to Work On

1. **Visit Open Robotics repositories:**
   - [gazebosim/gz-sim](https://github.com/gazebosim/gz-sim/issues)
   - [gazebosim/gz-math](https://github.com/gazebosim/gz-math/issues)
   - [gazebosim/gz-physics](https://github.com/gazebosim/gz-physics/issues)
   - [osrf/rocker](https://github.com/osrf/rocker/issues)

2. **Filter by labels:**
   - `good first issue` - Perfect for beginners
   - `help wanted` - Actively seeking contributors
   - `documentation` - Great for first contributions
   - `bug` - If you enjoy fixing issues

3. **Look for issues with:**
   - No assignee
   - No linked PR
   - Recent activity (opened/updated in last few months)
   - Clear description

### Step 2: Claim an Issue

1. **Read the issue carefully** - Understand what needs to be done
2. **Check existing PRs** - Make sure no one is already working on it
3. **Add a comment** claiming the issue:

```markdown
Hi! I'm a first-time contributor and I'd like to work on this issue.

Here's my plan:
- [Describe your approach]
- [List specific changes you'll make]
- [Timeline estimate]

Please let me know if there are any specific requirements!
```

4. **Wait for maintainer response** (optional but recommended)

### Step 3: Set Up Development Environment

1. **Fork the repository:**
   - Click "Fork" button on the repository page
   - Wait for fork to complete

2. **Clone your fork:**
```bash
git clone https://github.com/your-username/repository-name.git
cd repository-name
```

3. **Create a branch:**
```bash
git checkout -b fix/issue-number-short-description
# Example: git checkout -b docs/add-friction-tutorial-258
```

### Step 4: Make Your Changes

1. **Follow existing code style:**
   - Match indentation (spaces vs tabs)
   - Follow naming conventions
   - Use same documentation format

2. **For documentation changes:**
   - Use existing Doxygen/comment format
   - Add examples where appropriate
   - Include units for physical quantities
   - Cross-reference related classes/functions

3. **For code changes:**
   - Write clear, readable code
   - Add comments for complex logic
   - Test your changes locally if possible
   - Ensure no breaking changes

4. **Commit your changes:**
```bash
git add changed-file.cpp
git commit -m "type: descriptive message (fixes #issue-number)"

# Examples:
# "docs: Add friction parameters tutorial (fixes #258)"
# "fix: Blender 4.x compatibility in dataset generator (fixes #2588)"
# "feat: Add ROCm extension for AMD GPU support (fixes #326)"
```

### Step 5: Create Pull Request

1. **Push to your fork:**
```bash
git push origin branch-name
```

2. **Create PR on GitHub:**
   - Navigate to your fork
   - Click "Compare & pull request"
   - Ensure base repository is the original (e.g., gazebosim/gz-sim)
   - Ensure base branch is correct (e.g., gz-sim10, gz-physics9)

3. **Write a good PR description:**

```markdown
## Summary
Brief description of what this PR does

## Changes
- List specific changes made
- Reference files modified

## Related Issue
Fixes #issue-number

## Checklist
- [ ] Signed all commits for DCO
- [ ] Added tests (if applicable)
- [ ] Documentation updated
- [ ] CI checks pass
```

4. **Submit the PR**

### Step 6: Respond to Reviews

1. **Watch for notifications** - GitHub will email you about reviews
2. **Address feedback promptly:**
   - Make requested changes
   - Push new commits to the same branch
   - PR updates automatically
3. **Ask questions** if feedback is unclear
4. **Be patient** - Maintainers are volunteers

---

## 📝 Best Practices

### Commit Messages

Use [Conventional Commits](https://www.conventionalcommits.org/) format:
- `docs:` for documentation
- `fix:` for bug fixes
- `feat:` for new features
- `refactor:` for code refactoring
- `test:` for test additions/modifications

### Code Style

- **C++ projects:** Follow existing Doxygen comment style
- **Python projects:** Use type hints and docstrings
- **Markdown:** Use consistent heading levels and formatting

### Communication

- Be polite and professional
- Thank reviewers for their time
- Explain your reasoning when asked
- Don't take criticism personally - it's about the code

---

## 🎯 Contribution Ideas by Skill Level

### Beginner (First Contribution)
- Fix typos in documentation
- Improve existing documentation clarity
- Add examples to API docs
- Report bugs with detailed reproduction steps

### Intermediate
- Add new tutorials
- Fix compatibility issues (like Blender 4.x)
- Improve error messages
- Add unit tests for uncovered code

### Advanced
- Implement new features
- Refactor complex code sections
- Optimize performance-critical code
- Create new extensions/plugins

---

## 🔧 Tools You'll Need

### Essential
- Git and GitHub account
- Text editor (VS Code, CLion, etc.)
- C++ compiler (for gz-* projects)
- Python 3 (for rocker, scripts)

### Helpful
- Doxygen (for building docs locally)
- Docker (for testing rocker extensions)
- Gazebo simulator (for testing)
- Blender (for dataset generation)

---

## 📚 Resources

### Documentation
- [Gazebo Documentation](https://gazebosim.org/)
- [SDF Specification](https://sdformat.org/)
- [Open Robotics Contribution Guidelines](https://osrf.github.io/)

### Community
- [Gazebo Forum](https://community.gazebosim.org/)
- [ROS Discourse](https://discourse.ros.org/)
- [GitHub Discussions](https://github.com/gazebosim)

### My Contributions (Examples)
- [Friction Parameters Tutorial](https://github.com/gazebosim/gz-physics/pull/886)
- [ROCm Extension](https://github.com/osrf/rocker/pull/353)
- [API Documentation Plan](https://github.com/gazebosim/gz-math/pull/719)

---

## ❓ FAQ

**Q: How long does PR review take?**
A: Typically 1-2 weeks, but can vary based on maintainer availability.

**Q: Can I work on multiple issues?**
A: Yes! Just make sure to create separate branches and PRs for each.

**Q: What is DCO?**
A: Developer Certificate of Origin - you agree to it by signing your commits with `-s` flag.

**Q: My PR has failing checks. What do I do?**
A: Click on the check details to see what failed. Fix the issues and push new commits.

**Q: Can I contribute without being an expert?**
A: Absolutely! Documentation, testing, and bug reports are valuable contributions too.

---

## 🌟 Tips for Success

1. **Start small** - Your first PR doesn't need to be huge
2. **Be consistent** - Regular contributions build reputation
3. **Learn from others** - Read existing PRs to understand the process
4. **Ask for help** - Maintainers are generally helpful
5. **Don't give up** - Revisions are normal and make the project better

---

## 🎉 Your Contribution Journey Starts Here!

Remember: Every expert was once a beginner. Your contributions, no matter how small, help make Open Robotics better for everyone.

Good luck, and welcome to the open source community! 🚀

---

*Based on my journey contributing 6+ PRs to Open Robotics repositories (gz-sim, gz-math, gz-physics, rocker) as a first-year Robotics Engineering student.*

*Last Updated: March 4, 2026*
