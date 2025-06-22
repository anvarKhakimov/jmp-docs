# JMP Documentation

This repository contains the documentation for Jira Metrics Plugin (JMP).

## Structure

```
├── en/                 # English documentation
│   ├── getting-started/
│   ├── core-concepts/
│   └── reports/
└── ru/                 # Russian documentation
    ├── getting-started/
    ├── core-concepts/
    └── reports/
```

## Usage

This repository is designed to be used as a git submodule in multiple projects:

1. **jmp-site** - Main documentation website
2. **jmp-plugin** - Plugin development project

## Adding as Submodule

```bash
git submodule add <repository-url> contents/docs
git submodule update --init --recursive
```

## Updating Documentation

1. Make changes in your preferred project
2. Commit and push changes to this repository
3. Update submodule in other projects:
   ```bash
   git submodule update --remote contents/docs
   ```

## File Format

All documentation files are in MDX format with frontmatter:

```mdx
---
title: "Page Title"
description: "Page description"
---

# Content here
``` 