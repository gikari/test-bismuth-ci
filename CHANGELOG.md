<!--
  SPDX-FileCopyrightText: none
  SPDX-License-Identifier: MIT
-->

# Changelog

## [2.0.0](https://www.github.com/gikari/test-bismuth-ci/compare/v1.0.2...v2.0.0) (2021-11-05)


### ⚠ BREAKING CHANGES

* remove old config button from KWin scripts page
* These options should be always enabled by default, because this is how all tiling window managers work: mouse resize always has feedback and resizing always affects the layout.
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
* :lipstick: make the popup more consistent with the Plasma OSDs ([8d6a374](https://www.github.com/gikari/test-bismuth-ci/commit/8d6a3747e640c4bd418e361b342f1cb0745a3ff0))
* :memo: add issues' templates ([e59b3b2](https://www.github.com/gikari/test-bismuth-ci/commit/e59b3b2965dc9f07c19fd6d7b0d10dac906cc3d0))
* :sparkles: add basic husky hook ([3e7f3d3](https://www.github.com/gikari/test-bismuth-ci/commit/3e7f3d39b5ef4d992100472579fab4adc42c1602))
* :sparkles: add jest as unit testing framework ([caa1d25](https://www.github.com/gikari/test-bismuth-ci/commit/caa1d258582f97ecf66775d3390bc656a3a3fb25))
* :sparkles: add Krohnkite shortcuts import script ([4bd9a76](https://www.github.com/gikari/test-bismuth-ci/commit/4bd9a76c78956c7a99cd6b43e0cb32f6ab65fa08))
* :sparkles: add project icon ([eceeaa7](https://www.github.com/gikari/test-bismuth-ci/commit/eceeaa796cf7575f5a71b98c300c005e6ca910f9))
* :wrench: ner master area window count shortcuts ([3b2152e](https://www.github.com/gikari/test-bismuth-ci/commit/3b2152e81199cbf156f44efe4e333778d597e4eb))
* add KCM for Bismuth configuration ([1c410cf](https://www.github.com/gikari/test-bismuth-ci/commit/1c410cf1c759d707596a42214489dbe36bd52278))
* add prettier pre-commit hook ([8a439bb](https://www.github.com/gikari/test-bismuth-ci/commit/8a439bb41b73ff5afffb67aa75624b965fb00c1b))
* add reuse tool precommit hook ([4713d45](https://www.github.com/gikari/test-bismuth-ci/commit/4713d458afa4c3ab74e9c228d9d0618a64845016))
* compile as module ([f09d2c5](https://www.github.com/gikari/test-bismuth-ci/commit/f09d2c550a0b0f79dec7bead44f77e8536842e44))
* increase version ([82d3eca](https://www.github.com/gikari/test-bismuth-ci/commit/82d3eca2ec70c9eb7acbcf310169969d62596e29))
* install typescript via npm ([96cb46e](https://www.github.com/gikari/test-bismuth-ci/commit/96cb46ef00fb94f919efcf403b0ebf3a235ce30d))
* introduce tray item, that lets you toggle floating mode ([ba689c5](https://www.github.com/gikari/test-bismuth-ci/commit/ba689c5ff099c3263384395cfaa737a14e158b90))
* make layouts togglable ([8ebffbe](https://www.github.com/gikari/test-bismuth-ci/commit/8ebffbe639efcf1cfec5addad29e2777d1bbd5d2))
* prevent npm pushing ([393d1bb](https://www.github.com/gikari/test-bismuth-ci/commit/393d1bbf1a87085fc571a6e7e44dde9750ac0cde))
* reload script after applying configuraton ([e73cbce](https://www.github.com/gikari/test-bismuth-ci/commit/e73cbce4c8af5ab308634972409b4f7f87e95085))
* remove adjustLayout options ([1cdf1a5](https://www.github.com/gikari/test-bismuth-ci/commit/1cdf1a5bb22d7d323d0a242253f4e88216d251dc))
* remove node modules in clean ([7567dbe](https://www.github.com/gikari/test-bismuth-ci/commit/7567dbeda31ae5d632c43266000135ef31a4eaf1))
* rename ocurencies of krohnkite to bismuth ([07de0aa](https://www.github.com/gikari/test-bismuth-ci/commit/07de0aa5a443b4ed5946cb62143c94629f71c142))
* target es7 ([88dfdd0](https://www.github.com/gikari/test-bismuth-ci/commit/88dfdd027eddc107e96e10de38255d3de8a4dca4))
* use better layout notifications ([8c013ac](https://www.github.com/gikari/test-bismuth-ci/commit/8c013ac7bc8d293c81c1f14f03c2147d47d43703))
* use correct name and description ([9ee821d](https://www.github.com/gikari/test-bismuth-ci/commit/9ee821dab3dce37460fd97e30502c1fb9e515469))
* use esbuild for compiling script ([5845551](https://www.github.com/gikari/test-bismuth-ci/commit/584555191bd287dde6d2ef216c30c3d816c6a22e))
* use eslint instead of tslint ([08d8dce](https://www.github.com/gikari/test-bismuth-ci/commit/08d8dce1e2a55cee217705012d230bf7dc566ec1))
* **wayland:** :fire: remove mouse poller ([8ca1838](https://www.github.com/gikari/test-bismuth-ci/commit/8ca1838f684d2d51d962d106e853bc87b54e4963))
* **wayland:** :fire: remove qmlSetTimer ([3277a21](https://www.github.com/gikari/test-bismuth-ci/commit/3277a21888f6a660190124aab7041e19f7bd72d4))


### Bug Fixes

* :ambulance: add executable flag to installation script ([360588a](https://www.github.com/gikari/test-bismuth-ci/commit/360588ad216d364a81d518e020e5fe37b6365ccc))
* :ambulance: restore configuration dialog ([2be1673](https://www.github.com/gikari/test-bismuth-ci/commit/2be1673c41eafef2666a6265335b39159f916903))
* :bug: add Conky to default ignore list ([d989261](https://www.github.com/gikari/test-bismuth-ci/commit/d989261d82ed75781b59322402beb6c3916d09ce))
* :bug: correctly import Tile Layout Krohnkite shortcut ([04f11f9](https://www.github.com/gikari/test-bismuth-ci/commit/04f11f98c31ce63adb6c09a06da95377b01defba))
* :bug: Correctly init global configs ([3b87e93](https://www.github.com/gikari/test-bismuth-ci/commit/3b87e9388387726b97e09a00b92a79e34f84db92))
* :bug: do not tile utility windows on wayland ([935a338](https://www.github.com/gikari/test-bismuth-ci/commit/935a33820b20ab4c4b68dd797b62a64947cb9e0c))
* :bug: Monocle Layout "minimize unfocused windows" fixes and improvements ([5e26214](https://www.github.com/gikari/test-bismuth-ci/commit/5e262141a114e3d7163355e03d163c372bd050aa))
* :bug: Pass QML objects to various facilities ([24d5573](https://www.github.com/gikari/test-bismuth-ci/commit/24d557314958eb8b915e1ee0667434bd097e5b6b))
* :bug: prevent KWin freeze in various scenarious ([34d24a4](https://www.github.com/gikari/test-bismuth-ci/commit/34d24a4cb6494ea5bf29305462a1243ab143dc0c))
* :bug: put shaded windows to float state to avoid layout breakage ([aa05369](https://www.github.com/gikari/test-bismuth-ci/commit/aa053694aac927184ee17fdbe39b9f8a550b129c))
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
* correctly destroy callbacks after script unload ([aad9860](https://www.github.com/gikari/test-bismuth-ci/commit/aad986096273bc9d66ef7098c1c32b725a120902))
* do not debug line number ([cecb6cc](https://www.github.com/gikari/test-bismuth-ci/commit/cecb6cc6912300e2090469e3b43ce8487584d3cc))
* do not ignore second windows when resize ([165008b](https://www.github.com/gikari/test-bismuth-ci/commit/165008b9ac755bf312096ea45ac2ef303fb42e3a))
* **driver:** remove enter import ([3a98b8c](https://www.github.com/gikari/test-bismuth-ci/commit/3a98b8cf637df1c47fa3e1f13228371818eb32cf))
* **driver:** rename local screens var to fix ES6 compilation ([41b70a8](https://www.github.com/gikari/test-bismuth-ci/commit/41b70a8fde3d81de52fe65aa6749fd6b19595792))
* **engine_window:** rename local vars to fix ES6 compilation ([911fa8f](https://www.github.com/gikari/test-bismuth-ci/commit/911fa8f6249fdf8cd5e55e8d244c366eb59820ac))
* ignore ksmserver (logoug screen) ([caf7d08](https://www.github.com/gikari/test-bismuth-ci/commit/caf7d080d94776defbb4e2dfe9cf0e5ff7f00a31))
* improve popup geometry update ([1f02e47](https://www.github.com/gikari/test-bismuth-ci/commit/1f02e47a37fa0771f10e31e6e7f2e5d2cb9419db))
* install from correct path ([06f0e7e](https://www.github.com/gikari/test-bismuth-ci/commit/06f0e7edd3af82518a728646083dfe1f697e1884))
* **KWinDriver:** clients iteration for ES6 ([f5e04a8](https://www.github.com/gikari/test-bismuth-ci/commit/f5e04a82947bc1cfa2c5ec266069fbe31b06e6f5))
* no crashes in closing transients -- might fix others too; ref [#110](https://www.github.com/gikari/test-bismuth-ci/issues/110), [#109](https://www.github.com/gikari/test-bismuth-ci/issues/109) ([502f812](https://www.github.com/gikari/test-bismuth-ci/commit/502f8120815ce4a6b1d40ac1e79e046b0fc59624))
* **popup:** fix errors in popup.qml ([2862e56](https://www.github.com/gikari/test-bismuth-ci/commit/2862e56194fc37308224caf5fe826c76a59e088c))
* prevent crash with Monocle and monocleMinimizeRest when closing transient dialogs; ref [#110](https://www.github.com/gikari/test-bismuth-ci/issues/110) ([49ac131](https://www.github.com/gikari/test-bismuth-ci/commit/49ac131044f5202069f2202dea5ca0cd16a5257b))
* put package into build directory ([826b1e1](https://www.github.com/gikari/test-bismuth-ci/commit/826b1e1c52d37bbbfd9a6af57a00c73b58a3c181))
* remove old config button from KWin scripts page ([ff33753](https://www.github.com/gikari/test-bismuth-ci/commit/ff3375314b8cf3863d39875cb8751469a71977d6))
* rollback to es5 ([efdbb64](https://www.github.com/gikari/test-bismuth-ci/commit/efdbb64d297f858462987d09a4064e1a90dcbbbd))
* **wayland:** :bug: react to the new client immidiately ([f5a1068](https://www.github.com/gikari/test-bismuth-ci/commit/f5a1068389485ae84bf58cb323b63c4ed8898d12))
* **wayland:** :fire: remove basicUnit and its usages ([062352e](https://www.github.com/gikari/test-bismuth-ci/commit/062352e1ae04b88758900eb7f701f0f7a6218e44))


### Code Refactoring

* forward mouse poller ([eb51e0c](https://www.github.com/gikari/test-bismuth-ci/commit/eb51e0cce01b85d206a944c400d48513bcb1aa60))

## [2.0.0](https://www.github.com/Bismuth-Forge/bismuth/compare/v1.1.0...v2.0.0) (2021-11-03)


### ⚠ BREAKING CHANGES

* remove old config button from KWin scripts page. This is no longer needed, as the user should use KCM.
* removed adjust layout options. These options should be always enabled by default, because this is how all tiling window managers work: mouse resize always has feedback and resizing always affects the layout.

### Features

* add KCM for Bismuth configuration ([1c410cf](https://www.github.com/Bismuth-Forge/bismuth/commit/1c410cf1c759d707596a42214489dbe36bd52278))
* introduce tray item, that lets you toggle floating mode ([ba689c5](https://www.github.com/Bismuth-Forge/bismuth/commit/ba689c5ff099c3263384395cfaa737a14e158b90))
* make layouts togglable ([8ebffbe](https://www.github.com/Bismuth-Forge/bismuth/commit/8ebffbe639efcf1cfec5addad29e2777d1bbd5d2))
* reload script after applying configuraton ([e73cbce](https://www.github.com/Bismuth-Forge/bismuth/commit/e73cbce4c8af5ab308634972409b4f7f87e95085))

### Bug Fixes

* correctly destroy callbacks after script unload ([aad9860](https://www.github.com/Bismuth-Forge/bismuth/commit/aad986096273bc9d66ef7098c1c32b725a120902))

## [1.1.0](https://www.github.com/gikari/bismuth/compare/v1.0.2...v1.1.0) (2021-10-23)


### Features

* :lipstick: make the popup more consistent with the Plasma OSDs ([8d6a374](https://www.github.com/gikari/bismuth/commit/8d6a3747e640c4bd418e361b342f1cb0745a3ff0))
* use better layout notifications ([8c013ac](https://www.github.com/gikari/bismuth/commit/8c013ac7bc8d293c81c1f14f03c2147d47d43703))


### Bug Fixes

* :ambulance: add executable flag to installation script ([360588a](https://www.github.com/gikari/bismuth/commit/360588ad216d364a81d518e020e5fe37b6365ccc))
* improve popup geometry update ([1f02e47](https://www.github.com/gikari/bismuth/commit/1f02e47a37fa0771f10e31e6e7f2e5d2cb9419db))
* **popup:** fix errors in popup.qml ([2862e56](https://www.github.com/gikari/bismuth/commit/2862e56194fc37308224caf5fe826c76a59e088c))

### [1.0.2](https://www.github.com/gikari/bismuth/compare/v1.0.1...v1.0.2) (2021-10-22)


### Bug Fixes

* :bug: add Conky to default ignore list ([d989261](https://www.github.com/gikari/bismuth/commit/d989261d82ed75781b59322402beb6c3916d09ce))
* :bug: correctly import Tile Layout Krohnkite shortcut ([04f11f9](https://www.github.com/gikari/bismuth/commit/04f11f98c31ce63adb6c09a06da95377b01defba))
* :bug: do not tile utility windows on wayland ([935a338](https://www.github.com/gikari/bismuth/commit/935a33820b20ab4c4b68dd797b62a64947cb9e0c))
* :bug: prevent KWin freeze in various scenarious ([34d24a4](https://www.github.com/gikari/bismuth/commit/34d24a4cb6494ea5bf29305462a1243ab143dc0c))
* :bug: put shaded windows to float state to avoid layout breakage ([aa05369](https://www.github.com/gikari/bismuth/commit/aa053694aac927184ee17fdbe39b9f8a550b129c))
* ignore ksmserver (logoug screen) ([caf7d08](https://www.github.com/gikari/bismuth/commit/caf7d080d94776defbb4e2dfe9cf0e5ff7f00a31))
* no crashes in closing transients -- might fix others too; ref [#110](https://www.github.com/gikari/bismuth/issues/110), [#109](https://www.github.com/gikari/bismuth/issues/109) ([502f812](https://www.github.com/gikari/bismuth/commit/502f8120815ce4a6b1d40ac1e79e046b0fc59624))
* prevent crash with Monocle and monocleMinimizeRest when closing transient dialogs; ref [#110](https://www.github.com/gikari/bismuth/issues/110) ([49ac131](https://www.github.com/gikari/bismuth/commit/49ac131044f5202069f2202dea5ca0cd16a5257b))

### [1.0.1](https://www.github.com/gikari/bismuth/compare/v1.0.0...v1.0.1) (2021-10-02)


### Bug Fixes

* :ambulance: restore configuration dialog ([2be1673](https://www.github.com/gikari/bismuth/commit/2be1673c41eafef2666a6265335b39159f916903))
* :memo: provide more feedback after installation ([cf59968](https://www.github.com/gikari/bismuth/commit/cf59968dcaf3cf2df92541897824886b9d0fd4d5))

## [1.0.0](https://www.github.com/gikari/bismuth/compare/v1.0.0-beta...v1.0.0) (2021-10-02)

Initial release.
