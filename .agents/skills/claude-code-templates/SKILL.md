```markdown
# claude-code-templates Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development patterns and conventions used in the `claude-code-templates` repository. The project is built with TypeScript and Express, emphasizing consistent code style, structured commit messages, and clear test organization. By following these patterns, contributors can maintain code quality and streamline collaboration.

## Coding Conventions

### File Naming
- Use **camelCase** for all file names.
  - Example: `userRoutes.ts`, `authMiddleware.ts`

### Import Style
- Use **relative imports** for modules.
  - Example:
    ```typescript
    import { getUser } from './userService';
    ```

### Export Style
- Use **named exports** for all modules.
  - Example:
    ```typescript
    // In userService.ts
    export function getUser(id: string) { ... }
    export const USER_ROLE = 'admin';
    ```

### Commit Messages
- Follow **conventional commit** standards.
- Use the `chore` prefix for routine tasks.
- Keep commit messages concise (average ~77 characters).
  - Example:
    ```
    chore: update dependencies to latest minor versions
    ```

## Workflows

_No automated workflows were detected in this repository._

## Testing Patterns

- Test files use the pattern: `*.test.*`
  - Example: `userService.test.ts`
- Testing framework is **unknown** (not detected), but tests are organized alongside source files using the above pattern.

## Commands
| Command | Purpose |
|---------|---------|
| /commit-chore | Create a conventional commit with the `chore` prefix |
| /run-tests | Run all test files matching `*.test.*` |
```