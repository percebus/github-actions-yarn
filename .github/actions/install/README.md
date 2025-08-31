# (yarn) install

[`LICENSE`](./LICENSE)

Does some basic stuff

- `$> npm run setup:ci` (if present)\*
- `$> yarn install`

> NOTE: `yarn` does NOT support `run --if-present` (yet)

## Motivation

Sometimes we want to add some pre-setup stuff in the package that we want gets picked up by CI.

Things like packages being recommended being installed globally (i.e. `yarn`). Or some other setup w/ python `pip install -r requirements.txt`

## FAQs

### What is the difference w/ (pre|post)install

When developing locally, sometimes you want to run `yarn run setup(:ci)` only 1x. Whereas `yarn install` is executed more often when maintaining dependencies.

## References

- [`npm` CLI Commands](https://docs.npmjs.com/cli/v11/commands)

  - [`npm-install`](https://docs.npmjs.com/cli/v11/commands/npm-install)
  - [`npm-ci`](https://docs.npmjs.com/cli/v11/commands/npm-ci)
  - [`npm-run`](https://docs.npmjs.com/cli/v11/commands/npm-run)

- [`yarn` CLI Reference](https://yarnpkg.com/cli)
  - [`yarn install`](https://yarnpkg.com/cli/install)
  - [`yarn run`](https://yarnpkg.com/cli/run)
