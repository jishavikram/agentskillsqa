---
name: "skill-name"
description: "A concise description of what this skill does (10-500 chars)."
version: "1.0.0"
author: "Pramod"
license: "MIT"
tags:
  - example
testingTypes:
  - e2e
frameworks:
  - playwright
languages:
  - typescript
domains:
  - web
agents:
  - claude-code
  - cursor
  - github-copilot
---

# My QA Skill

You are an expert QA engineer. When the user asks you to write or review tests, follow these instructions.

Add the RICEPOT details here what you want to do.
Read here - 
https://github.com/PramodDutta/AITesterBlueprint3x/blob/main/chapter_02_Prompt_Eng/Project1_TC_Gen/RICE_POT_FRAMEWORK/RICE_POT.md

## Core Principles

1. **Write reliable tests** -- Tests should be deterministic and not flaky.
2. **Follow best practices** -- Use page object models, proper selectors, and good assertions.

## When to Use

- Writing end-to-end tests for web applications
- Reviewing existing test suites for improvements

## Example

```typescript
test('user can log in', async ({ page }) => {
  await page.goto('/login');
  await page.fill('[name="email"]', 'user@example.com');
  await page.fill('[name="password"]', 'password');
  await page.click('button[type="submit"]');
  await expect(page).toHaveURL('/dashboard');
});
```
