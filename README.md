# INTRODUCTION

Eslint, Prettier, Lint-Staged & Husky setup with PNPM

# PRECAP

Husky allows us to define commands that run before the commit thing happens.
In this case It runs

```
npx lint-staged
npm run lint
```

in sequence before for every commit.

# NOTES

1.Pre-commit hooks
Following line is important although it prompts to remove.

```
#!/usr/bin/env sh
. "$(dirname -- "$0")/_/husky.sh"
```

If we dont include so, we'll be thrown

```
error: cannot spawn .husky/pre-commit: No such file or directory
Couldn't start hook '.husky/pre-commit'
```

# MISCELLANEOUS

```
npx husky add .husky/pre-push "npm run test""
```
