# rollup changelog

## 0.35.11

* Deconflict reified namespaces with other declarations ([#910](https://github.com/rollup/rollup/issues/910))

## 0.35.10

* Only remove EmptyStatement nodes directly inside blocks ([#913](https://github.com/rollup/rollup/issues/931))

## 0.35.9

* Support Node 0.12 ([#909](https://github.com/rollup/rollup/issues/909))

## 0.35.8

* Correctly deshadow re-assigned module functions ([#910](https://github.com/rollup/rollup/issues/910))

## 0.35.7

* Refactor `flushTime.js` ([#922](https://github.com/rollup/rollup/pull/922))

## 0.35.6

* Fix browser build

## 0.35.5

* Allow empty for loop heads ([#919](https://github.com/rollup/rollup/issues/919))

## 0.35.4

* Preserve effects in for-of and for-in loops ([#870](https://github.com/rollup/rollup/issues/870))
* Remove empty statements ([#918](https://github.com/rollup/rollup/pull/918))

## 0.35.3

* Render identifiers inside template literals

## 0.35.2

* Fix broken build caused by out of date locally installed dependencies

## 0.35.1

* Rewrite deconflicted class identifiers ([#915](https://github.com/rollup/rollup/pull/915))
* Include `dependencies` in `bundle.modules` objects ([#903](https://github.com/rollup/rollup/issues/903))
* Update to Acorn 4 ([#914](https://github.com/rollup/rollup/pull/914))

## 0.35.0

* Rewrite analysis/tree-shaking code ([#902](https://github.com/rollup/rollup/pull/902))
* Include conditional mutations of global objects ([#901](https://github.com/rollup/rollup/issues/901))
* Only reify namespaces if necessary ([#898](https://github.com/rollup/rollup/issues/898))
* Track mutations of aliased globals ([#893](https://github.com/rollup/rollup/issues/893))
* Include duplicated var declarations ([#716](https://github.com/rollup/rollup/issues/716))

## 0.34.13

* Pass `{ format }` through to `transformBundle` ([#867](https://github.com/rollup/rollup/issues/867))

## 0.34.12

* Fix `rollup --watch` ([#887](https://github.com/rollup/rollup/issues/887))
* Case-sensitive paths ([#862](https://github.com/rollup/rollup/issues/862))

## 0.34.11

* Prevent leaky state when `bundle` is reused ([#875](https://github.com/rollup/rollup/issues/875))
* Ensure `intro` appears before interop block ([#880](https://github.com/rollup/rollup/issues/880))

## 0.34.10

* Allow custom `options.context` to replace top-level `this` ([#851](https://github.com/rollup/rollup/issues/851))
* Fix `noConflict` when used via `rollup --config` ([#846](https://github.com/rollup/rollup/issues/846))
* Place `outro` block *after* export block ([#852](https://github.com/rollup/rollup/issues/852))

## 0.34.9

* Disable indentation by default, for faster bundle generation ([#812](https://github.com/rollup/rollup/pull/812))
* More helpful error on missing entry file ([#802](https://github.com/rollup/rollup/issues/802))
* Preserve comments before import declarations ([#815](https://github.com/rollup/rollup/pull/815))

## 0.34.8

* Wrap UMD factory function in parens to avoid lazy parsing ([#774](https://github.com/rollup/rollup/pull/774))

## 0.34.7

* Leave it up to resolveId to normalize the entry path ([#835](https://github.com/rollup/rollup/pull/835))
* Cache decoded mappings ([#834](https://github.com/rollup/rollup/pull/834))

## 0.34.5

* Fix circular export ([#813](https://github.com/rollup/rollup/issues/813))

## 0.34.4

* Module render performance tweak ([#823](https://github.com/rollup/rollup/pull/823))

## 0.34.3

* Avoid infinite recursion in `Bundle.sort()` ([#800](https://github.com/rollup/rollup/pull/800))

## 0.34.2

* resolveId calls are cached now to improve incremental build
* Fixed error message recursion in plugins

## 0.34.1

* Support `paths` config ([#754](https://github.com/rollup/rollup/issues/754))
* Allow `export *` from external module, internally

## 0.34.0

* Use resolved IDs for relative imports that are also external modules, to allow `options.globals` to work with them ([#763](https://github.com/rollup/rollup/issues/763))
* Ensure reassigned exports are declared in an ES bundle, and remove empty `exports.foo;` statements ([#755](https://github.com/rollup/rollup/issues/755))
* Add newline after sourcemap comment ([#756](https://github.com/rollup/rollup/issues/756))

## 0.33.2

* Add `bundle` as second argument to `ongenerate` and `onwrite` hooks ([#773](https://github.com/rollup/rollup/pull/773))
* Warn on top-level `this` ([#770](https://github.com/rollup/rollup/issues/770))

## 0.33.1

* Fix `--no-strict` option ([#751](https://github.com/rollup/rollup/pull/751))
* Fix Windows edge case with case-sensitive paths ([#760](https://github.com/rollup/rollup/pull/760))

## 0.33.0

* Downgrade missing transformer sourcemap to a warning, not an error, and print the name of the offending plugin if possible ([#746](https://github.com/rollup/rollup/issues/746))
* Warn if same name is re-exported from two modules ([#722](https://github.com/rollup/rollup/issues/722))

## 0.32.4

* Add `ongenerate` and `onwrite` plugin hooks ([#742](https://github.com/rollup/rollup/pull/742))

## 0.32.3

* Generated correct sourcemaps with reified namespaces ([#668](https://github.com/rollup/rollup/issues/668))
* Exclude plugin helper modules from sourcemaps ([#747](https://github.com/rollup/rollup/pull/747))

## 0.32.2

* Allow `--globals` to work with `--external` or `options.external` in whatever configuration ([#743](https://github.com/rollup/rollup/issues/743))

## 0.32.1

* Preserve side-effects to default exports that coincide with used named exports ([#733](https://github.com/rollup/rollup/issues/733))
* Support `rollup -c node:pkgname` ([#736](https://github.com/rollup/rollup/issues/736))

## 0.32.0

* Deprecate `es6` format in favour of `es` ([#468](https://github.com/rollup/rollup/issues/468))
* Add correct `jsnext:main` build ([#726](https://github.com/rollup/rollup/pull/726))

## 0.31.2

* Allow `load` plugins to provide sourcemap ([#715](https://github.com/rollup/rollup/pull/715))
* Allow `sourceMapFile` in config options ([#717](https://github.com/rollup/rollup/issues/717))

## 0.31.1

* Logging for errors emitted by `rollup-watch` ([#712](https://github.com/rollup/rollup/issues/712))

## 0.31.0

* Rewrite top-level `this` as `undefined` ([#707](https://github.com/rollup/rollup/pull/707))
* Pass `options.acorn` to Acorn ([#564](https://github.com/rollup/rollup/issues/564))

## 0.30.0

* Bundle CLI ([#700](https://github.com/rollup/rollup/issues/700))
* Ensure absolute paths are normalised ([#704](https://github.com/rollup/rollup/issues/704))
* Allow `rollup --watch` to work with targets

## 0.29.1

* Merge `target` options with main options ([#701](https://github.com/rollup/rollup/issues/701))
* Update magic-string ([#690](https://github.com/rollup/rollup/issues/690))

## 0.29.0

* `rollup --watch` ([#284](https://github.com/rollup/rollup/issues/284))

## 0.28.0

* Experimental support for incremental rebuilds ([#658](https://github.com/rollup/rollup/pull/658))

## 0.27.1

* Ensure names exported from a module are not replaced with reserved words ([#696](https://github.com/rollup/rollup/pull/696))
* Revert ([#692](https://github.com/rollup/rollup/pull/692)) – resolved IDs must be strings

## 0.27.0

* Use native promises instead of `es6-promise` ([#689](https://github.com/rollup/rollup/issues/689))
* Support multiple targets in config files ([#655](https://github.com/rollup/rollup/issues/655))
* Allow `resolveId` plugin functions to return non-strings ([#692](https://github.com/rollup/rollup/pull/692))

## 0.26.7

* Distinguish between default and namespace imports of external module ([#637](https://github.com/rollup/rollup/issues/637))
* Add `__esModule` property to named exports in AMD, CJS and UMD modes ([#650](https://github.com/rollup/rollup/issues/650))

## 0.26.6

* Deconflict named imports from external modules in ES bundles ([#659](https://github.com/rollup/rollup/issues/659))
* Support `options.preferConst` to generate `const` declarations for exports rather than `var` declarations ([#653](https://github.com/rollup/rollup/issues/653))

## 0.26.5

* Preserve `debugger` statements ([#664](https://github.com/rollup/rollup/issues/664))
* Allow `options.external` to be a function ([#522](https://github.com/rollup/rollup/issues/522))

## 0.26.4

* Prevent plugin-provided external IDs being normalised ([#630](https://github.com/rollup/rollup/issues/630), [#633](https://github.com/rollup/rollup/issues/633))
* Throw if module exports/re-exports the same name twice, or has multiple default exports ([#679](https://github.com/rollup/rollup/issues/679))
* Warn about `eval` security issue ([#675]((https://github.com/rollup/rollup/issues/675)))


## 0.26.3

* Ensure reference is not incorrectly marked as a reassignment ([#648](https://github.com/rollup/rollup/issues/648))

## 0.26.2

* Sanity check output of `load` hook ([#607](https://github.com/rollup/rollup/issues/607))
* Correct scoping for ID class expressions ([#626](https://github.com/rollup/rollup/issues/626))
* Warn if named and default exports are used together in auto mode ([#587](https://github.com/rollup/rollup/issues/587))
* Allow variable initialisers to be rewritten if necessary ([#632](https://github.com/rollup/rollup/issues/632))
* Prevent double `var` with no-treeshake option ([#639](https://github.com/rollup/rollup/pull/639))

## 0.26.1

* Add `treeshake: false`/`--no-treeshake` option for debugging ([#505](https://github.com/rollup/rollup/issues/505))
* Update build process to use Bublé ([#620](https://github.com/rollup/rollup/pull/620))

## 0.26.0

* Add `noConflict`/`--no-conflict` option for UMD builds ([#580](https://github.com/rollup/rollup/pull/580))
* Normalise relative external paths ([#591](https://github.com/rollup/rollup/pull/591))
* Report files causing transform errors ([#609](https://github.com/rollup/rollup/pull/609))
* Handle sourcemap segments with a single member ([#619](https://github.com/rollup/rollup/pull/619))
* Update dependencies

## 0.25.8

* Unixize entry path ([#586](https://github.com/rollup/rollup/pull/586))

## 0.25.7

* Expand deshadowed shorthand properties ([#575](https://github.com/rollup/rollup/issues/575))
* Allow external files to be non-existent ([#532](https://github.com/rollup/rollup/issues/532))

## 0.25.6

* Fix a regression introduced by #566 ([#569](https://github.com/rollup/rollup/issues/569))
* Prune dead conditional expressions more carefully ([#567](https://github.com/rollup/rollup/issues/567))

## 0.25.5

* Make sure shorthand destructuring assignments don't break ([#528](https://github.com/rollup/rollup/issues/528))
* Allow 'exports' key ([#542](https://github.com/rollup/rollup/issues/542))
* Ensure `foo.  bar` where `foo` is a namespace import is rewritten correctly ([#566](https://github.com/rollup/rollup/issues/566))
* Fix an edge case for exported globals (e.g. `export { document }`) ([#562](https://github.com/rollup/rollup/issues/562))

## 0.25.4

* Fix misnamed exports of default imports in ES bundles ([#513](https://github.com/rollup/rollup/issues/513))
* CLI: warn on missing config ([#515](https://github.com/rollup/rollup/pull/515))
* Detect side-effects in non-top-level member expression assignment ([#476](https://github.com/rollup/rollup/issues/476))
* Don't remove computed property class keys ([#504](https://github.com/rollup/rollup/issues/504))
* Augment existing global object rather than replacing ([#493](https://github.com/rollup/rollup/issues/493))
* Don't fail on `export {}`, warn instead ([#486](https://github.com/rollup/rollup/issues/486))

## 0.25.3

* Handle non-objects and `null` in `_interopDefault` ([#474](https://github.com/rollup/rollup/issues/474))

## 0.25.2

* Skip dead branches of a conditional expression (#[465](https://github.com/rollup/rollup/pull/465))
* Allow globals to be exported ([#472](https://github.com/rollup/rollup/pull/472))
* Ensure reassigned exports are exported ([#484](https://github.com/rollup/rollup/issues/484))

## 0.25.1

* Throw error if namespace is called ([#446](https://github.com/rollup/rollup/issues/446))
* Prevent shadowing bug in ES6 output ([#441](https://github.com/rollup/rollup/pull/441))
* Prevent `var exports.foo` ([#426](https://github.com/rollup/rollup/issues/426))
* Prevent double export of aliased symbols ([#438](https://github.com/rollup/rollup/issues/438))
* Provide more informative error if Rollup is used in-browser without appropriate `resolveId`/`load` hooks ([#275](https://github.com/rollup/rollup/issues/275))
* Use `_interopDefault` function to DRY out code with many external dependencies, in CommonJS output ([#458](https://github.com/rollup/rollup/pull/458))

## 0.25.0

* **breaking** Module order is determined according to spec, rather than in a way designed to prevent runtime errors. Rollup will warn if it detects runtime errors are likely ([#435](https://github.com/rollup/rollup/issues/435))
* Prevent overly aggressive tree-shaking with complex call expressions ([#440](https://github.com/rollup/rollup/issues/440))

## 0.24.1

* Handle calls to default exports other that are not function expressions or references to function declarations ([#421](https://github.com/rollup/rollup/issues/421))
* Ensure namespace blocks are created for chained imports ([#430](https://github.com/rollup/rollup/issues/430))
* Include references in computed property keys ([#434](https://github.com/rollup/rollup/issues/434))
* Use CLI `--external` option correctly ([#417](https://github.com/rollup/rollup/pull/417))
* Allow relative imports to be treated as external, if absolute paths are provided in `options.external` ([#410](https://github.com/rollup/rollup/issues/410))
* Make IIFE output adhere to Crockford style ([#415](https://github.com/rollup/rollup/pull/415))

## 0.24.0

* No longer attempts to resolve IDs in `options.external` ([#407](https://github.com/rollup/rollup/issues/407))
* Fix broken sourcemap resolution in cases where some modules are transformed and others aren't ([#404](https://github.com/rollup/rollup/issues/404))

## 0.23.2

* Ensure `dest` or `sourceMapFile` is resolved against CWD for purposes of sourcemap generation ([#344](https://github.com/rollup/rollup/issues/344))
* Support `banner`, `footer`, `intro` and `outro` options via CLI ([#330](https://github.com/rollup/rollup/issues/330))
* Allow `options.global` to be a function rather than an object, and warn on missing names ([#293](https://github.com/rollup/rollup/issues/293))
* Ensure side-effects are captured in cyclical call expressions ([#397](https://github.com/rollup/rollup/issues/397))
* Fix parse error with body-less arrow function expressions ([#403](https://github.com/rollup/rollup/issues/403))

## 0.23.1

* Reinstate missing fix from ([#392](https://github.com/rollup/rollup/pull/392))

## 0.23.0

* Add `bundleTransform` plugin hook and option ([#387](https://github.com/rollup/rollup/pull/387))
* Correctly store names in sourcemaps, regardless of transformers
* Add `--environment` option to CLI ([#388](https://github.com/rollup/rollup/pull/388))
* Handle destructuring in exports ([#374](https://github.com/rollup/rollup/issues/374))
* Fix UMD global exports bug introduced in 0.22.1 ([#392](https://github.com/rollup/rollup/pull/392))

## 0.22.2

* Prevent lost `var` keywords ([#390](https://github.com/rollup/rollup/issues/390))

## 0.22.1

* Update expected option keys ([#379](https://github.com/rollup/rollup/issues/379))
* Handle transformers that return stringified sourcemaps ([#377](https://github.com/rollup/rollup/issues/377))
* Automatically create missing namespaces if `moduleName` contains dots ([#378](https://github.com/rollup/rollup/issues/378))
* Ignore external dependency warnings coming from config file ([#333](https://github.com/rollup/rollup/issues/333))
* Update to latest magic-string for performance boost

## 0.22.0

* Duplicate warnings are squelched ([#362](https://github.com/rollup/rollup/issues/362))
* Plugins can manipulate or override the `options` object ([#371](https://github.com/rollup/rollup/pull/371))

## 0.21.3

* Validate option keys ([#348](https://github.com/rollup/rollup/pull/348))
* Allow namespaces imports to sit alongside named imports ([#355](https://github.com/rollup/rollup/issues/355))
* Count references inside destructured objects ([#364](https://github.com/rollup/rollup/issues/364))
* Preserve top-level `delete` statements ([#352](https://github.com/rollup/rollup/issues/352))

## 0.21.2

* Missing relative imports are an error, not a warning ([#321](https://github.com/rollup/rollup/issues/321))
* Fixed incorrectly renamed default exports in ES6 bundles ([#339](https://github.com/rollup/rollup/issues/339))
* Fixed infinite recursion bug ([#341](https://github.com/rollup/rollup/issues/341))

## 0.21.1

* Remove `aggressive: true` (was too aggressive) ([#309](https://github.com/rollup/rollup/pull/309))
* Handle top-level block statements ([#326](https://github.com/rollup/rollup/issues/326))
* Optimise namespaces with default exports ([#314](https://github.com/rollup/rollup/issues/314))

## 0.21.0

* Only include statements whose side-effects are relevant (i.e. contribute to exports or affect global state) ([#253](https://github.com/rollup/rollup/pull/253)) ([#253](https://github.com/rollup/rollup/pull/253))
* Exclude dead branches from analysis and inclusion ([#249](https://github.com/rollup/rollup/pull/249))
* Add `aggressive: true` option to eliminate all side-effects outside entry module
* More informative error when re-exporting non-existent binding ([#274](https://github.com/rollup/rollup/issues/274))
* Fix infinite recursion bug ([#291](https://github.com/rollup/rollup/issues/291))
* Log errors when using `rollup --config` ([#288](https://github.com/rollup/rollup/pull/288))
* Return rejected promises on startup instead of throwing error, if options are invalid ([#303](https://github.com/rollup/rollup/pull/303))

## 0.20.5

* Ensure re-exports don't create a local binding ([#270](https://github.com/rollup/rollup/pull/270))

## 0.20.4

* Check file exists at resolve time, to allow filenames with non-extension dots in them ([#250](https://github.com/rollup/rollup/pull/250))
* Import `Promise` where used, for Node 0.10 support ([#254](https://github.com/rollup/rollup/issues/254))
* Allow asynchronous transformer plugins ([#260](https://github.com/rollup/rollup/issues/260))
* Don't assume re-exported bindings are globals when deconflicting ([#267](https://github.com/rollup/rollup/issues/267))


## 0.20.3

* Fix bug where multiple `export *` declarations caused error ([#244](https://github.com/rollup/rollup/pulls/244))
* Missing namespace exports are a warning, not an error ([#244](https://github.com/rollup/rollup/pulls/244))
* Plugins can provide `banner` and `footer` options (string, or function that returns a string) ([#235](https://github.com/rollup/rollup/issues/235))
* Warn on encountering `eval` ([#186](https://github.com/rollup/rollup/issues/186))

## 0.20.2

* Handle errors in build config file
* More robust deconflicting, in cases where e.g. `foo$1` already exists
* Use Rollup CLI for own build process

## 0.20.1

* Support `--config` file to enable plugins with CLI ([#226](https://github.com/rollup/rollup/pulls/226))
* Prevent `default` being used as variable name ([#215](https://github.com/rollup/rollup/issues/215))
* Update deps

## 0.20.0

* Support for [plugins](https://github.com/rollup/rollup/wiki/Plugins) ([#207](https://github.com/rollup/rollup/pulls/207))
* BREAKING – `options.transform`, `options.load`, `options.resolveId`, `options.resolveExternal` and `options.external` are no longer supported, and should be handled by plugins. [More info](https://github.com/rollup/rollup/wiki/Plugins)
* BREAKING – the .js extension is only added if it looks like there's no extension, allowing e.g. `import data from 'data.json'` (with the appropriate transformer). For safety, always include the file extension – import `./foo.js`, not `./foo`

## 0.19.2

* Fix exporting namespaces to include all of their exports ([#204](https://github.com/rollup/rollup/issues/204))
* Namespace exotic objects are frozen to ensure that its properties cannot be modified, reconfigured, redefined or deleted ([#203](https://github.com/rollup/rollup/pulls/203))
* Fix `ReferenceError: Promise is not defined` in node v0.10 ([#189](https://github.com/rollup/rollup/issues/189))

## 0.19.1

* Fix `module.basename()` when used with custom `resolveId` function
* Use [rollup-babel](https://github.com/rollup/rollup-babel) to build self
* Exposed the version string through the API: `require( 'rollup' ).VERSION`

## 0.19.0

* **breaking** The `transform` option is no longer passed through to custom loaders. Loaders should only concern themselves with providing source code; transformation will *always* take place
* `options.transform` functions can return a string, or a `{code, map, ast}` object. Where possible, sourcemap chains will be flattened ([#175](https://github.com/rollup/rollup/pull/175))
* `options.resolveId`, `options.resolveExternal` and `options.load` can each be a function or an array of functions. If an array, the first non-null/undefined return value is used. In both cases, failed resolution/loading will fall back to the defaults, unless an error is thrown. ([#174](https://github.com/rollup/rollup/pull/174))
* New `intro` and `outro` options – similar to `banner` and `footer` except inserted *inside* any format-specific wrapper
* Multiple var declarations in an export block (e.g. `export let a = 1, b = 2`) are split up to facilitate tree-shaking ([#171](https://github.com/rollup/rollup/issues/171))
* More informative error when using a missing namespace property  ([#169](https://github.com/rollup/rollup/pull/169))
* Update various dependencies

## 0.18.5

* Allow namespaces to be assigned to variables ([#168](https://github.com/rollup/rollup/issues/168))
* Promote `chalk` and `source-map-support` to `dependencies`, as they're used by the CLI ([#167](https://github.com/rollup/rollup/pull/167))

## 0.18.4

* Make external modules configurable (i.e. `external.config.foo = 'bar'`) without erroring

## 0.18.3

* Crop indent exclusion ranges to exclude enclosing quotes ([#166](https://github.com/rollup/rollup/issues/166))

## 0.18.2

* Include definitions of namespace members that are exported as defaults

## 0.18.1

* Include `acorn.parse` in bundle, remove `sander` from dependencies, simplify build

## 0.18.0

* Internal rewrite
* Reinstate statically-analysable namespace imports
* Avoid using getters in namespace blocks where possible ([#144](https://github.com/rollup/rollup/issues/144))
* Track variable aliases ([#96](https://github.com/rollup/rollup/issues/96))
* Prevent multiline strings being indented ([#164](https://github.com/rollup/rollup/issues/164))

## 0.17.4

* Allow imports from hidden directories (replay of [#133](https://github.com/rollup/rollup/issues/133))

## 0.17.3

* Handle parenthesised default exports ([#136](https://github.com/rollup/rollup/issues/136))

## 0.17.2

* Allow use of scoped npm packages ([#131](https://github.com/rollup/rollup/issues/131))

## 0.17.1

* Allow namespaces to be passed to a function ([#149](https://github.com/rollup/rollup/issues/149))

## 0.17.0

* Roll back to 0.15.0 and reapply subsequent fixes pending resolution of ([#132](https://github.com/rollup/rollup/issues/132)) and related issues

## 0.16.4

* Fix import paths with `.` ([#133](https://github.com/rollup/rollup/issues/133))
* Prevent sourceMappingURL confusion leading to broken sourcemap
* Add code coverage reporting [#130](https://github.com/rollup/rollup/pull/130))
* Add `modules` property to user-facing `bundle` – an array with `{id}` objects ([#128](https://github.com/rollup/rollup/issues/128))

## 0.16.3

* Prevent adjacent blocks of multiple var declarations causing magic-string failure ([#105](https://github.com/rollup/rollup/issues/105))

## 0.16.2

* Top-level function calls and assignments to globals are treated as side-effects, and always included
* Import files from subdirectories of external packages, e.g. `import mod from 'foo/sub/mod'` ([#126](https://github.com/rollup/rollup/issues/126))

## 0.16.1

* Handle assignment patterns, and destructured/rest parameters, when analysing scopes
* Fix bug preventing project from self-building (make base `Identifier` class markable)

## 0.16.0

* Internal refactoring ([#99](https://github.com/rollup/rollup/pull/99))
* Optimisation for statically-analysable namespace imports ([#99](https://github.com/rollup/rollup/pull/99))
* Windows support (theoretically!) ([#117](https://github.com/rollup/rollup/pull/117) / [#119](https://github.com/rollup/rollup/pull/119))

## 0.15.0

* Load all modules specified by `import` statements, and do tree-shaking synchronously once loading is complete. This results in simpler and faster code, and enables future improvements ([#97](https://github.com/rollup/rollup/pull/97))
* Only rewrite `foo` as `exports.foo` when it makes sense to ([#92](https://github.com/rollup/rollup/issues/92))
* Fix bug with shadowed variables that are eventually exported ([#91](https://github.com/rollup/rollup/issues/91))
* Exclude unused function declarations that happen to modify a used name ([#90](https://github.com/rollup/rollup/pull/90))
* Simplify internal `Scope` model – scopes always attach to blocks, never function expressions/declarations

## 0.14.1

* `export { name } from './other'` does not create a local binding ([#16](https://github.com/rollup/rollup/issues/16))
* A single binding can be exported under multiple names ([#18](https://github.com/rollup/rollup/issues/18))
* `useStrict` option exposed to CLI as `--strict`/`--no-strict` ([#81](https://github.com/rollup/rollup/issues/81))
* Neater exports from ES6 bundles

## 0.14.0

* Internal refactoring
* Correctly deconflict generated default export names ([#72](https://github.com/rollup/rollup/issues/72))
* Handle `export { x } from 'y'` declarations ([#74](https://github.com/rollup/rollup/issues/74))
* Dedupe named imports from external modules in ES6 bundles ([#77](https://github.com/rollup/rollup/issues/77))

## 0.13.0

* Support `banner` and `footer` options ([#66](https://github.com/rollup/rollup/pull/66))
* Remove pre-existing sourcemap comments ([#66](https://github.com/rollup/rollup/pull/66))
* Deconflict external imports ([#66](https://github.com/rollup/rollup/pull/66))
* Use existing AST, if provided ([#66](https://github.com/rollup/rollup/pull/66))
* Rename internal namespace exports as appropriate ([#66](https://github.com/rollup/rollup/pull/66))
* Remove uninitialised var declarations that get exported ([#66](https://github.com/rollup/rollup/pull/66))
* Rename variables named `exports` to avoid conflicts ([#66](https://github.com/rollup/rollup/pull/66))

## 0.12.1

* Don't attempt to mark statements belonging to external modules ([#68](https://github.com/rollup/rollup/issues/68))
* Correctly deshadow variables that conflict with imports ([#68](https://github.com/rollup/rollup/issues/68))

## 0.12.0

* Internal re-architecting, resulting in more efficient bundling with reduced memory usage
* Shorthand properties are expanded if necessary ([#61](https://github.com/rollup/rollup/issues/61))
* Fixed various bugs with bundle external dependencies, particularly when generating ES6 bundles ([#59](https://github.com/rollup/rollup/issues/59))
* Add `--globals` option to CLI ([#60](https://github.com/rollup/rollup/pull/60))
* Allow imports of external modules for side-effects ([#55](https://github.com/rollup/rollup/pull/55))
* Prevent Rollup hanging on non-existent external module ([#54](https://github.com/rollup/rollup/pull/54))

## 0.11.4

* Side-effect preservation applies to internal default exports ([#43](https://github.com/rollup/rollup/issues/43))

## 0.11.3

* Class methods are not incorrectly renamed ([#42](https://github.com/rollup/rollup/issues/42))
* External modules are assigned names before canonical names are determined ([#42](https://github.com/rollup/rollup/issues/42))

## 0.11.2

* Correctly handle computed properties (e.g. `foo[bar]`) when discovering dependencies ([#47](https://github.com/rollup/rollup/pull/47))

## 0.11.1

* Support for `export * from '..'` ([#46](https://github.com/rollup/rollup/pull/46))

## 0.11.0

* Experimental browser-friendly build (`dist/rollup.browser.js`) ([#25](https://github.com/rollup/rollup/issues/25))
* Internal re-architecting to make discovery process simpler and more performant
* Preservation of side-effects that happen in a separate module to the affected definition ([#39](https://github.com/rollup/rollup/issues/39))

## 0.10.0

* Better sorting algorithm – sorting happens at the module level, rather than the statement level. This avoids certain edge cases
* IIFEs are ignored for the purposes of distinguishing between 'strong' and 'weak' dependencies
* Empty `var` declarations for exported bindings are omitted

## 0.9.1

* Much faster statement insertion (fixes major 0.9.0 performance regression)

## 0.9.0

* BREAKING - `resolvePath` is now `resolveId`. The returned `id` (which by default is a filepath) is passed to the `load` function, which can optionally be overridden, and which is applied to all modules including the entry module. This allows custom resolver and loading logic for integration with third party systems (e.g. JSPM) or, eventually, in-browser usage ([#30](https://github.com/rollup/rollup/issues/30))
* A statement cannot appear after later statements from the same bundle ([#34](https://github.com/rollup/rollup/issues/34))
* Tricky cyclical dependencies are handled ([#36](https://github.com/rollup/rollup/issues/36))
* `sourcemap` option is used by CLI (was omitted previously)

## 0.8.3

* Correctly rename functions that have arguments with the same name ([#32](https://github.com/rollup/rollup/issues/32))
* Ensure unused default exports are given a legal name ([#33](https://github.com/rollup/rollup/issues/33))

## 0.8.2

* Support `moduleId` and `moduleName` via CLI ([#24](https://github.com/rollup/rollup/issues/24))

## 0.8.1

* Anonymous functions that are exported as default are converted to named function declarations for correct hoisting, rather than being bound to functions ([#29](https://github.com/rollup/rollup/issues/29))
* Automatically-generated default export names are deconflicted with local definitions ([#29](https://github.com/rollup/rollup/issues/29))

## 0.8.0

* Top-level variable declarations with multiple declarators are split up, to avoid unnecessary code importing and incorrectly-ordered statements ([#26](https://github.com/rollup/rollup/issues/26))
* `this` at the top level is `undefined` ([#28](https://github.com/rollup/rollup/issues/28))

## 0.7.8

* Avoid using `path.parse` - unsupported in node 0.10

## 0.7.7

* Promise `source-map-support` from `devDependencies` to `dependencies` ([#23](https://github.com/rollup/rollup/issues/23))

## 0.7.6

* Better placement of `export default` statements ([#21](https://github.com/rollup/rollup/issues/21))
* Prevent function calls and property assignments from being treated as rebinding for sake of unbound default exports
* Add `--external foo,bar,baz` option to CLI (equivalent to `external: ['foo', 'bar', 'baz']`)
* Add CLI tests

## 0.7.5

* Prevent accidental conflicts with the global namespace ([#20](https://github.com/rollup/rollup/issues/20))

## 0.7.4

* More precise statement re-ordering to satisfy `export default` constraint (fixes bug introduced in 0.7.3)

## 0.7.3

* Default exports are not bound. To enable this, statements within a module are sorted to retain their original order ([#15](https://github.com/rollup/rollup/issues/15))
* Better positioning of comments ([#14](https://github.com/rollup/rollup/issues/14))
* Various fixes to get Travis-CI rigged up

## 0.7.2

* Fix sourcemap paths on Windows ([#6](https://github.com/rollup/rollup/pull/6))

## 0.7.1

* Named functions can be used as default exports from a bundle
* Method calls are assumed to mutate the owner (i.e. `foo.bar()` mutates `foo`) ([#13](https://github.com/rollup/rollup/issues/13))
* `options.indent` can be used to control indentation of resulting bundle. `options.true` (default) means 'auto', `options.false` means empty string. Alternatively specify whitespace e.g. `'  '` or `'\t'` ([#5](https://github.com/rollup/rollup/issues/5))

## 0.7.0

* Ensure statements are always separated by a newline ([#9](https://github.com/rollup/rollup/pull/9))
* Use CommonJS `exports` correctly (UMD exports)
* Throw error if `moduleName` is required but missing (UMD exports)
* Attach IIFE global to `this` rather than `window`
* Allow names inside bundle to the the names of `Object.prototype` properties ([#12](https://github.com/rollup/rollup/pull/12))
* Keep exports live ([#11](https://github.com/rollup/rollup/pull/11))

## 0.6.5

* Add sourceMappingURL comment to code, as appropriate
* Higher resolution sourcemaps

## 0.6.4

* Fix CJS bundling with default export

## 0.6.3

* Fix exports and external module imports with some output formats
* Fix endless cycle bug on Windows ([#3](https://github.com/rollup/rollup/pull/3)) - thanks @Bobris

## 0.6.2

* Permit assignments to properties of imported bindings

## 0.6.1

* Support for basic transformers

## 0.6.0

* BREAKING - `rollup.rollup` and `bundle.write` both take a single options argument
* BREAKING - external modules must be declared upfront with `options.external: [...]`
* Non-relative module paths will be resolved by looking for `jsnext:main` fields in the appropriate `package.json` files. This behaviour can be overridden by passing an alternative `resolveExternal` function
* Fix sourcemap options
* Include CLI files in npm package (duh)

## 0.5.0

* Command line interface
* Sourcemap generation
* Correct behaviour with `export { x as y } from 'z'`

## 0.4.1

* More import name deconflicting

## 0.4.0

* Self-hosting! `rollup.rollup` now rolls up rollup
* Fix bug with comments inside a statement later being appended to it
* Prevent shadowing of external modules
* Rewrite computed property identifiers where necessary
* Preserve original statement order where possible
* Internal refactoring

## 0.3.1

* Saner deconflicting
* Rename namespace imports from external modules correctly

## 0.3.0

* Basic functionality present, mostly spec-compliant

## 0.2.1

* Include dist files in npm package (duh)

## 0.2.0

* First release capable of doing anything useful
* Still lots of basic functionality missing

## 0.1.0

* Initial experiment
