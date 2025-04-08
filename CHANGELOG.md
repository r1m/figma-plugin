# Changelog

## 2.6.0 (2025-04-08)


### Features

* add font style support for italic ([1a81e9a](https://github.com/r1m/figma-plugin/commit/1a81e9af7ad79e70881ec71a66b5903dab143800))
* add font style support for italic ([e1af3b8](https://github.com/r1m/figma-plugin/commit/e1af3b820bf4923c2623c4f750a2712eed8a079c))
* add support for grid ([3737ae3](https://github.com/r1m/figma-plugin/commit/3737ae3beb1b909071b4d7100fdaa89d2debc3b4))
* add support for more font weight combinations ([45429c7](https://github.com/r1m/figma-plugin/commit/45429c7c5d74fc43cea702f6fab50320a2f86c70))
* add support for selfhosted gitlab ([029b877](https://github.com/r1m/figma-plugin/commit/029b877e0956ab8c7cc2ffdda9b111d41b10abb8))
* add support for selfhosted gitlab ([95e6c3a](https://github.com/r1m/figma-plugin/commit/95e6c3a45479b651b4cdf3041f7ed5bc29934d50))
* add support for text and effects ([9ba4fa7](https://github.com/r1m/figma-plugin/commit/9ba4fa7455498777b4043748c398e16f60955e05))


### Bug Fixes

* clean options ([f6d206c](https://github.com/r1m/figma-plugin/commit/f6d206cb7f7878e0f20d802dfcdff4e21cef90da))
* cli package ([bbc0963](https://github.com/r1m/figma-plugin/commit/bbc0963c2a3fbfd387fadae618a7311a84901c5c))
* fix precision errors for floats ([73d82cf](https://github.com/r1m/figma-plugin/commit/73d82cf22a6180bac8c0cb3a1f59e52719238fd6))
* font style parsing ([be1af57](https://github.com/r1m/figma-plugin/commit/be1af5743de54d761217154a9f6749fb901932d9))
* precision errors for floats ([913b53b](https://github.com/r1m/figma-plugin/commit/913b53bc59bb19bd9600327e80f4826b3f63efed))
* version from package ([c982aa7](https://github.com/r1m/figma-plugin/commit/c982aa7aff525ab35ceb423f03beb3cf8a5ff8f1))


### Miscellaneous Chores

* release 2.6.0 ([b0053a8](https://github.com/r1m/figma-plugin/commit/b0053a816dacc49c9fef131106a9129b5759b4ad))

## 2.5.0

- [Introduce CLI Based tool that uses Figma Rest API](https://github.com/tokens-bruecke/figma-plugin/pull/33) _by [Sylvain Marcadal](https://github.com/r1m)_ (not yet published to NPM)
- [Fix: support font style strings like "Semi Bold"](https://github.com/tokens-bruecke/figma-plugin/pull/36) _by [Peter Lazar](peterlazar1993)_
- [Fix: precision errors for floats](https://github.com/tokens-bruecke/figma-plugin/pull/37) _by [Peter Lazar](peterlazar1993)_

## 2.4.0

- [Add font style support for italic](https://github.com/tokens-bruecke/figma-plugin/pull/35) _by [Sylvain Marcadal](https://github.com/r1m)_
- [Add support for selfhosted gitlab](https://github.com/tokens-bruecke/figma-plugin/pull/34) _by [Sylvain Marcadal](https://github.com/r1m)_

## 2.3.1

- [Fixes dimension type for vars with single scope](https://github.com/tokens-bruecke/figma-plugin/pull/31)

## 2.3.0

- Added `codeSyntax` property to variables. See this PR — [include variable's "codeSyntax" property in exported token json](https://github.com/tokens-bruecke/figma-plugin/pull/28)

## 2.2.3

- Convert `OPACITY` scope to valid value using this formula `value / 100`.

## 2.2.2

- Do not convert the value to PX units if the variable scope is `FONT_WEIGHT`

## 2.2.1

- Added `paragraphSpacing` and `paragraphIndent` to the typography styles

## 2.2.0

- Added aliases handling for typography styles — [Related issue](https://github.com/tokens-bruecke/figma-plugin/issues/24)
- Added aliases handling for effects

## 2.1.4 and 2.1.5

- Fix wrong font weight output. Related PR — [Right the heuristic wrongs](https://github.com/tokens-bruecke/figma-plugin/pull/20). _by [@JeroenRoodIHS](https://github.com/JeroenRoodIHS)_

## 2.1.3

- Fixed font weights to be numbers. Related PR — [Font weights fix - output as numbers (DTCG format)](https://github.com/tokens-bruecke/figma-plugin/pull/22)

## 2.1.2

- Updated the function to generate text styles. Related PR — [Update textStylesToTokens.ts ](https://github.com/tokens-bruecke/figma-plugin/pull/19)

## 2.1.1

- `$meta` tag moved to `$extensions` object. See issue — [$meta is not valid DTCG](https://github.com/tokens-bruecke/figma-plugin/issues/13)

## 2.1.0

- Multiple `Shadow` and `Blur` styles support added. [Link to the PR](https://github.com/tokens-bruecke/figma-plugin/issues/11)

## 2.0.0

- tokens structure was changed. All modes now moved from variable names into `$extensions/modes` object. In order to make it work with [Cobalt](https://cobalt-ui.pages.dev/guides/modes#with-modes). For morre details see this issue — [Multiple collection and modes](https://github.com/tokens-bruecke/figma-plugin/issues/7). Previous implementation didn't work correctly with multiple modes and aliasees.

## 1.6.0

- `value` string for aliases is now optional

## 1.5.0

- Added `GitHub PR` option to the `Push to server` feature
- `Connect server` renamed to `Push to server`
- _Thanks for contribution to [@distolma](https://github.com/distolma)_

## 1.4.0

- Added `warning` type to the `Toast` component
- structure refactoring
- code refactoring
- updated `Github` errors handling
- added `value` to all aliases at the end of the path. Also support for `DTCG` keys format added
- added storage versioning
- updated DTCG format switching
- added `Copy` button for the tokens preview

## 1.3.0

- Functions names refactoring

## 1.2.0

- Updated method to check `VARIABLE_ALIAS` in `normalizeValue` function
- Handle aliases from another files
- Removed the property `aliasPath` from `$extensions` object, since it's not needed anymore

## 1.1.1

- Updated errors handling for GitHub server

## 1.1.0

- `Update` button animation added
- added token types as a separate package

## 1.0.9

- Fixed `line-height` value conversion. It wasn't rounded to the nearest integer.

## 1.0.8

- Fix for [Reference tokens auto-referencing themselves in the exported JSON](https://github.com/PavelLaptev/tokens-bruecke/issues/1)

## 1.0.7

- Code cleanup

## 1.0.6

- WIP [Reference tokens auto-referencing themselves in the exported JSON](https://github.com/PavelLaptev/tokens-bruecke/issues/1)

## 1.0.5

- Allowed to use plugin in files without variables

## 1.0.4

- Fix scopes conversion
- `$meta` info adding order fixed

## 1.0.3

- HEX color fixed
- Alias variables fixed

## 1.0.2

- Fixed RGBA to HEXA conversion
- Added color styles support
- Added basic support for linear and radial gradients

## 1.0.1

- Fixed Aliases handling. Removed `mode` from the alias string if there is only one mode in the collection.

## 1.0.0

- Initial release
