# Next.js Guidance

This is not the Next.js you know. This version has breaking changes:
APIs, conventions, and file structure may all differ from your training data.
Read the relevant guide in `node_modules/next/dist/docs/` before writing any code.
Heed deprecation notices.

## Project Rules

- Use Tailwind for all styling.
- Use block `if` statements with braces. Do not write one-line conditionals.
- Use shadcn/ui components where practical. Ask before adding custom base components.
- When sibling HTML or JSX elements share an indentation level, leave a blank line between them.
- Assume the dev server is already running.
- Run `bun run format`, `bun run lint`, and `bun run spell` after changing files.
- If `bun run spell` fails, fix real spelling mistakes first. If there are no spelling mistakes, update `cspell.json` so spellcheck passes.

## File Organization

Organize source files in this order. Do not add section comments.

1. Constants and types
2. Main exported function or functions
3. Helper functions, ordered so callers appear before callees
