# Contributing

Thanks for helping out. Setup and dev instructions live in the [README](README.md#from-source).

## Before opening a PR

The build must pass. There's no CI yet, so please check locally:

```bash
npm run build
```

TypeScript runs with `strict: true` and `ts-loader` fails the build on any error, so a type error is a broken build, not a warning.

Test against a real Tabby install. Say which platform and Tabby version you used.

## Commit messages

Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/): `type(scope): subject`, scope optional.

Types: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `build`, `ci`, `chore`. Breaking change: `type!: subject`.

```
feat(browser): support Tabby split panes
fix(browser): forward function keys to HotkeysService
```

PRs are squash merged, so branch history is yours to organise however you like. Put the reasoning in the PR description - that's what gets read.

## Code style

Skip unnecessary comments. Code should speak for itself, so a comment restating what the code does can go - rename or restructure instead. Keep the ones that carry something the code can't say on its own, like an Electron or Tabby quirk you had to work around.

Match the surrounding code: 4 spaces, no semicolons, single quotes, space before the paren in method declarations.
