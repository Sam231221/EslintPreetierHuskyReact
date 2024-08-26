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
