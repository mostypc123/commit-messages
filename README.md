# Good Git Commit Messages 📝

## Types with Emojis

✨ feat: New feature

🐛 fix: Bug fix

📚 docs: Documentation changes  

💄 style: Code formatting

♻️ refactor: Code refactoring

⚡ perf: Performance improvements

✅ test: Adding/modifying tests

🔧 chore: Maintenance tasks

## Message Format

```
<emoji> <type>(<scope>): <subject>

<body>

<footer>
```

## Examples

```
✨ feat(auth): add Google OAuth2 login

- Implement OAuth2 client configuration
- Add user profile mapping
- Update session management

Closes #123
```

```
🐛 fix(api): prevent payment processing race condition

Added mutex lock to prevent double-charging during concurrent requests.

Fixes #456
```

```
📚 docs(readme): update installation steps

- Add Docker setup instructions
- Update environment variables table
- Include troubleshooting guide

Related to #789
```

```
♻️ refactor(db): migrate user queries to Prisma

Replace raw SQL queries with Prisma client in user service.

BREAKING CHANGE: User model schema updated
```

```
💄 style: enforce consistent spacing

- Add prettier configuration
- Format all files
- Update CI to check formatting
```

```
⚡ perf(cache): optimize database caching

- Implement Redis caching layer
- Add cache invalidation
- Reduce average query time by 50%
```

```
✅ test(auth): add unit tests for login flow

- Test successful login
- Test invalid credentials
- Test rate limiting
```

```
🔧 chore(deps): update dependencies

- Update React to v18
- Update TypeScript to v5
- Fix peer dependency warnings
```
