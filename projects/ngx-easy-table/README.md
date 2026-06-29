> This is an actively maintained fork of [ssuperczynski/ngx-easy-table](https://github.com/ssuperczynski/ngx-easy-table). Published to npm as `ngx-easy-table-plus`.

[![npm version](https://badge.fury.io/js/ngx-easy-table-plus.svg)](https://www.npmjs.com/package/ngx-easy-table-plus)
[![last commit](https://badgen.net/github/last-commit/vincent-cholet/ngx-easy-table-plus)](https://badgen.net/github/last-commit/vincent-cholet/ngx-easy-table-plus)
[![total downloads](https://badgen.net/npm/dt/ngx-easy-table-plus)](https://badgen.net/npm/dt/ngx-easy-table-plus)

## Demo

<a href="https://vincent-cholet.github.io/ngx-easy-table-plus/" target="_blank">
https://vincent-cholet.github.io/ngx-easy-table-plus/
</a>

## Code Examples

<a href="https://github.com/vincent-cholet/ngx-easy-table-plus/tree/master/src/app/demo" target="_blank">
https://github.com/vincent-cholet/ngx-easy-table-plus/tree/master/src/app/demo
</a>

## Installation

```sh
npm install ngx-easy-table-plus --save
```

Library requires `@angular/cdk`, please install it as well.

```sh
npm install @angular/cdk --save
```

## Available config settings

Every available configuration option and feature has a runnable example in the
[demo](https://vincent-cholet.github.io/ngx-easy-table-plus/), with the source for each
example in [src/app/demo](src/app/demo).

## Development

- 1st tab - `npm run watch:table`
- 2nd tab - `cd dist/ngx-easy-table && npm link`
- 2nd tab - go back to project root dir and `npm link ngx-easy-table-plus`
- 2nd tab - `npm run start`

At the end run `npm run cy:ci` to make sure everything works.

## Releasing a new version

1. Bump the version in `projects/ngx-easy-table/package.json`.
2. Commit and push that change.
3. Tag and push the tag — this triggers the publish workflow:

```sh
git tag v15.8.0
git push origin v15.8.0
```

The `.github/workflows/publish.yml` workflow lints, builds, runs e2e tests,
and publishes to npm automatically. If any of those steps fail, the tag is
pushed but nothing gets published — fix the issue and push a new tag.
