# Changelog

## [8.0.0](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/compare/v7.3.0...v8.0.0) (2026-05-16)


### ⚠ BREAKING CHANGES

* Requires Node.js: ^18.18.0 || ^20.9.0 || >=21.1.0
* Update node versions to align with eslint v9 ([#484](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/484))
* Requires Node@^12.22.0 || ^14.17.0 || >=16.0.0
* Requires ESLint@^7.x
* dropping support for Node 4 requires a major version bump.

### 🌟 Features

* **`catch-or-return`, `prefer-await-to-then`:** do not report Cypress commands ([#495](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/495)) ([943f162](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/943f16290f11af9717612e079646802e22310290))
* **`no-callback-in-promise`:** add `timeoutsErr` option ([#514](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/514)) ([907753f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/907753f4b6108ba78b93571a40b6f1384b3c6899))
* **`no-promise-in-callback`:** add `exemptDeclarations` option ([#513](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/513)) ([550524f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/550524f2e07e392926b1e6330c7e21b5f91529ad))
* **`prefer-await-to-then`:** ignore constructor scope unless with `strict` option ([#496](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/496)) ([7bffb7a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7bffb7a666ed74a876ba3a6c482c36ea6f9d6d07))
* **`valid-params`:** add `exclude` option ([#515](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/515)) ([7ff2cb9](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7ff2cb9298f5dd0b4dae82321605d04e50ca935b))
* add `name` property to configs (for use with tooling) ([#486](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/486)) ([ca9e9b4](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ca9e9b4cc1d6e9d1c6951125514b2facbc2d9ad9))
* add `no-multiple-resolved` rule ([#369](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/369)) ([3a6fdbe](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/3a6fdbe3745e1253d5da5fb1d313e9025e4e7269))
* add `strict` option to disallow `then` or `catch` following `await` or `yield` ([#494](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/494)) ([fa482cc](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/fa482cc1134f5669b2dd9f56ea2ef9e96c3c30a0))
* add support for ESLint v10 ([#617](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/617)) ([6096821](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/6096821370e7662a61abcee2822f9b1750fb53c4))
* add support for eslint v9 ([#478](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/478)) ([4dfc8a7](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4dfc8a77c0592a19d467a268708678114c3c7c2b))
* add support for flat config ([#479](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/479)) ([ecbce9f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ecbce9faef0c8e05636287cf9c851949be6d70cc))
* add tests for @typescript-eslint/parser ([9bdf8dc](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/9bdf8dcabe90dc2a746cde81e75e18c4583c5f96))
* **always-return:** add `ignoreAssignmentVariable` option ([#518](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/518)) ([701279c](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/701279c573437598e86873f48b4f5cf6432ae38e))
* **always-return:** add `ignoreLastCallback` option ([#365](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/365)) ([01def31](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/01def31afe765887eaaeb269992e03ef91426ede))
* **catch-or-return,no-new-statics,no-promise-in-callback,valid-params:** add support for `Promise.allSettled()` & `Promise.any()` ([#370](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/370)) ([e080f82](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/e080f826a997e97f4b9be52c567b77268ad18deb))
* **catch-or-return:** add ['catch'] support ([6bf9642](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/6bf9642950a97decdf1f6cc132553e9ee67a610b))
* **catch-or-return:** add `allowThenStrict` option ([#522](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/522)) ([53be970](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/53be970e91023a104ce3ef2918b3ee80ef265f27))
* drop Node 10 support ([ea6536b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ea6536bd3d702af2a6cb38253954c978bfddffab))
* drop Node 10 support ([7ac06ac](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7ac06ac3aef4efa288917babff41649cc52fef53))
* **fixer:** add fixer for param-names ([#99](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/99)) ([c0c662a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c0c662a0906bc5b6b117b9bf454af31249b97b4f)), closes [#90](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/90)
* **fixer:** add fixer to no-new-statics rule ([#133](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/133)) ([15f0649](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/15f0649c920b263c3c5bdefce39bf47868edbc84))
* new rule `prefer-catch` ([#525](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/525)) ([05c8a93](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/05c8a930893e6abff2a0a7e1fb82a1543c19df9f))
* new rule `spec-only` to check for non-spec Promise methods ([#502](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/502)) ([d6e9de1](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/d6e9de1f9c81194b775484ed0299dc5cc4898684))
* **param-names:** add `resolvePattern` & `rejectPattern` option ([#368](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/368)) ([df25e3c](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/df25e3c2c2faf3ab5aa96fbd5de747285776bafe))
* Resolve `getAncestors` and `getScope` calls in eslint v9 ([#466](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/466)) ([c0c716b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c0c716b1c5e513ece52443c0f0848e5aee5e2ef7))
* **rule:** add no-new-statics rule ([#82](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/82)) ([3af50b7](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/3af50b7804be61d08c6ba841510e440237efdba5)), closes [#75](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/75)
* **rule:** add valid-params rule ([#85](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/85)) ([4782ae5](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4782ae51dd5800f7ffe954ee96f8ef049ffe53b0)), closes [#47](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/47)
* Support ESLint 7.x ([462a3b2](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/462a3b2c25cf71bd03380bd59f8828417ac0982b))
* Support ESLint 7.x ([e2b1fcc](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/e2b1fcc970a6d585e03f4d2aff577b5844a00a18))
* support ESLint 8.x ([ff1ad03](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ff1ad0331c3d96a961f6c2812e4dabda50009401))
* support ESLint 8.x ([86d81ee](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/86d81ee26994bf497f4d5d85da01fb5dc3926775))
* turn off avoid-new in recommended configuration ([#119](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/119)) ([ceb7414](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ceb7414fe34ceceec4904012a69c93155b603e3c)), closes [#111](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/111)
* Update node versions to align with eslint v9 ([#505](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/505)) ([09d0650](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/09d0650846806df7fc4ce26156865cf57e27fba6))


### 🩹 Fixes

* **`always-return`:** treat process.exit() or process.abort() as an acceptable "return" ([#493](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/493)) ([f368c5a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/f368c5a7e4a1c1f40cafbf038b629e6054d2027e))
* **`no-callback-in-promise`:** false triggering of callback ([#574](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/574)) ([8324564](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/83245645a1731b8720ba4b17951f0e98567f449c))
* 49 ([81b2172](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/81b2172de96264f2eefd6172a67489de8741e57b))
* add rule documentation ([#91](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/91)) ([d74d879](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/d74d8793199b33380ac96b9e39e81c415c8784f8)), closes [#61](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/61)
* add typescript to dev dependencies ([c681f8a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c681f8a018813678b604f106c980b66a5e2ea11d))
* **always-return:** false positives for logical expr ([#363](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/363)) ([a60d1cb](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/a60d1cbd427159d913e57f5845cec111d3ab882e))
* **CI:** fix release script ([#380](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/380)) ([71e53a0](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/71e53a0b8270b4e7d8c59ad987d8024f9529c56a))
* default to leftToBeResolved, fixes [#205](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/205) ([5acfe8e](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5acfe8e05bcf6b414347fe718967df451c139a41))
* default to leftToBeResolved, fixes [#205](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/205) ([60d3ed7](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/60d3ed714a8c40cb111a64dc16a52bdeac37e8c0))
* ignore event listener callbacks in prefer-await-to-callbacks ([#117](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/117)) ([4ebd2c6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4ebd2c667d389e4b4f677560264db33612c86497))
* ignore top-level awaits in prefer-await-to-then ([#126](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/126)) ([4a3d5b8](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4a3d5b8ebfd581b3fdfec0df82363e6690985953)), closes [#122](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/122)
* include plugin with recommended settings ([#157](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/157)) ([c159832](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c1598326b1d89d26af8a864f70a7759efb613f50))
* minor typos ([#359](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/359)) ([b431e46](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b431e4656453efa645e0aa63d1c7cbbf535e2cea))
* **no-callback-in-promise:** false positives when the exception is an argument ([#446](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/446)) ([5e4546d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5e4546d83b45eae41637f0c13b1c9748421098aa))
* **no-multiple-resolved:** false positives when the last expression in a try block is a call to resolve ([#384](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/384)) ([dc51b1c](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/dc51b1c890b284b262b384ab65263e65aff903b7))
* **no-native:** fix to report `Promise` usage in eslint v9 or later ([#619](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/619)) ([1230ced](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/1230ced57c422196735fa5f4c404d4c46c620c14))
* **no-nesting:** nested references vars in closure ([#361](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/361)) ([08052e8](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/08052e8528ec1ebfd60847801e44b8b2ed5803e1))
* **no-return-wrap:** fix it not reporting for arrow functions without braces ([41ec09f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/41ec09fdd30e45dcb1bf8a9c430de7dde3cddb71))
* **no-return-wrap:** fix it not reporting for arrow functions without braces (fixes [#193](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/193)) ([927a7f0](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/927a7f0be74619e2eae587c2a21c78e390bff2f9))
* **param-names:** avoid including `fixable: code` when not fixable ([045aa2e](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/045aa2e079292daf8185fa34ab7fa3597c5fb49c))
* **param-names:** remove fixer ([#146](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/146)) ([af28d6f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/af28d6f774613ab3d3dd1d3f3ba1ecc6d8d8d5e5)), closes [#145](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/145)
* permit appropriate computed member expressions and prototype access ([#535](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/535)) ([4de9d43](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4de9d43b84f1beb166a7ba779a4da9d732d0eab3))
* **prefer-await-to-then:** member access without call ([#362](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/362)) ([9b3ef57](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/9b3ef57cb3030e64b9a6b510aea6b2b5e7553ce8))
* remove `name` from eslintrc config; fixes [#489](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/489) ([#490](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/490)) ([c011a1a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c011a1a9f208efe35f1940b8a09db6023200625b))
* **rulesMeta:** update invalid rule docs url in rule's metadata ([5bffa17](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5bffa17ae5f8170f36299c61e085be2cbc266524))
* **rulesMeta:** update invalid rule docs url in rule's metadata ([79e8bda](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/79e8bdab89e227e8d888ac7a208bdda2b90a097c))
* update repo link ([#349](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/349)) ([3906810](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/39068101e207903a79bbb7d67d2c5f4a1a189d36))


### 📚 Documentation

* add code of conduct ([#94](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/94)) ([a36a243](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/a36a243a0dfed7049e6878175e673af9d0592a9b))
* add CONTRIBUTING.md ([#97](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/97)) ([ccae75b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ccae75b9c3c330674a8705c2b28c577ea65e6a6d)), closes [#84](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/84)
* add examples to `prefer-await-to-then` ([#121](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/121)) ([5956eca](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5956eca1b087f04ac49574a035d3045786a165d1))
* add for `prefer-await-to-callbacks`; fixes [#118](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/118) ([#491](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/491)) ([36d13f5](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/36d13f5266158eef615d3801117e40000c29dd21))
* add GitHub issue template ([#104](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/104)) ([e3504bf](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/e3504bf311712e4ea49bcd2002cb406266fbdb85)), closes [#87](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/87)
* add GitHub pull request template ([#105](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/105)) ([7d72e0c](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7d72e0cd7d40c8bf28fd79664daee476115d1ab2)), closes [#88](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/88)
* add no-nesting examples ([#120](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/120)) ([0b231da](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/0b231da24b8c63b636cb42e571abc3365e8f06cd))
* automate docs with `eslint-doc-generator` ([#396](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/396)) ([cfd5506](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/cfd5506e941e15413247c28f6784fbfcfb5e4cdb))
* **changelog:** prepare for v3.7.0 ([#115](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/115)) ([c274c6b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c274c6b10ab3858e659bdf47cb92e73367760f40))
* **changelog:** prepare for v3.8.0 ([#132](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/132)) ([212e557](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/212e557f0d518f39b401631e845644307815022d))
* **changelog:** prepare for v4.0.1 ([1b01507](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/1b0150716d9456e94056e6bed4349ad3f43d7b95))
* fixes the CI readme badge ([#511](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/511)) ([030a3be](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/030a3be890d371381ef13258806f97ec62d6b4fd))
* migrate rule documentation to docs/rules ([#112](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/112)) ([3e674c3](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/3e674c3205f883bb97ca803d9210abad3563eb61))
* **no-new-statics:** add mention of the rule being fixable ([15229b6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/15229b6c28856dd1bf7404168c88ee4230fc1e96))
* **param-names:** clarify that param-names includes ordering ([#143](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/143)) ([24c4bd7](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/24c4bd71cd8baf858e5a7d9d4dca0711d96d8e6a)), closes [#139](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/139)
* **param-names:** fix incorrect description location ([#137](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/137)) ([47d5c55](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/47d5c559cbff144b3fdbf0b3c6c568fc9aa54a03))
* **param-names:** Remove `fixable` reference as not currently fixable ([202798d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/202798df49c0596630304f3e2ee2fb1da75dbe4b))
* prettify changelog ([#114](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/114)) ([0f8e861](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/0f8e8616612a0fa640dcf27cdffe0c0c896ffb40))
* prettify README ([#98](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/98)) ([c9870d6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c9870d6beffaa0408b030125822bf2b1078d7173))
* **readme:** add maintainers section ([#92](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/92)) ([7b30978](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7b309784a953f38c625503489a37c006b6a3d3f9))
* **README:** add no-multiple-resolved rule link ([#371](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/371)) ([55a304c](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/55a304cbaffeadb26b841c2cc1a02f1feab69b55))
* **readme:** add table of contents ([#86](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/86)) ([d52d30c](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/d52d30cd1737187e838cc163525c28731589282a))
* **readme:** update badges ([#107](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/107)) ([216649b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/216649b1e992f33162bbae7ff15f22948be9ab42))
* recommend `util.promisify` instead of pify and `util.callbackify` over nodeify ([#492](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/492)) ([9d0e447](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/9d0e44733d32a0b22fd604b758386bd51f9da6df))
* supply missing docs ([#503](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/503)) ([602d825](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/602d8254871e46c9d1808ee1a3a2c48cb7493334))
* update README ([#383](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/383)) ([d8d0fbe](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/d8d0fbe4d2d34292e737d895d2b531fe901cba48))
* updated docs for always-return ([b72d831](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b72d831346383baf663fab119d08d35302a4640e))
* Use link to tagged version for rule docs ([#110](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/110)) ([8c82ddb](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/8c82ddbed953fd697ba80103e6521c094daba20c))


### 🧹 Chores

* add `format` workflow ([#441](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/441)) ([1376ecf](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/1376ecfb8291561ef33301d983c9e9433ddef53d))
* add aaditmshah to the contributors list ([c97dc50](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c97dc505312adbb8cab16357f9a68d7a1ef61a81))
* add license ([34c2f76](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/34c2f76d1a5b332ff93bb9c22ccb4fedbec4755d))
* add license ([c30a439](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c30a43908be2cc00912e84f56e16f8f11ef277d5))
* add missing `'use strict'` directive ([#593](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/593)) ([4cd7ea1](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4cd7ea162c946604f953199393fa66ea47dce872))
* add pkg.funding ([#468](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/468)) ([7d33c30](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7d33c30db828a484447651bf12ab3f077cd82c80))
* add tests for Node 20 ([#440](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/440)) ([bbcfcbf](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/bbcfcbf85ef97cba58f4fe4b9f46c907e04bc5a6))
* also test ESLint v7 on Node v18 ([#364](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/364)) ([ac98c63](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ac98c631132772b4decab61ff748ee2e6a062166))
* avoid recursion in `format`/`lint` ([#487](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/487)) ([46667d3](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/46667d3657a218191d1360b3de7e391d6557274e))
* bump dev dependencies ([#483](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/483)) ([197ae4e](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/197ae4eb4f05f34c54189102871d969379595a54))
* **CI:** add automatic release ([#379](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/379)) ([04fa169](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/04fa169ca9a70006f7d204e057355fdad2e2e519))
* **CI:** simplify testing strategy ([#378](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/378)) ([c970565](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c970565d20098579157debea7509201d54373646))
* **CI:** support testing against multiple ESLint versions ([4281516](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/42815161a16f95bab60047cb901445a2e439df78))
* **CI:** support testing against multiple ESLint versions ([364b664](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/364b664db50e3534ed7c4f05c1f2e7df8d1b730c))
* clean up tests ([#101](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/101)) ([752bbd7](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/752bbd7aca51a46f43c69528ed9c951bdc8ddcff))
* create `dependabot.yml` ([5db056c](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5db056c5742dc1298ddbfdf367f4e6f0e9df7d6b))
* create `dependabot.yml` ([4d8f3f0](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4d8f3f0a64dd6d7ed31d2661d45bb4bbaff91f4f))
* **deps-dev:** bump @babel/traverse from 7.19.1 to 7.24.1 ([#453](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/453)) ([ce9ae7f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ce9ae7f4ff43859fd7fb895644ed4f16a8ef27dc))
* **deps-dev:** bump @typescript-eslint/parser from 5.38.0 to 5.38.1 ([#358](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/358)) ([5d77f93](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5d77f937c3c06f8435351dc7821da6658551d73b))
* **deps-dev:** bump @typescript-eslint/parser from 5.38.1 to 5.39.0 ([#374](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/374)) ([7cfa19e](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7cfa19eda3f5781e8cd50f99ca23717e3f645c05))
* **deps-dev:** bump @typescript-eslint/parser from 5.39.0 to 5.40.0 ([#377](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/377)) ([e8eabf4](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/e8eabf46744c7b8cbdfbb608cc870c7ca5000735))
* **deps-dev:** bump @typescript-eslint/parser from 5.40.0 to 5.40.1 ([#390](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/390)) ([ea286a6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ea286a6670ce2cfffa809c2c17e3ae4c80f5698c))
* **deps-dev:** bump @typescript-eslint/parser from 5.40.1 to 5.41.0 ([#395](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/395)) ([23bf271](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/23bf27128fac92e57f7be7a951af86806ca10aa0))
* **deps-dev:** bump @typescript-eslint/parser from 5.41.0 to 5.42.0 ([#397](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/397)) ([0f76e1a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/0f76e1a03d97e6abfdd07da6dcdf9c7efb075c56))
* **deps-dev:** bump @typescript-eslint/parser from 5.42.0 to 5.43.0 ([#409](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/409)) ([fe6b233](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/fe6b2336bda1f3b46eb8ea07694ee6e2b35b7f46))
* **deps-dev:** bump @typescript-eslint/parser from 5.43.0 to 5.45.0 ([#417](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/417)) ([6d046e6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/6d046e6033d43d2c023966b33a7fabc1438899c2))
* **deps-dev:** bump braces from 3.0.2 to 3.0.3 ([#477](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/477)) ([afbda82](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/afbda82b8e6c2f3b905192d26e893a9d45bfc6a1))
* **deps-dev:** bump doctoc from 2.2.0 to 2.2.1 ([#343](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/343)) ([6bd5f3f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/6bd5f3fccae6ef6ecc536816d8250e3ad7a6fac2))
* **deps-dev:** bump eslint from 8.23.1 to 8.24.0 ([#355](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/355)) ([3c2f68a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/3c2f68a7bb24d65b2b79cef8a2d9f0fdde253dc3))
* **deps-dev:** bump eslint from 8.24.0 to 8.25.0 ([#376](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/376)) ([b2136c3](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b2136c39b38881ca1225560a5d74a0f7384a8244))
* **deps-dev:** bump eslint from 8.25.0 to 8.26.0 ([#393](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/393)) ([ed41376](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ed41376b2b3c40a8f46fc081d2dfde116392a77a))
* **deps-dev:** bump eslint from 8.26.0 to 8.27.0 ([#400](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/400)) ([4533989](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/453398979aa6c62fce0c9c155a1e38f1226b32e1))
* **deps-dev:** bump eslint from 8.27.0 to 8.28.0 ([#414](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/414)) ([d5d3b40](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/d5d3b40e39dd933189a6924e550bba669f639847))
* **deps-dev:** bump eslint from 8.5.0 to 8.23.1 ([#342](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/342)) ([ff9f525](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ff9f5257b743839d2a4eeb63783d082be0459583))
* **deps-dev:** bump eslint-config-prettier from 8.3.0 to 8.5.0 ([#280](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/280)) ([4ae2fa1](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4ae2fa10545c0014462dfd1e12955a6b088ef7a5))
* **deps-dev:** bump eslint-doc-generator from 0.17.0 to 0.19.0 ([#399](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/399)) ([326f67d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/326f67d5b70173f78c6078f1ce4299b531a5cc41))
* **deps-dev:** bump eslint-doc-generator from 0.19.0 to 0.19.1 ([#404](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/404)) ([82c4644](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/82c464496bd0d20d827c8dabddc17d735b5c650e))
* **deps-dev:** bump eslint-doc-generator from 0.19.1 to 0.21.0 ([#411](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/411)) ([2d52062](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/2d520621cb3cbcfcec745b4a8e67d36aee3974e7))
* **deps-dev:** bump eslint-doc-generator from 0.21.0 to 0.25.0 ([#413](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/413)) ([97fe33b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/97fe33bd8af7a222cbfacf4d7542cc70cc31d1f9))
* **deps-dev:** bump eslint-plugin-jest from 26.9.0 to 28.6.0 ([#474](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/474)) ([744ef1d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/744ef1d99fdc8417b13b4092e369202e05c674c2))
* **deps-dev:** bump eslint-plugin-jest from 28.6.0 to 28.8.0 ([#536](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/536)) ([80741f8](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/80741f849db526cad362cfc976c69a1df036a6c6))
* **deps-dev:** bump eslint-plugin-n from 17.9.0 to 17.10.2 ([#529](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/529)) ([a646010](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/a646010a7700a87c0fcc8aa0bb0d580bd6a14fd4))
* **deps-dev:** bump eslint-plugin-prettier from 4.0.0 to 4.2.1 ([#348](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/348)) ([e55013a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/e55013a295e96dc79c8e9b85924e6587c4f017e3))
* **deps-dev:** bump globals from 15.8.0 to 15.9.0 ([#527](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/527)) ([b8afe92](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b8afe920bd3be1120f5effb4a9a71451a3e71c24))
* **deps-dev:** bump husky from 9.1.1 to 9.1.2 ([#516](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/516)) ([ab8e7a0](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ab8e7a0d4fc8bde63fb6a6bb1e9743152778c4ee))
* **deps-dev:** bump husky from 9.1.2 to 9.1.4 ([#524](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/524)) ([b8fdb9f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b8fdb9f1d23446d74a9d0976507988dac06684b2))
* **deps-dev:** bump jest-runner-eslint from 1.0.0 to 1.1.0 ([#352](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/352)) ([e84c381](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/e84c3814458cec3ac4bf2a8e794708bd0b9e96fa))
* **deps-dev:** bump lint-staged from 12.5.0 to 15.2.7 ([#476](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/476)) ([1c951cd](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/1c951cd2fe9640f4f56124b21f0e33fcde491286))
* **deps-dev:** bump lint-staged from 15.2.7 to 15.2.8 ([#539](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/539)) ([9e2528f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/9e2528ffabe91217d0cd12d634dceb70462b9353))
* **deps-dev:** bump prettier from 2.5.1 to 2.7.1 ([#351](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/351)) ([3881ae4](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/3881ae41bbcaadd921a3c6831cf1a73f7bbc8683))
* **deps-dev:** bump typescript from 4.7.4 to 4.8.3 ([#353](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/353)) ([b0820b7](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b0820b742904a34927146bf388885efc8884f65a))
* **deps-dev:** bump typescript from 4.8.3 to 4.8.4 ([#356](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/356)) ([428d8dd](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/428d8dd539a4bdf204da762a420f43741ae25e78))
* **deps-dev:** bump typescript from 4.8.4 to 4.9.3 ([#410](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/410)) ([4fcd263](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4fcd263b9ea1d33bd99f6e5e89c4c08ce5c851c4))
* **deps-dev:** update eslint-plugin-eslint-plugin to v6.3.0 ([#560](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/560)) ([7459bd6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7459bd67b0056d363e3d53de084642eb79b74944))
* **deps-dev:** update eslint-plugin-eslint-plugin to v6.3.1 ([#561](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/561)) ([434c6fa](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/434c6fa2ed1d8747b28b002ce539fa5ccc2d0921))
* **deps-dev:** update eslint-plugin-eslint-plugin to v6.3.2 ([#570](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/570)) ([a849f64](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/a849f6467ef90ec2f3c988b9e6591b347287a80a))
* **deps-dev:** update eslint-plugin-eslint-plugin to v6.4.0 ([#583](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/583)) ([45385a3](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/45385a3d8de361a82b6a5faada6113272791e56c))
* **deps-dev:** update eslint-plugin-jest to v28.11.0 ([#585](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/585)) ([a33ffb6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/a33ffb6ae735c1fc58c25edab667214f234e2936))
* **deps-dev:** update eslint-plugin-jest to v28.9.0 ([#565](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/565)) ([cf213fb](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/cf213fbab43533f338333b1cb986d4b1041dc51c))
* **deps-dev:** update eslint-plugin-n to v17.12.0 ([#563](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/563)) ([d39e2f0](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/d39e2f0d6f5cbaa495957aa69be74f4c94113148))
* **deps-dev:** update eslint-plugin-n to v17.13.0 ([#566](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/566)) ([b62f234](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b62f2345de7a1d307ff63e761471431cfc2bfb8f))
* **deps-dev:** update eslint-plugin-n to v17.13.1 ([#567](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/567)) ([266ddbb](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/266ddbb03076c05c362a6daecb9382b80cdd7108))
* **deps-dev:** update eslint-plugin-n to v17.13.2 ([#569](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/569)) ([390f51f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/390f51fe07b2d375ec93f52c19a6964637c3ae8c))
* **deps-dev:** update eslint-plugin-n to v17.14.0 ([#575](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/575)) ([fad9049](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/fad904995e2d99a064f40c32b43e35b6371b2e8a))
* **deps-dev:** update eslint-plugin-prettier to v5.2.3 ([#586](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/586)) ([b2095cb](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b2095cbee2a7a10bf90aa5966751240d1cd302e8))
* **deps-dev:** update eslint-plugin-prettier to v5.2.4 ([#600](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/600)) ([fad5029](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/fad50297fc9c368e8e8f7bfa494f0c1a07e5a4db))
* **deps-dev:** update husky to v9.1.7 ([#573](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/573)) ([24fd90a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/24fd90a0262e1521983095f0934e9bb0195b4d23))
* **deps-dev:** update lint-staged to v15.4.3 ([#582](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/582)) ([d1e23e5](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/d1e23e53c162905ecd7e8399bbf6eb9a8aa45d83))
* **deps-dev:** update npm-run-all2 to v6.2.4 ([#558](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/558)) ([2cf1732](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/2cf17322af17311fac773b524fa55589ebe4c9fd))
* **deps-dev:** update npm-run-all2 to v6.2.6 ([#559](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/559)) ([dc32933](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/dc32933c0d61e2a916a96ee21d37d3058976c090))
* **deps-dev:** update prettier to v3.4.1 ([#578](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/578)) ([3fae241](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/3fae2417bb59ae82a56d3f82d8e28a09eba26421))
* **deps-dev:** update prettier to v3.4.2 ([#580](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/580)) ([7219528](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7219528cc595d408bac32a0912dab7e81f55eb3c))
* **deps-dev:** update prettier to v3.5.0 ([#588](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/588)) ([5da83c4](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5da83c4cd1e673b7687a466c58d9972bb433e71c))
* **deps:** bump actions/checkout from 2 to 3 ([#279](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/279)) ([49e2ce3](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/49e2ce3843b349410bff54b075de6ce111b7e16d))
* **deps:** bump actions/checkout from 3 to 4 ([#461](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/461)) ([62af490](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/62af4905947b46d19167f0e5e53937db2e7565d2))
* **deps:** bump actions/checkout from 3 to 4 ([#500](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/500)) ([aea6d94](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/aea6d94f8391da80270949e76bf39c5ec2c17baf))
* **deps:** bump actions/setup-node from 2 to 3 ([#344](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/344)) ([5afbb72](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5afbb723e38265138c4393b0429644a9c06d7d9e))
* **deps:** bump actions/setup-node from 3 to 4 ([#460](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/460)) ([8c74b9b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/8c74b9bda97bbb13b744d40f6f8b78174f5792b2))
* **deps:** bump actions/setup-node from 3 to 4 ([#499](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/499)) ([84334f4](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/84334f4ba5b2d8301ed6c41dc82f55c01f981b6c))
* **deps:** bump codecov/codecov-action from 3 to 4 ([#459](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/459)) ([19b21b4](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/19b21b413b4a6c5fa52b8a0b5882f96c1519ae3f))
* **deps:** bump cross-spawn from 7.0.3 to 7.0.6 ([#568](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/568)) ([f33f82e](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/f33f82e03ee949d2864e266aedfe5da9762ad540))
* **deps:** bump cycjimmy/semantic-release-action from 3 to 4 ([#462](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/462)) ([bf75e4d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/bf75e4d9b5cdbb07018480c291473fde9b33aedc))
* **deps:** bump json5 from 2.2.1 to 2.2.3 ([#425](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/425)) ([6fcf8e3](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/6fcf8e3ed771328b9da2c84849ec5bbc3d56eddd))
* **deps:** bump lodash from 4.17.15 to 4.17.19 ([ac57a5f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ac57a5f844e3cedde689bd69fbb6289705302a93))
* **deps:** bump lodash from 4.17.15 to 4.17.19 ([cbfb8a6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/cbfb8a604e540592997cb69a1bdd257f84b1811f))
* **deps:** bump styfle/cancel-workflow-action from 0.10.0 to 0.10.1 ([#372](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/372)) ([8875343](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/887534373988d6c4192b5c5bf62e09c358ef4821))
* **deps:** bump styfle/cancel-workflow-action from 0.9.1 to 0.10.0 ([#318](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/318)) ([8c44b64](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/8c44b643e01ac32d743c8fb95cddc18549a40cfb))
* **deps:** switch from dependabot to renovate using shared eslint community configuration ([#537](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/537)) ([30efed7](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/30efed7cf9e8b49d6368df9ae8be84b9619cf621))
* **deps:** update @eslint-community/eslint-utils to v4.4.1 ([#562](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/562)) ([5c3628d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5c3628de60c4a5f6cbcd9240264397c5f7821f16))
* **deps:** update globals to v15.12.0 ([#564](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/564)) ([c8632d1](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/c8632d1558f87c5c4761a9e7b5a7f277c8bdfda6))
* **deps:** update globals to v15.13.0 ([#579](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/579)) ([75defcf](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/75defcf8c6262f42124a7dba7e4f862be0ea9d0f))
* **deps:** update globals to v15.14.0 ([#584](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/584)) ([846ad48](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/846ad4861b5f24cd45093fffb2db48a37473553d))
* **deps:** update typescript to v5.7.3 ([#589](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/589)) ([79b0eff](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/79b0eff3f660f9e7a6c30aa4a29fc1391df39059))
* enable strict mode in all files ([#81](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/81)) ([0095432](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/0095432c7af75138a1b6438ce16bc4594ac9d4fd))
* file extension missing ([#519](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/519)) ([94c9834](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/94c983483596bca2baa6c710273d348f8cf98d58))
* fix branch of rule docs link URL to `main` ([#381](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/381)) ([70f0012](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/70f00122895b30f6b912122e25dd7686418f7318))
* fix format.yml ([#507](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/507)) ([948c097](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/948c09776e23e7dc38f155b268dcc002d59a957b))
* fix npm audit vulnerabilities and update caniuse ([21382f8](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/21382f899cc685813bd6cef4817fac7db2cc5b3b))
* fix typos in some comments ([12dfa12](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/12dfa129a8cbe731106231bf3075ebbf5d0de97d))
* ignore package-lock.json ([#78](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/78)) ([2a2d2e9](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/2a2d2e9e6ca0441d8fe0536e27903e92065ba0ea))
* include .travis.yml in .npmignore ([#83](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/83)) ([f2c405d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/f2c405dac217d4b0873cd84d6330b0a89eb9aa7f))
* lint all files by default and add `--report-unused-disable-directives` flag ([#198](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/198)) ([81d0f94](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/81d0f94e36bdb8f7f046d358a81da5c1c5548ff6))
* lookup promise statics from object instead of array ([#131](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/131)) ([9b0cbd1](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/9b0cbd1a06e295d0348ddf06c517af695a133ce0))
* **main:** release 7.1.0 ([#510](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/510)) ([d0ff43f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/d0ff43f07cbc610a9bb755b713fe49aea1c593f5))
* **main:** release 7.2.0 ([#538](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/538)) ([5b987c6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5b987c6c0a3b2401bcf66f195b391bb1756e2f3c))
* **main:** release 7.2.1 ([#571](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/571)) ([6bda064](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/6bda06446b51a74309e18fab4f2bb758dd6aa714))
* **main:** release 7.3.0 ([#576](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/576)) ([f1dd605](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/f1dd60596f7cf0d01eb1d208f2cfd07ff76ffa57))
* migrate all message to messageId ([#482](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/482)) ([b0fc13b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b0fc13b278a7dbb0452d86247ef7dd9191d149e7))
* **package:** add package-lock.json ([#130](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/130)) ([b5a6423](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b5a6423ca7edebfd48ffeb324357dddc54fc00ac))
* **package:** explicitly declare js module type ([#592](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/592)) ([b19e133](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b19e133b438a8e3bf6ff99f0abd14b234f061ee2))
* **package:** update ESLint plugins ([#141](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/141)) ([56434a6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/56434a6443821c9587180394f273863db5c26123))
* **package:** update test dependencies ([bcb6808](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/bcb6808061c9f98360d02410f933bb5054f53ddb))
* **package:** update to eslint v4 ([#76](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/76)) ([4941c5d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/4941c5d9515ff6b9f7daa0766155c124836dc1b5)), closes [#63](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/63)
* **package:** update to mocha v5 ([#77](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/77)) ([a2edaa1](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/a2edaa1a5dc7e1e81326957ccb0c3472cedacc2a))
* **package:** update to prettier@1.13.0 ([#135](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/135)) ([54f1958](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/54f1958f1955942e736374a029eabae4263ee0c3))
* **package:** update to prettier@1.14 ([1e15366](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/1e153665f92672411e5acb733910c6962fce30ef))
* remove `styfle/cancel-workflow-action` usage ([#439](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/439)) ([0b50079](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/0b50079d21a31739fb5254841c7e3ec1c9bcfd4c))
* remove old Travis CI badge and update `.npmignore` ([#242](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/242)) ([91345d9](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/91345d98307b44ee97aafb59d97f76dbf24d788d))
* resolve eslint-plugin-eslint-plugin warnings ([#93](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/93)) ([15c0aa5](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/15c0aa593f5eb9959420d7f0040f5db991e1a79b)), closes [#89](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/89)
* simplify linter configuration ([#134](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/134)) ([586d9eb](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/586d9ebfda80b3ca22f6b10af9cc165bb2dc2cf0))
* sort `package.json` ([#385](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/385)) ([72cfdc8](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/72cfdc8b512a835a6d4cbc3ea2079bc4d234a6f2))
* support ESLint v5 ([#144](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/144)) ([ff1635d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ff1635d83c0d2550b637ff0b3c521dcc2e7f22b0))
* update .npmignore ([7f2d0a0](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7f2d0a0f25160dd77137d3f4056c7791ca897285))
* update @typescript-eslint/parser to v7.18.0 ([#545](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/545)) ([5744e60](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/5744e6061059acbd2fe736bd74cd50c5d3fd2808))
* update `eslint-plugin-eslint-plugin` to latest ([3f5520f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/3f5520f13c80a945b23b7dee65036fc417cacd94))
* update `eslint-plugin-eslint-plugin` to latest ([8dd426a](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/8dd426aefc6609e5f95423aeb12cd780742d8c8f))
* update code formatting tools ([#96](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/96)) ([834c69d](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/834c69d26df35c2eccfdd4da702b7b72b4e35edc)), closes [#95](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/95)
* update dependencies ([#350](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/350)) ([75899ac](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/75899acc937a94c83a10f194b0ff56448eee3424))
* update dependencies to latest minor version ([bc65288](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/bc65288afd126ddc05ac64356ca985b3df649dbb))
* update dependencies to latest minor version ([26a4ab8](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/26a4ab84da4f357a57821be6f66bf22318990143))
* update dependency eslint-plugin-n to v17.11.0 ([#556](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/556)) ([bbd048b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/bbd048bdd13e3004f56863fae8221e4e8fcaac77))
* update dependency eslint-plugin-n to v17.11.1 ([#557](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/557)) ([e545254](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/e5452545904462a5c5574ed506d4d9d6afca6701))
* update dependency globals to v15.11.0 ([#555](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/555)) ([9151db8](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/9151db8c21c9566ad7c87aad55a75fedba6cb980))
* update dependency typescript to v5.6.3 ([#554](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/554)) ([ab55120](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ab55120d425047594db18c4cfb3f5c1f6bd44b61))
* update devDeps ([e9a0dd6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/e9a0dd6462edbdc40fb460d40ded086d597c92da))
* update devDeps. and lint as per latest prettier ([1327f69](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/1327f6956a23b8cc974f1a61ef8e38fbe1579589))
* update eslint to v8.57.1 ([#551](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/551)) ([38e2757](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/38e27571e8583eb014b167fccc37f9b5a90af52f))
* update eslint-plugin-jest to v28.8.3 ([#548](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/548)) ([89f2578](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/89f257856b919fac252c2a6e742f2c385c7cf25e))
* update eslint-plugin-n to v17.10.3 ([#552](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/552)) ([2d738fe](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/2d738fedfc162215140c374a6de4a2d2d13c0472))
* update globals to v15.10.0 ([#553](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/553)) ([b871314](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/b8713140b2e42180a936b21d503273f2aacaea4a))
* update husky to v9.1.6 ([#547](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/547)) ([1e8d18f](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/1e8d18f56a889d4f1ba327c3554bec84c8e9fcb2))
* update jest ([3d3e8d5](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/3d3e8d5fe957ba501c8438003526401e9c06d237))
* update lint-staged to v15.2.10 ([#544](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/544)) ([7d46b3b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/7d46b3b0eced0ff31a4e8492b70cd4f363f02d2e))
* Update node versions to align with eslint v9 ([#484](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/484)) ([8a981d2](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/8a981d293565e4e1c1fcedd52c18e2809322ed4e))
* update npm-run-all2 to v6.2.3 ([#550](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/550)) ([14cd4c0](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/14cd4c098e50a6c5d14becafc9f337237015a5cc))
* update typescript to ~5.6.0 ([#549](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/549)) ([ebcdd8b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ebcdd8bc6e2fed8164abf78650a7d45689aa04dc))
* update typescript to ~5.7.0 ([#577](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/577)) ([04d0b2b](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/04d0b2bbed91c44baec0ed1bbe5bf3ac051f2f8f))
* updated prettier ([0bacbc3](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/0bacbc3deebf7523b7dafd787e3368f6be81f8ea))
* use Jest for tests and linting ([#113](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/issues/113)) ([44c7355](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/44c73556f3ae45f04dc0c68d6b0f135c12ad7ce4))
* Use setup-node NPM caching ([ad955c6](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/ad955c61f7d7032b763e77848c4e740e3398f748))
* Use setup-node NPM caching ([f57fd3c](https://github.com/JoshuaKGoldberg/eslint-plugin-promise/commit/f57fd3c681c564d50e462e408dcddbc6d972d3dd))

## [7.3.0](https://github.com/eslint-community/eslint-plugin-promise/compare/v7.2.1...v7.3.0) (2026-04-27)


### 🌟 Features

* **`no-promise-in-callback`:** add `exemptDeclarations` option ([#513](https://github.com/eslint-community/eslint-plugin-promise/issues/513)) ([550524f](https://github.com/eslint-community/eslint-plugin-promise/commit/550524f2e07e392926b1e6330c7e21b5f91529ad))
* add support for ESLint v10 ([#617](https://github.com/eslint-community/eslint-plugin-promise/issues/617)) ([6096821](https://github.com/eslint-community/eslint-plugin-promise/commit/6096821370e7662a61abcee2822f9b1750fb53c4))


### 🩹 Fixes

* **no-native:** fix to report `Promise` usage in eslint v9 or later ([#619](https://github.com/eslint-community/eslint-plugin-promise/issues/619)) ([1230ced](https://github.com/eslint-community/eslint-plugin-promise/commit/1230ced57c422196735fa5f4c404d4c46c620c14))


### 🧹 Chores

* add missing `'use strict'` directive ([#593](https://github.com/eslint-community/eslint-plugin-promise/issues/593)) ([4cd7ea1](https://github.com/eslint-community/eslint-plugin-promise/commit/4cd7ea162c946604f953199393fa66ea47dce872))
* **deps-dev:** update eslint-plugin-eslint-plugin to v6.4.0 ([#583](https://github.com/eslint-community/eslint-plugin-promise/issues/583)) ([45385a3](https://github.com/eslint-community/eslint-plugin-promise/commit/45385a3d8de361a82b6a5faada6113272791e56c))
* **deps-dev:** update eslint-plugin-jest to v28.11.0 ([#585](https://github.com/eslint-community/eslint-plugin-promise/issues/585)) ([a33ffb6](https://github.com/eslint-community/eslint-plugin-promise/commit/a33ffb6ae735c1fc58c25edab667214f234e2936))
* **deps-dev:** update eslint-plugin-n to v17.14.0 ([#575](https://github.com/eslint-community/eslint-plugin-promise/issues/575)) ([fad9049](https://github.com/eslint-community/eslint-plugin-promise/commit/fad904995e2d99a064f40c32b43e35b6371b2e8a))
* **deps-dev:** update eslint-plugin-prettier to v5.2.3 ([#586](https://github.com/eslint-community/eslint-plugin-promise/issues/586)) ([b2095cb](https://github.com/eslint-community/eslint-plugin-promise/commit/b2095cbee2a7a10bf90aa5966751240d1cd302e8))
* **deps-dev:** update eslint-plugin-prettier to v5.2.4 ([#600](https://github.com/eslint-community/eslint-plugin-promise/issues/600)) ([fad5029](https://github.com/eslint-community/eslint-plugin-promise/commit/fad50297fc9c368e8e8f7bfa494f0c1a07e5a4db))
* **deps-dev:** update lint-staged to v15.4.3 ([#582](https://github.com/eslint-community/eslint-plugin-promise/issues/582)) ([d1e23e5](https://github.com/eslint-community/eslint-plugin-promise/commit/d1e23e53c162905ecd7e8399bbf6eb9a8aa45d83))
* **deps-dev:** update prettier to v3.4.1 ([#578](https://github.com/eslint-community/eslint-plugin-promise/issues/578)) ([3fae241](https://github.com/eslint-community/eslint-plugin-promise/commit/3fae2417bb59ae82a56d3f82d8e28a09eba26421))
* **deps-dev:** update prettier to v3.4.2 ([#580](https://github.com/eslint-community/eslint-plugin-promise/issues/580)) ([7219528](https://github.com/eslint-community/eslint-plugin-promise/commit/7219528cc595d408bac32a0912dab7e81f55eb3c))
* **deps-dev:** update prettier to v3.5.0 ([#588](https://github.com/eslint-community/eslint-plugin-promise/issues/588)) ([5da83c4](https://github.com/eslint-community/eslint-plugin-promise/commit/5da83c4cd1e673b7687a466c58d9972bb433e71c))
* **deps:** update globals to v15.13.0 ([#579](https://github.com/eslint-community/eslint-plugin-promise/issues/579)) ([75defcf](https://github.com/eslint-community/eslint-plugin-promise/commit/75defcf8c6262f42124a7dba7e4f862be0ea9d0f))
* **deps:** update globals to v15.14.0 ([#584](https://github.com/eslint-community/eslint-plugin-promise/issues/584)) ([846ad48](https://github.com/eslint-community/eslint-plugin-promise/commit/846ad4861b5f24cd45093fffb2db48a37473553d))
* **deps:** update typescript to v5.7.3 ([#589](https://github.com/eslint-community/eslint-plugin-promise/issues/589)) ([79b0eff](https://github.com/eslint-community/eslint-plugin-promise/commit/79b0eff3f660f9e7a6c30aa4a29fc1391df39059))
* **package:** explicitly declare js module type ([#592](https://github.com/eslint-community/eslint-plugin-promise/issues/592)) ([b19e133](https://github.com/eslint-community/eslint-plugin-promise/commit/b19e133b438a8e3bf6ff99f0abd14b234f061ee2))
* update typescript to ~5.7.0 ([#577](https://github.com/eslint-community/eslint-plugin-promise/issues/577)) ([04d0b2b](https://github.com/eslint-community/eslint-plugin-promise/commit/04d0b2bbed91c44baec0ed1bbe5bf3ac051f2f8f))

## [7.2.1](https://github.com/eslint-community/eslint-plugin-promise/compare/v7.2.0...v7.2.1) (2024-11-26)


### 🩹 Fixes

* **`no-callback-in-promise`:** false triggering of callback ([#574](https://github.com/eslint-community/eslint-plugin-promise/issues/574)) ([8324564](https://github.com/eslint-community/eslint-plugin-promise/commit/83245645a1731b8720ba4b17951f0e98567f449c))


### 🧹 Chores

* **deps-dev:** update husky to v9.1.7 ([#573](https://github.com/eslint-community/eslint-plugin-promise/issues/573)) ([24fd90a](https://github.com/eslint-community/eslint-plugin-promise/commit/24fd90a0262e1521983095f0934e9bb0195b4d23))
* **deps:** bump cross-spawn from 7.0.3 to 7.0.6 ([#568](https://github.com/eslint-community/eslint-plugin-promise/issues/568)) ([f33f82e](https://github.com/eslint-community/eslint-plugin-promise/commit/f33f82e03ee949d2864e266aedfe5da9762ad540))

## [7.2.0](https://github.com/eslint-community/eslint-plugin-promise/compare/v7.1.0...v7.2.0) (2024-11-25)


### 🌟 Features

* **`no-callback-in-promise`:** add `timeoutsErr` option ([#514](https://github.com/eslint-community/eslint-plugin-promise/issues/514)) ([907753f](https://github.com/eslint-community/eslint-plugin-promise/commit/907753f4b6108ba78b93571a40b6f1384b3c6899))
* **`valid-params`:** add `exclude` option ([#515](https://github.com/eslint-community/eslint-plugin-promise/issues/515)) ([7ff2cb9](https://github.com/eslint-community/eslint-plugin-promise/commit/7ff2cb9298f5dd0b4dae82321605d04e50ca935b))
* **always-return:** add `ignoreAssignmentVariable` option ([#518](https://github.com/eslint-community/eslint-plugin-promise/issues/518)) ([701279c](https://github.com/eslint-community/eslint-plugin-promise/commit/701279c573437598e86873f48b4f5cf6432ae38e))
* **catch-or-return:** add `allowThenStrict` option ([#522](https://github.com/eslint-community/eslint-plugin-promise/issues/522)) ([53be970](https://github.com/eslint-community/eslint-plugin-promise/commit/53be970e91023a104ce3ef2918b3ee80ef265f27))
* new rule `prefer-catch` ([#525](https://github.com/eslint-community/eslint-plugin-promise/issues/525)) ([05c8a93](https://github.com/eslint-community/eslint-plugin-promise/commit/05c8a930893e6abff2a0a7e1fb82a1543c19df9f))


### 🩹 Fixes

* permit appropriate computed member expressions and prototype access ([#535](https://github.com/eslint-community/eslint-plugin-promise/issues/535)) ([4de9d43](https://github.com/eslint-community/eslint-plugin-promise/commit/4de9d43b84f1beb166a7ba779a4da9d732d0eab3))


### 🧹 Chores

* **deps-dev:** bump eslint-plugin-jest from 28.6.0 to 28.8.0 ([#536](https://github.com/eslint-community/eslint-plugin-promise/issues/536)) ([80741f8](https://github.com/eslint-community/eslint-plugin-promise/commit/80741f849db526cad362cfc976c69a1df036a6c6))
* **deps-dev:** bump eslint-plugin-n from 17.9.0 to 17.10.2 ([#529](https://github.com/eslint-community/eslint-plugin-promise/issues/529)) ([a646010](https://github.com/eslint-community/eslint-plugin-promise/commit/a646010a7700a87c0fcc8aa0bb0d580bd6a14fd4))
* **deps-dev:** bump globals from 15.8.0 to 15.9.0 ([#527](https://github.com/eslint-community/eslint-plugin-promise/issues/527)) ([b8afe92](https://github.com/eslint-community/eslint-plugin-promise/commit/b8afe920bd3be1120f5effb4a9a71451a3e71c24))
* **deps-dev:** bump husky from 9.1.2 to 9.1.4 ([#524](https://github.com/eslint-community/eslint-plugin-promise/issues/524)) ([b8fdb9f](https://github.com/eslint-community/eslint-plugin-promise/commit/b8fdb9f1d23446d74a9d0976507988dac06684b2))
* **deps-dev:** bump lint-staged from 15.2.7 to 15.2.8 ([#539](https://github.com/eslint-community/eslint-plugin-promise/issues/539)) ([9e2528f](https://github.com/eslint-community/eslint-plugin-promise/commit/9e2528ffabe91217d0cd12d634dceb70462b9353))
* **deps-dev:** update eslint-plugin-eslint-plugin to v6.3.0 ([#560](https://github.com/eslint-community/eslint-plugin-promise/issues/560)) ([7459bd6](https://github.com/eslint-community/eslint-plugin-promise/commit/7459bd67b0056d363e3d53de084642eb79b74944))
* **deps-dev:** update eslint-plugin-eslint-plugin to v6.3.1 ([#561](https://github.com/eslint-community/eslint-plugin-promise/issues/561)) ([434c6fa](https://github.com/eslint-community/eslint-plugin-promise/commit/434c6fa2ed1d8747b28b002ce539fa5ccc2d0921))
* **deps-dev:** update eslint-plugin-eslint-plugin to v6.3.2 ([#570](https://github.com/eslint-community/eslint-plugin-promise/issues/570)) ([a849f64](https://github.com/eslint-community/eslint-plugin-promise/commit/a849f6467ef90ec2f3c988b9e6591b347287a80a))
* **deps-dev:** update eslint-plugin-jest to v28.9.0 ([#565](https://github.com/eslint-community/eslint-plugin-promise/issues/565)) ([cf213fb](https://github.com/eslint-community/eslint-plugin-promise/commit/cf213fbab43533f338333b1cb986d4b1041dc51c))
* **deps-dev:** update eslint-plugin-n to v17.12.0 ([#563](https://github.com/eslint-community/eslint-plugin-promise/issues/563)) ([d39e2f0](https://github.com/eslint-community/eslint-plugin-promise/commit/d39e2f0d6f5cbaa495957aa69be74f4c94113148))
* **deps-dev:** update eslint-plugin-n to v17.13.0 ([#566](https://github.com/eslint-community/eslint-plugin-promise/issues/566)) ([b62f234](https://github.com/eslint-community/eslint-plugin-promise/commit/b62f2345de7a1d307ff63e761471431cfc2bfb8f))
* **deps-dev:** update eslint-plugin-n to v17.13.1 ([#567](https://github.com/eslint-community/eslint-plugin-promise/issues/567)) ([266ddbb](https://github.com/eslint-community/eslint-plugin-promise/commit/266ddbb03076c05c362a6daecb9382b80cdd7108))
* **deps-dev:** update eslint-plugin-n to v17.13.2 ([#569](https://github.com/eslint-community/eslint-plugin-promise/issues/569)) ([390f51f](https://github.com/eslint-community/eslint-plugin-promise/commit/390f51fe07b2d375ec93f52c19a6964637c3ae8c))
* **deps-dev:** update npm-run-all2 to v6.2.4 ([#558](https://github.com/eslint-community/eslint-plugin-promise/issues/558)) ([2cf1732](https://github.com/eslint-community/eslint-plugin-promise/commit/2cf17322af17311fac773b524fa55589ebe4c9fd))
* **deps-dev:** update npm-run-all2 to v6.2.6 ([#559](https://github.com/eslint-community/eslint-plugin-promise/issues/559)) ([dc32933](https://github.com/eslint-community/eslint-plugin-promise/commit/dc32933c0d61e2a916a96ee21d37d3058976c090))
* **deps:** switch from dependabot to renovate using shared eslint community configuration ([#537](https://github.com/eslint-community/eslint-plugin-promise/issues/537)) ([30efed7](https://github.com/eslint-community/eslint-plugin-promise/commit/30efed7cf9e8b49d6368df9ae8be84b9619cf621))
* **deps:** update @eslint-community/eslint-utils to v4.4.1 ([#562](https://github.com/eslint-community/eslint-plugin-promise/issues/562)) ([5c3628d](https://github.com/eslint-community/eslint-plugin-promise/commit/5c3628de60c4a5f6cbcd9240264397c5f7821f16))
* **deps:** update globals to v15.12.0 ([#564](https://github.com/eslint-community/eslint-plugin-promise/issues/564)) ([c8632d1](https://github.com/eslint-community/eslint-plugin-promise/commit/c8632d1558f87c5c4761a9e7b5a7f277c8bdfda6))
* update @typescript-eslint/parser to v7.18.0 ([#545](https://github.com/eslint-community/eslint-plugin-promise/issues/545)) ([5744e60](https://github.com/eslint-community/eslint-plugin-promise/commit/5744e6061059acbd2fe736bd74cd50c5d3fd2808))
* update dependency eslint-plugin-n to v17.11.0 ([#556](https://github.com/eslint-community/eslint-plugin-promise/issues/556)) ([bbd048b](https://github.com/eslint-community/eslint-plugin-promise/commit/bbd048bdd13e3004f56863fae8221e4e8fcaac77))
* update dependency eslint-plugin-n to v17.11.1 ([#557](https://github.com/eslint-community/eslint-plugin-promise/issues/557)) ([e545254](https://github.com/eslint-community/eslint-plugin-promise/commit/e5452545904462a5c5574ed506d4d9d6afca6701))
* update dependency globals to v15.11.0 ([#555](https://github.com/eslint-community/eslint-plugin-promise/issues/555)) ([9151db8](https://github.com/eslint-community/eslint-plugin-promise/commit/9151db8c21c9566ad7c87aad55a75fedba6cb980))
* update dependency typescript to v5.6.3 ([#554](https://github.com/eslint-community/eslint-plugin-promise/issues/554)) ([ab55120](https://github.com/eslint-community/eslint-plugin-promise/commit/ab55120d425047594db18c4cfb3f5c1f6bd44b61))
* update eslint to v8.57.1 ([#551](https://github.com/eslint-community/eslint-plugin-promise/issues/551)) ([38e2757](https://github.com/eslint-community/eslint-plugin-promise/commit/38e27571e8583eb014b167fccc37f9b5a90af52f))
* update eslint-plugin-jest to v28.8.3 ([#548](https://github.com/eslint-community/eslint-plugin-promise/issues/548)) ([89f2578](https://github.com/eslint-community/eslint-plugin-promise/commit/89f257856b919fac252c2a6e742f2c385c7cf25e))
* update eslint-plugin-n to v17.10.3 ([#552](https://github.com/eslint-community/eslint-plugin-promise/issues/552)) ([2d738fe](https://github.com/eslint-community/eslint-plugin-promise/commit/2d738fedfc162215140c374a6de4a2d2d13c0472))
* update globals to v15.10.0 ([#553](https://github.com/eslint-community/eslint-plugin-promise/issues/553)) ([b871314](https://github.com/eslint-community/eslint-plugin-promise/commit/b8713140b2e42180a936b21d503273f2aacaea4a))
* update husky to v9.1.6 ([#547](https://github.com/eslint-community/eslint-plugin-promise/issues/547)) ([1e8d18f](https://github.com/eslint-community/eslint-plugin-promise/commit/1e8d18f56a889d4f1ba327c3554bec84c8e9fcb2))
* update lint-staged to v15.2.10 ([#544](https://github.com/eslint-community/eslint-plugin-promise/issues/544)) ([7d46b3b](https://github.com/eslint-community/eslint-plugin-promise/commit/7d46b3b0eced0ff31a4e8492b70cd4f363f02d2e))
* update npm-run-all2 to v6.2.3 ([#550](https://github.com/eslint-community/eslint-plugin-promise/issues/550)) ([14cd4c0](https://github.com/eslint-community/eslint-plugin-promise/commit/14cd4c098e50a6c5d14becafc9f337237015a5cc))
* update typescript to ~5.6.0 ([#549](https://github.com/eslint-community/eslint-plugin-promise/issues/549)) ([ebcdd8b](https://github.com/eslint-community/eslint-plugin-promise/commit/ebcdd8bc6e2fed8164abf78650a7d45689aa04dc))

## [7.1.0](https://github.com/eslint-community/eslint-plugin-promise/compare/v7.0.0...v7.1.0) (2024-08-06)


### 🌟 Features

* **`catch-or-return`, `prefer-await-to-then`:** do not report Cypress commands ([#495](https://github.com/eslint-community/eslint-plugin-promise/issues/495)) ([943f162](https://github.com/eslint-community/eslint-plugin-promise/commit/943f16290f11af9717612e079646802e22310290))
* **`prefer-await-to-then`:** ignore constructor scope unless with `strict` option ([#496](https://github.com/eslint-community/eslint-plugin-promise/issues/496)) ([7bffb7a](https://github.com/eslint-community/eslint-plugin-promise/commit/7bffb7a666ed74a876ba3a6c482c36ea6f9d6d07))
* new rule `spec-only` to check for non-spec Promise methods ([#502](https://github.com/eslint-community/eslint-plugin-promise/issues/502)) ([d6e9de1](https://github.com/eslint-community/eslint-plugin-promise/commit/d6e9de1f9c81194b775484ed0299dc5cc4898684))


### 📚 Documentation

* fixes the CI readme badge ([#511](https://github.com/eslint-community/eslint-plugin-promise/issues/511)) ([030a3be](https://github.com/eslint-community/eslint-plugin-promise/commit/030a3be890d371381ef13258806f97ec62d6b4fd))
* supply missing docs ([#503](https://github.com/eslint-community/eslint-plugin-promise/issues/503)) ([602d825](https://github.com/eslint-community/eslint-plugin-promise/commit/602d8254871e46c9d1808ee1a3a2c48cb7493334))


### 🧹 Chores

* bump dev dependencies ([#483](https://github.com/eslint-community/eslint-plugin-promise/issues/483)) ([197ae4e](https://github.com/eslint-community/eslint-plugin-promise/commit/197ae4eb4f05f34c54189102871d969379595a54))
* **deps-dev:** bump husky from 9.1.1 to 9.1.2 ([#516](https://github.com/eslint-community/eslint-plugin-promise/issues/516)) ([ab8e7a0](https://github.com/eslint-community/eslint-plugin-promise/commit/ab8e7a0d4fc8bde63fb6a6bb1e9743152778c4ee))
* file extension missing ([#519](https://github.com/eslint-community/eslint-plugin-promise/issues/519)) ([94c9834](https://github.com/eslint-community/eslint-plugin-promise/commit/94c983483596bca2baa6c710273d348f8cf98d58))
* fix format.yml ([#507](https://github.com/eslint-community/eslint-plugin-promise/issues/507)) ([948c097](https://github.com/eslint-community/eslint-plugin-promise/commit/948c09776e23e7dc38f155b268dcc002d59a957b))

## 6.0.2

- Added tests for @typescript-eslint/parser support

## 6.0.1

- Fixed @typescript-eslint/parser issue #331, #205

## 6.0.0

- Dropped node 10 from engines #231
- Updated a ton of deps #236, #237, #235, #234
- ESLint 8 support #219

## 5.2.0

- Updated `param-names` rule to allow for unused params

## 5.1.1

- Updated docs to include `no-callback-in-promise` reasons #215

## 5.1.0

- Included `catch()` and `finally()` in `prefer-await-to-then` #196
- Added some additional tests and upgraded some dev deps #196
- Exempted array methods in prefer-await-to-callbacks
  ([#212](https://github.com/eslint-community/eslint-plugin-promise/issues/212))

## 5.0.0

- ESLint 7.0 Support

## 4.3.1.

- Updated and applied prettier

## 4.3.0

- https://github.com/eslint-community/eslint-plugin-promise/pull/202
- Updated jest

## 4.2.2

- Added license
- Dependabot security updates

## 4.2.1

- Added more use cases to `no-return-wrap`

## 4.0.1

- Remove `promise/param-names` fixer
  ([#146](https://github.com/eslint-community/eslint-plugin-promise/pull/146))

## 4.0.0

- Added fixer for `promise/no-new-statics` rule
  ([#133](https://github.com/eslint-community/eslint-plugin-promise/pull/133))
- Support ESLint v5
  ([#144](https://github.com/eslint-community/eslint-plugin-promise/pull/144))

This is a breaking change that drops support for Node v4. In order to use ESLint
v5 and eslint-plugin-promise v4, you must use Node >=6.

## 3.8.0

- Removed `promise/avoid-new` from recommended configuration
  ([#119](https://github.com/eslint-community/eslint-plugin-promise/pull/119))
- Ignored event listener callbacks in `promise/prefer-await-to-callbacks`
  ([#117](https://github.com/eslint-community/eslint-plugin-promise/pull/117))
- Ignored top-level awaits in `promise/prefer-await-to-then`
  ([#126](https://github.com/eslint-community/eslint-plugin-promise/pull/126))
- Added docs for `promise/no-nesting` and `promise/prefer-await-to-then`
  ([#120](https://github.com/eslint-community/eslint-plugin-promise/pull/120))
  ([#121](https://github.com/eslint-community/eslint-plugin-promise/pull/121))

## 3.7.0

- Added `promise/valid-params` rule
  ([#85](https://github.com/eslint-community/eslint-plugin-promise/pull/85))
- Added `promise/no-new-statics` rule
  ([#82](https://github.com/eslint-community/eslint-plugin-promise/pull/82))
- Added fixer for `promise/param-names` rule
  ([#99](https://github.com/eslint-community/eslint-plugin-promise/pull/99))
- Added rule documentation to each rule
  ([#91](https://github.com/eslint-community/eslint-plugin-promise/pull/91))

## 3.6.0

- Added `['catch']` support in `catch-or-return`
- Added `no-return-in-finally` rule
- Fixed some formatting in the docs
- Added `allowReject` option to `no-return-wrap`
- Added exceptions for `no-callback-in-promise`

## 3.5.0

- Added support for recommended settings using
  `extends: plugin:promise/recommended`

## 3.4.2

- Fixed always return false positive with ternary (#31)

## 3.4.1

- fixed #49

## 3.4.0

- new rule: avoid-new
- new rule: no-promise-in-callback
- new rule: no-callback-in-promise
- new rule: no-nesting

## 3.3.2

- Removed eslint from peerDeps

## 3.3.1

- Updated engines with proper stuff
- Fixed bug for unreachable code

## 3.3.0

- Rule: `prefer-async-to-callbacks` added
- Rule: `prefer-async-to-then` added

## 3.2.1

- Fix: `no-return-wrap` rule missing from index.js

## 3.2.0

- Added `no-return-wrap` rule

## 3.1.0

- Added multiple terminationMethods

## 3.0.1

- Removed deprecated `always-catch` rule
- FIX: always-return error with "fn && fn()"

## 3.0.0

- Updated column and line numbers
- Added flow analysis for better handling of if statements

## 2.0.1

- Fixed type in docs

## 2.0.0

- ESLint 3.0 Support

## 1.3.2

- Updated tests to run on eslint 2.0
- Fixed some issues with `no-native` rule

## 1.3.1

- Actually added `no-native` rule

## 1.3.0

- Added `no-native` rule

## 1.2.0

- Allow `throw` in `always-return` rule
- Added `terminationMethod` option to `catch-or-return` rule

## 1.1.0

- Added `catch-or-return` rule

## 1.0.8

- Fixed crash issues

## 1.0.0 - 1.0.7

- Lots of basic feature updates and doc changes
