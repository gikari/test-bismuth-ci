<!--
  SPDX-FileCopyrightText: none
  SPDX-License-Identifier: MIT
-->

# Changelog

## 1.0.0 (2021-10-03)


### ⚠ BREAKING CHANGES

* **action:** This will break already binded shortcuts
* Using description strings for configuration was unsafe: we could potentially introduce forbidden characters. Also if we wanted to change she description of the shortcut, we would break the shortcut configuration on the user side. Now it is only possible with the change of the unique config string.
* This completely changes how are shortcuts are interpreted by the script. Instead of using the complicated system, where up, down, left and right keys (hjkl) were used dynamically depended on the mode (directional, dwm), we just put all the possible shortcuts in the list. This increases the user's flexibility to bind shortcuts however they want and also reduces the code complexity.
* use esbuild for compiling script
* forward mouse poller
* compile as module

### Features

* :art: Remove git rev from metadata description ([5425c63](https://www.github.com/gikari/test-bismuth-ci/commit/5425c637d2a7647801050a2227cfe03f4b2ad523))
* :bug: use unique key strings instead of description for shortcuts configuration ([5416912](https://www.github.com/gikari/test-bismuth-ci/commit/5416912efdca0acfd892ab4b5f45e2015b0b16f0))
* :building_construction: lean out the shortcuts definitions ([92d57cc](https://www.github.com/gikari/test-bismuth-ci/commit/92d57cc82b993dfd7522a8fb424f6328116d01c4))
* :memo: add issues' templates ([e59b3b2](https://www.github.com/gikari/test-bismuth-ci/commit/e59b3b2965dc9f07c19fd6d7b0d10dac906cc3d0))
* :sparkles: add basic husky hook ([3e7f3d3](https://www.github.com/gikari/test-bismuth-ci/commit/3e7f3d39b5ef4d992100472579fab4adc42c1602))
* :sparkles: add jest as unit testing framework ([caa1d25](https://www.github.com/gikari/test-bismuth-ci/commit/caa1d258582f97ecf66775d3390bc656a3a3fb25))
* :sparkles: add Krohnkite shortcuts import script ([4bd9a76](https://www.github.com/gikari/test-bismuth-ci/commit/4bd9a76c78956c7a99cd6b43e0cb32f6ab65fa08))
* :sparkles: add project icon ([eceeaa7](https://www.github.com/gikari/test-bismuth-ci/commit/eceeaa796cf7575f5a71b98c300c005e6ca910f9))
* :wrench: ner master area window count shortcuts ([3b2152e](https://www.github.com/gikari/test-bismuth-ci/commit/3b2152e81199cbf156f44efe4e333778d597e4eb))
* add prettier pre-commit hook ([8a439bb](https://www.github.com/gikari/test-bismuth-ci/commit/8a439bb41b73ff5afffb67aa75624b965fb00c1b))
* add reuse tool precommit hook ([4713d45](https://www.github.com/gikari/test-bismuth-ci/commit/4713d458afa4c3ab74e9c228d9d0618a64845016))
* compile as module ([f09d2c5](https://www.github.com/gikari/test-bismuth-ci/commit/f09d2c550a0b0f79dec7bead44f77e8536842e44))
* increase version ([82d3eca](https://www.github.com/gikari/test-bismuth-ci/commit/82d3eca2ec70c9eb7acbcf310169969d62596e29))
* install typescript via npm ([96cb46e](https://www.github.com/gikari/test-bismuth-ci/commit/96cb46ef00fb94f919efcf403b0ebf3a235ce30d))
* prevent npm pushing ([393d1bb](https://www.github.com/gikari/test-bismuth-ci/commit/393d1bbf1a87085fc571a6e7e44dde9750ac0cde))
* remove node modules in clean ([7567dbe](https://www.github.com/gikari/test-bismuth-ci/commit/7567dbeda31ae5d632c43266000135ef31a4eaf1))
* rename ocurencies of krohnkite to bismuth ([07de0aa](https://www.github.com/gikari/test-bismuth-ci/commit/07de0aa5a443b4ed5946cb62143c94629f71c142))
* target es7 ([88dfdd0](https://www.github.com/gikari/test-bismuth-ci/commit/88dfdd027eddc107e96e10de38255d3de8a4dca4))
* use correct name and description ([9ee821d](https://www.github.com/gikari/test-bismuth-ci/commit/9ee821dab3dce37460fd97e30502c1fb9e515469))
* use esbuild for compiling script ([5845551](https://www.github.com/gikari/test-bismuth-ci/commit/584555191bd287dde6d2ef216c30c3d816c6a22e))
* use eslint instead of tslint ([08d8dce](https://www.github.com/gikari/test-bismuth-ci/commit/08d8dce1e2a55cee217705012d230bf7dc566ec1))
* **wayland:** :fire: remove mouse poller ([8ca1838](https://www.github.com/gikari/test-bismuth-ci/commit/8ca1838f684d2d51d962d106e853bc87b54e4963))
* **wayland:** :fire: remove qmlSetTimer ([3277a21](https://www.github.com/gikari/test-bismuth-ci/commit/3277a21888f6a660190124aab7041e19f7bd72d4))


### Bug Fixes

* :ambulance: restore configuration dialog ([2be1673](https://www.github.com/gikari/test-bismuth-ci/commit/2be1673c41eafef2666a6265335b39159f916903))
* :bug: Correctly init global configs ([3b87e93](https://www.github.com/gikari/test-bismuth-ci/commit/3b87e9388387726b97e09a00b92a79e34f84db92))
* :bug: Monocle Layout "minimize unfocused windows" fixes and improvements ([5e26214](https://www.github.com/gikari/test-bismuth-ci/commit/5e262141a114e3d7163355e03d163c372bd050aa))
* :bug: Pass QML objects to various facilities ([24d5573](https://www.github.com/gikari/test-bismuth-ci/commit/24d557314958eb8b915e1ee0667434bd097e5b6b))
* :bug: use correct key for floating layout ([ca2a53b](https://www.github.com/gikari/test-bismuth-ci/commit/ca2a53b6664fec1254366d8db65522d3a8fc4cb0))
* :bug: use correct quarter layout id ([d196853](https://www.github.com/gikari/test-bismuth-ci/commit/d196853941ed068678cd8df1cab03b220ac71ded))
* :fire: Pass config object instead of global ([33ae26a](https://www.github.com/gikari/test-bismuth-ci/commit/33ae26a35b4aa53efda07c98566d76723f5b6d8e))
* :memo: add simple installation instructions ([6f14c55](https://www.github.com/gikari/test-bismuth-ci/commit/6f14c55708d322abd71b57c7517335bdda58e640))
* :memo: provide more feedback after installation ([cf59968](https://www.github.com/gikari/test-bismuth-ci/commit/cf59968dcaf3cf2df92541897824886b9d0fd4d5))
* :memo: Use npm commands instead of make in docs ([5c2d21e](https://www.github.com/gikari/test-bismuth-ci/commit/5c2d21eb931273c59fcc8eb3d87045b4a96697ac))
* :sparkles: Corretly pass all global objects ([54e3966](https://www.github.com/gikari/test-bismuth-ci/commit/54e39666a3844916d9a9072d623b6ee9c37896a8))
* **action:** :bug: correctly prefix layout shortcuts ([b90a5d4](https://www.github.com/gikari/test-bismuth-ci/commit/b90a5d49b7bedc566f2c86d2606844a6c9008e23))
* **action:** :bug: notify about rotation non-appliance ([78c220e](https://www.github.com/gikari/test-bismuth-ci/commit/78c220e496d217577a7a896aff7c2f3cafac4b8c))
* add extentions so import statements in code ([e45d3a9](https://www.github.com/gikari/test-bismuth-ci/commit/e45d3a908ac6e9176fa11c7ef1108acdb1deedf0))
* **build:** add tsc type checking before bundling ([b185f37](https://www.github.com/gikari/test-bismuth-ci/commit/b185f375f8602a5b68bdc06498856947c7cabb7c))
* check plugin info after installation ([3f65866](https://www.github.com/gikari/test-bismuth-ci/commit/3f65866b9dd55e5a4034654b16280d4e4fbf83c3))
* config crash ([4fd8615](https://www.github.com/gikari/test-bismuth-ci/commit/4fd8615b7dec361cfb6bdd308ab3150d61d09159))
* correct preinstall hook ([d95521c](https://www.github.com/gikari/test-bismuth-ci/commit/d95521c5afea2ec4d08bee77b1b2ddb1de01f0d6))
* do not debug line number ([cecb6cc](https://www.github.com/gikari/test-bismuth-ci/commit/cecb6cc6912300e2090469e3b43ce8487584d3cc))
* **driver:** remove enter import ([3a98b8c](https://www.github.com/gikari/test-bismuth-ci/commit/3a98b8cf637df1c47fa3e1f13228371818eb32cf))
* **driver:** rename local screens var to fix ES6 compilation ([41b70a8](https://www.github.com/gikari/test-bismuth-ci/commit/41b70a8fde3d81de52fe65aa6749fd6b19595792))
* **engine_window:** rename local vars to fix ES6 compilation ([911fa8f](https://www.github.com/gikari/test-bismuth-ci/commit/911fa8f6249fdf8cd5e55e8d244c366eb59820ac))
* install from correct path ([06f0e7e](https://www.github.com/gikari/test-bismuth-ci/commit/06f0e7edd3af82518a728646083dfe1f697e1884))
* **KWinDriver:** clients iteration for ES6 ([f5e04a8](https://www.github.com/gikari/test-bismuth-ci/commit/f5e04a82947bc1cfa2c5ec266069fbe31b06e6f5))
* publish artifacts on release ([638c876](https://www.github.com/gikari/test-bismuth-ci/commit/638c8766ae2e46b94242eb6aff62c37bb0ce2fd2))
* put package into build directory ([826b1e1](https://www.github.com/gikari/test-bismuth-ci/commit/826b1e1c52d37bbbfd9a6af57a00c73b58a3c181))
* rollback to es5 ([efdbb64](https://www.github.com/gikari/test-bismuth-ci/commit/efdbb64d297f858462987d09a4064e1a90dcbbbd))
* **wayland:** :bug: react to the new client immidiately ([f5a1068](https://www.github.com/gikari/test-bismuth-ci/commit/f5a1068389485ae84bf58cb323b63c4ed8898d12))
* **wayland:** :fire: remove basicUnit and its usages ([062352e](https://www.github.com/gikari/test-bismuth-ci/commit/062352e1ae04b88758900eb7f701f0f7a6218e44))


### Code Refactoring

* forward mouse poller ([eb51e0c](https://www.github.com/gikari/test-bismuth-ci/commit/eb51e0cce01b85d206a944c400d48513bcb1aa60))

### [1.0.1](https://www.github.com/gikari/bismuth/compare/v1.0.0...v1.0.1) (2021-10-02)


### Bug Fixes

* :ambulance: restore configuration dialog ([2be1673](https://www.github.com/gikari/bismuth/commit/2be1673c41eafef2666a6265335b39159f916903))
* :memo: provide more feedback after installation ([cf59968](https://www.github.com/gikari/bismuth/commit/cf59968dcaf3cf2df92541897824886b9d0fd4d5))

## [1.0.0](https://www.github.com/gikari/bismuth/compare/v1.0.0-beta...v1.0.0) (2021-10-02)

Initial release.
