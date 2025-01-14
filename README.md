# Awesome Git Commit Conventions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome Git commit conventions, tools, resources, and best practices.

## Contents

- [Commit Types](#commit-types)
- [Message Format](#message-format)
- [Examples](#examples)
- [Tools](#tools)
- [Guidelines](#guidelines)

## Commit Types

Common types of commits with their corresponding emojis:

- ✨ feat: New feature
- 🐛 fix: Bug fix
- 📚 docs: Documentation changes
- 💄 style: Code formatting
- ♻️ refactor: Code refactoring
- ⚡ perf: Performance improvements
- ✅ test: Adding/modifying tests
- 🔧 chore: Maintenance tasks
- 🔒 security: Security improvements
- 🌐 i18n: Internationalization and localization
- 📱 mobile: Mobile-specific changes
- 🎨 ui: User interface and design changes
- 📦 deps: Dependency updates
- 🚀 deploy: Deployment related changes
- 🔍 seo: Search Engine Optimization
- 🎯 ci: Continuous Integration configuration
- 📈 analytics: Analytics and tracking
- 🗃️ db: Database changes
- 🧪 experiment: Experimental features
- 🚧 wip: Work in progress
- 🔥 remove: Code removal
- 🚨 alert: Critical changes
- 🔈 logging: Logging improvements
- 🏗️ build: Build system changes
- 🔁 sync: Data synchronization
- 📊 metrics: Metrics and monitoring
- 🔌 api: API-related changes

## Message Format

The commit message should be structured as follows:

```
<emoji> <type>(<scope>): <subject>

<body>

<footer>
```

### Components

- `emoji`: A visual indicator of the commit type
- `type`: The category of the commit change
- `scope`: The module/component being modified (optional)
- `subject`: A brief description of the change
- `body`: Detailed explanation of the change (optional)
- `footer`: Reference to issues, breaking changes, etc. (optional)

## Examples

### Feature Addition
```
✨ feat(auth): add Google OAuth2 login

- Implement OAuth2 client configuration
- Add user profile mapping
- Update session management

Closes #123
```

### Bug Fix
```
🐛 fix(api): prevent payment processing race condition

Added mutex lock to prevent double-charging during concurrent requests.

Fixes #456
```

### Security Update
```
🔒 security(auth): implement rate limiting for login attempts

- Add Redis-based rate limiting
- Block IPs after 5 failed attempts
- Send notification on suspicious activity

Fixes CVE-2024-xxxx
```

## Tools

### Commit Linting
- [commitlint](https://github.com/conventional-changelog/commitlint) - Lint commit messages
- [husky](https://github.com/typicode/husky) - Git hooks made easy

### Commit Generation
- [commitizen](https://github.com/commitizen/cz-cli) - Interactive commit message CLI
- [gitmoji-cli](https://github.com/carloscuesta/gitmoji-cli) - Interactive emoji commit generator

### Changelog Generation
- [conventional-changelog](https://github.com/conventional-changelog/conventional-changelog) - Generate changelogs from commit messages
- [release-please](https://github.com/googleapis/release-please) - Automate releases with conventional commits

## Guidelines

### Best Practices

1. Keep subject lines concise (50 characters or less)
2. Use imperative mood in subject line ("Add feature" not "Added feature")
3. Capitalize the subject line
4. Don't end the subject line with a period
5. Separate subject from body with a blank line
6. Wrap the body at 72 characters
7. Use the body to explain what and why vs. how

### Do's and Don'ts

✅ Do:
- Write clear, meaningful commit messages
- Use the specified format consistently
- Reference issues and PRs where appropriate
- Include breaking changes in footer

❌ Don't:
- Write vague messages ("Fix bug", "Update code")
- Mix multiple unrelated changes
- Forget to mention breaking changes
- Skip the emoji if your team uses them

## Contributing

Feel free to submit pull requests to add more commit types, tools, or resources to this list.
