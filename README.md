[![Release][release-src]][release-href]
[![npm version][npm-version-src]][npm-version-href]
[![License][license-src]][license-href]

# Install

My typescript configs.


```
yarn add -D @alanscodelog/tsconfigs \
&& ./node_modules/@alanscodelog/tsconfigs/install.sh
```
Note: The last command will overwrite `tsconfig.json` and `tsconfig.types.json` if it exists.

# Manual Setup
```bash
cp ./node_modules/@alanscodelog/tsconfigs/copy/tsconfig.json tsconfig.json
```
or copy [this](https://github.com/AlansCodeLog/tsconfigs/blob/master/copy/tsconfig.json) to `tsconfig.json`.


For generating types:
```bash
cp ./node_modules/@alanscodelog/tsconfigs/copy/tsconfig.types.json tsconfig.types.json
```
or copy [this](https://github.com/AlansCodeLog/tsconfigs/blob/master/copy/tsconfig.types.json) to `tsconfig.types.json`.

Then add a script to the `package.json`:
```json
"scripts": {
	"build:types": "tsc -p tsconfig.types.json --emitDeclarationOnly",
}
```

<!-- Badges -->
[release-src]: https://github.com/alanscodelog/tsconfigs/actions/workflows/release.yml/badge.svg
[release-href]: https://github.com/alanscodelog/tsconfigs/actions/workflows/release.yml
[npm-version-src]: https://img.shields.io/npm/v/@alanscodelog/tsconfigs/latest
[npm-version-href]: https://www.npmjs.com/package/@alanscodelog/tsconfigs/v/latest
[license-src]: https://img.shields.io/npm/l/@alanscodelog/tsconfigs.svg?style=flat&colorA=020420&colorB=00DC82
[license-href]: https://npmjs.com/package/@alanscodelog/tsconfigs
