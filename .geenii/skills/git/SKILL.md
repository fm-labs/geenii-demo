---
name: git
description: Use this skill whenever the user wants to execute Git commands, manage repositories, or interact with GitHub using command-line tools.
compatibility: Runs on any system with Git installed and appropriate permissions for executing commands and accessing files.
metadata:
  version: 1.0
  author: geenii
allowed-tools: execute_command file_read
---

# Git CLI Usage Guide

## Overview

This guide covers essential Git commands for managing repositories, checking status, viewing commit history, and cloning repositories using command linetools.


## Rules
- Always check the current git status first
- Then perform git operation


## Quick Reference

All operations use the `git` binary.

```bash
git
```

### Check the status of a Git repository:

```bash
git status
```

### Check if there are uncommitted changes in a Git repository:

```bash
git status --porcelain
```

### View the commit history of a Git repository:

```bash
git log --oneline
```

To get the last N commits, use:

```bash
git log --oneline -n N
# e.g. git log --oneline -n 5
```

### Clone a Git repository:

```bash
git clone REPOSITORY_URL
# e.g. git clone https://github.com/username/repository.git
```

### Check the current branch of a Git repository:

```bash
git branch --show-current
```

### List all branches in a Git repository:

```bash
git branch
```

### Create a new branch in a Git repository:

```bash
git checkout -b NEW_BRANCH_NAME
# e.g. git checkout -b feature/new-feature
```

### Switch to an existing branch in a Git repository:

```bash
git checkout BRANCH_NAME
# e.g. git checkout main
```

### Initialize a new Git repository in the current directory:

```bash
git init
```


## When to use

- Use if the user wants to perform an operation on a git repository



## Dependencies

- `git` binary installed