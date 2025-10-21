# Contributing to Fusion Party

Thank you for your interest in contributing to Fusion Party's technical infrastructure! This document outlines our standards, processes, and guidelines for contributing to any repository in the Fusion Party GitHub organisation.

---

## 🎯 Repository Naming Conventions

To maintain clarity and consistency across our organisation, follow these naming standards when creating new repositories:

### Format: `{category}-{name}`

Use **kebab-case** (lowercase with hyphens) for all repository names.

### Categories

- **`website-`** — Website themes, pages, and frontend code
- **`tools-`** — Utilities, scripts, and developer tools
- **`docs-`** — Documentation, guides, and resources
- **`campaign-`** — Campaign-specific materials and code
- **`policy-`** — Policy documents and research
- **`event-`** — Event management systems
- **`data-`** — Data processing and analysis tools
- **`api-`** — API integrations and interfaces

### Examples

✅ **Good:**
- `website-theme-2024` — Current NationBuilder theme
- `tools-electorate-maps` — Electorate boundary processing
- `api-nationbuilder-python` — Python interface for NationBuilder
- `campaign-yarra-council` — Yarra Council campaign theme
- `tools-aec-checker` — AEC membership verification tool
- `event-management` — Event registration system
- `docs-technical` — IT systems documentation

❌ **Bad:**
- `colourful_fusion_theme` — Uses underscores, unclear category
- `emu` — Too vague, no category
- `FusionPolicy` — PascalCase, no category
- `Fusion-Party-Aus.github.io` — Special case (GitHub Pages), but generally avoid

### Special Cases

- **`.github`** — Organisation-wide settings and profile (mandatory name)
- **`fusion-party.github.io`** — GitHub Pages site (mandatory format)

## 🔧 Repository Setup

### Required Files

Every public repository should include:

- **`README.md`** — Project overview, setup instructions, usage
- **`LICENSE`** — Open source license (typically MIT or Apache 2.0)
- **`.gitignore`** — Language/framework appropriate ignore rules
- **`CHANGELOG.md`** — Version history (for versioned projects)

### Recommended Files

- **`CONTRIBUTING.md`** — Contribution guidelines (for collaborative repos)
- **`CODE_OF_CONDUCT.md`** — Behavioral standards
- **`.editorconfig`** — Code formatting standards

### Repository Settings

- **Description:** Write a clear, concise description (shows in org view)
- **Topics:** Add relevant tags (e.g., `nationbuilder`, `python`, `campaign`)
- **Visibility:** Default to **Public** unless handling sensitive data
- **Issues:** Enable for collaborative projects
- **Wiki:** Disable (use `/docs` folder instead)

---

## 🤝 Contributing Code

### Workflow

1. **Fork** the repository (or branch if you have write access)
2. **Create a feature branch** — `git checkout -b feature/your-feature-name`
3. **Make changes** — Follow code style guidelines
4. **Commit** — Use clear, descriptive commit messages
5. **Push** — `git push origin feature/your-feature-name`
6. **Pull Request** — Submit PR with description of changes

### Commit Message Format

Use conventional commits for clarity:

```
type(scope): short description

- Detailed explanation (optional)
- Why the change was needed
- What was changed
```

**Types:**
- `feat:` — New feature
- `fix:` — Bug fix
- `docs:` — Documentation changes
- `style:` — Formatting, no code change
- `refactor:` — Code restructuring
- `test:` — Adding tests
- `chore:` — Maintenance tasks

**Examples:**
```
feat(voting): add preferential voting explainer section
fix(nav): correct mobile menu toggle behavior
docs(readme): update installation instructions
style(css): format homepage styles with prettier
```

---

## 🎨 Code Style

### General Principles

- **Consistency** — Follow existing project style
- **Readability** — Code is read more than written
- **Simplicity** — Prefer clear over clever
- **Documentation** — Comment complex logic

### Language-Specific

#### HTML/CSS
- 2-space indentation
- BEM naming for CSS classes (e.g., `.hero__title--large`)
- Semantic HTML5 elements

#### JavaScript
- ES6+ syntax
- Prettier formatting (`.prettierrc` in repo)
- JSDoc comments for functions

#### Python
- PEP 8 style guide
- Type hints where practical
- Docstrings for all functions/classes

---

## 🧪 Testing

- Write tests for new features
- Run existing tests before submitting PR
- Update tests when refactoring

---

## 📝 Documentation

### README Structure

Every README should include:

1. **Project Title** — Clear, descriptive name
2. **Description** — What it does, why it exists
3. **Installation** — How to set it up
4. **Usage** — Examples and basic commands
5. **Contributing** — Link to this guide
6. **License** — License type and link
7. **Contact** — How to get help

### Code Comments

- Explain **why**, not **what**
- Document edge cases and gotchas
- Keep comments up-to-date with code

---

## 🔒 Security

### Sensitive Data

**NEVER commit:**
- API keys or tokens
- Passwords or credentials
- Personal data (emails, phone numbers)
- NationBuilder access tokens

Use **environment variables** or **secret management** tools.

### Reporting Vulnerabilities

Email security concerns to: **contact@fusionparty.org.au**

Do not open public issues for security vulnerabilities.

---

## 📋 Pull Request Guidelines

### Before Submitting

- ✅ Code follows style guidelines
- ✅ All tests pass
- ✅ Documentation updated
- ✅ Commit messages are clear
- ✅ No merge conflicts

### PR Description Template

```markdown
## Description
Brief summary of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Refactoring
- [ ] Other (describe)

## Testing
How was this tested?

## Checklist
- [ ] Code follows style guidelines
- [ ] Self-review completed
- [ ] Comments added for complex logic
- [ ] Documentation updated
- [ ] No new warnings generated
```

---

## 🏷️ Issue Guidelines

### Creating Issues

- **Search first** — Check if issue already exists
- **One issue per problem** — Don't combine unrelated issues
- **Use templates** — Follow issue templates when provided
- **Be specific** — Include steps to reproduce, expected vs actual behavior

### Labels

Common labels we use:
- `bug` — Something isn't working
- `enhancement` — New feature request
- `documentation` — Docs need improvement
- `good first issue` — Good for newcomers
- `help wanted` — Extra attention needed
- `priority: high` — Critical issues

---

## 🌐 Localization

Currently, all code and documentation is in **English (Australian)**.

If contributing content visible to users:
- Use Australian English spelling (e.g., "colour", "labour", "organise")
- Follow Fusion Party style guide for political terminology

---

## 👥 Code of Conduct

All contributors must follow the [Fusion Party Code of Conduct](https://fusionparty.org.au/code_of_conduct).

### Summary

- Be respectful and inclusive
- Welcome diverse perspectives
- Focus on constructive feedback
- No harassment or discrimination

Violations can be reported to: **contact@fusionparty.org.au**

---

## ❓ Getting Help

### Questions?

- **Discord** — Join our [community server](#) for real-time help
- **Email** — [contact@fusionparty.org.au](mailto:contact@fusionparty.org.au)
- **Issues** — Open an issue in the relevant repository

### Resources

- [Fusion Party Website](https://fusionparty.org.au)
- [Policy Platform](https://fusionparty.org.au/policy)
- [NationBuilder Developer Docs](https://nationbuilder.com/developers)

---

## 📜 License

Unless otherwise specified, Fusion Party code repositories are licensed under:

- **MIT License** — For libraries and tools
- **Apache 2.0** — For larger projects
- **Creative Commons** — For documentation

**Party branding, logos, and official communications** are © Fusion Party Australia and not covered by code licenses.

---

## 🚀 Next Steps

Ready to contribute?

1. Browse [open issues](https://github.com/Fusion-Party-Aus) across repositories
2. Look for `good first issue` labels
3. Fork a repo and start coding
4. Submit your first PR!

---

**Thank you for helping build evidence-based politics in Australia!**

*For organisation-level questions, contact [contact@fusionparty.org.au](mailto:contact@fusionparty.org.au)*
