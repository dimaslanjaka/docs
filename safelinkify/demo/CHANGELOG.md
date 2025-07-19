## CHANGELOG of safelinkify


### 1.2.1

- [ _2023-09-07 12:44:48_ ] [a4878d7](<https://github.com/dimaslanjaka/safelink/commit/a4878d7>) add changelog v1.2.1
- [ _2023-10-17 18:30:11_ ] [d47e4a9](<https://github.com/dimaslanjaka/safelink/commit/d47e4a9>) chore: update dependencies
- [ _2023-10-17 18:33:46_ ] [65912cf](<https://github.com/dimaslanjaka/safelink/commit/65912cf>) try add exports property
- [ _2023-10-17 18:35:21_ ] [0e6c920](<https://github.com/dimaslanjaka/safelink/commit/0e6c920>) install husky and lint-staged
- [ _2023-10-17 18:39:14_ ] [e63f256](<https://github.com/dimaslanjaka/safelink/commit/e63f256>) chore: url starts with `?` and `#` should be internal/not anonymize
- [ _2023-10-17 18:40:07_ ] [54ea68e](<https://github.com/dimaslanjaka/safelink/commit/54ea68e>)
    
    remove `@types/prettier`
    prettier v3 has internal definition files
- [ _2023-10-17 18:41:05_ ] [977f69f](<https://github.com/dimaslanjaka/safelink/commit/977f69f>) remove unused files in monorepo
- [ _2023-10-17 18:44:52_ ] [07990b6](<https://github.com/dimaslanjaka/safelink/commit/07990b6>) url starts with `?` and `#` should be internal
- [ _2023-10-17 18:45:24_ ] [ba73a6a](<https://github.com/dimaslanjaka/safelink/commit/ba73a6a>) ignore lint dist files
- [ _2025-02-07 12:18:59_ ] [15470c5](<https://github.com/dimaslanjaka/safelink/commit/15470c5>) docs: change sample link to blame
- [ _2025-07-19 11:30:46_ ] [1de95da](<https://github.com/dimaslanjaka/safelink/commit/1de95da>) fix: update code actions on save settings to never organize imports and explicitly fix all
- [ _2025-07-19 11:35:11_ ] [1afad2c](<https://github.com/dimaslanjaka/safelink/commit/1afad2c>) fix: replace cross-spawn with child_process and improve package checks
- [ _2025-07-19 11:37:03_ ] [8ed6ec1](<https://github.com/dimaslanjaka/safelink/commit/8ed6ec1>) fix: update build-release workflow to improve path handling and node version configuration
- [ _2025-07-19 11:54:55_ ] [416ec72](<https://github.com/dimaslanjaka/safelink/commit/416ec72>) feat: add instructions for conventional commits and Node.js configuration
- [ _2025-07-19 12:46:18_ ] [01d0dff](<https://github.com/dimaslanjaka/safelink/commit/01d0dff>)
    
    refactor(changelog): rewrite changelog generation with version grouping
    
    - Replace static markdown with dynamic extraction of versions and commits from git log.
    - Group commits by detected version bumps.
    - Output detailed changelog with commit links and dates.
    - Write raw log to tmp/original.md for debugging.
    - Improve version extraction and sorting logic.
- [ _2025-07-19 12:57:11_ ] [a54e015](<https://github.com/dimaslanjaka/safelink/commit/a54e015>)
    
    chore(changelog): improve extraction logic
    
    - Exclude "update build from http(s)://" commits from changelog.
    - Prevent duplicate commit messages in version sections by overwriting previous entries with the latest hash and date.
- [ _2025-07-19 12:59:58_ ] [e65b788](<https://github.com/dimaslanjaka/safelink/commit/e65b788>)
    
    fix(changelog): detect version bumps for plain semantic version strings
    
    - Added support to treat commits like `1.2.3` as version bumps in changelog generation
- [ _2025-07-19 13:17:04_ ] [5372def](<https://github.com/dimaslanjaka/safelink/commit/5372def>)
    
    feat(changelog): improve commit parsing with author info and better filtering
    
    - Include author and committer names in git log extraction
    - Filter out commits from dependabot[bot] and specific non-changelog patterns
    - Improve detection of version bumps with stricter version format
    - Enhance duplication detection by matching cleaned message lines
    - Render multiline commit messages correctly in changelog
- [ _2025-07-19 13:18:57_ ] [a00193a](<https://github.com/dimaslanjaka/safelink/commit/a00193a>) feat: add binary-collections dependency
- [ _2025-07-19 13:20:21_ ] [4cd2414](<https://github.com/dimaslanjaka/safelink/commit/4cd2414>) chore: remove auto generated CHANGELOG.md file
- [ _2025-07-19 13:22:03_ ] [d87c48b](<https://github.com/dimaslanjaka/safelink/commit/d87c48b>) chore(package): update scripts for prepack and prepublish hooks
- [ _2025-07-19 13:24:58_ ] [c9f86a2](<https://github.com/dimaslanjaka/safelink/commit/c9f86a2>) feat: add resolutions for binary-collections, markdown-it, and sbg-utility dependencies
- [ _2025-07-19 13:26:00_ ] [8db48de](<https://github.com/dimaslanjaka/safelink/commit/8db48de>) refactor: ignore dist files
- [ _2025-07-19 13:28:10_ ] [359b90a](<https://github.com/dimaslanjaka/safelink/commit/359b90a>) fix: ensure proper initialization of MarkdownIt with commonmark option
- [ _2025-07-19 13:33:42_ ] [6128fa6](<https://github.com/dimaslanjaka/safelink/commit/6128fa6>) fix: handle optional constructor parameter and improve redirect option handling
- [ _2025-07-19 13:33:52_ ] [3d5d78b](<https://github.com/dimaslanjaka/safelink/commit/3d5d78b>) feat: add import test for safelinkify and demonstrate encodeURL functionality
- [ _2025-07-19 13:50:58_ ] [14c127d](<https://github.com/dimaslanjaka/safelink/commit/14c127d>) feat(test): mjs import
- [ _2025-07-19 13:53:54_ ] [dbde81e](<https://github.com/dimaslanjaka/safelink/commit/dbde81e>)
    
    refactor(eslint): migrate to flat config and update dependencies
    
    - Removed legacy `.eslintrc.js` and `.eslintignore` files
    - Introduced `eslint.config.mjs` using FlatConfig with ESLint v9
    - Updated `.vscode/settings.json` to enable flat config support
    - Updated ESLint and related dependencies to latest versions
    - Aligned Prettier and TypeScript settings with new ESLint config
    - Enhanced ignore patterns and plugin rules for consistency
- [ _2025-07-19 14:03:15_ ] [8c28067](<https://github.com/dimaslanjaka/safelink/commit/8c28067>) feat(test): initialize jest
- [ _2025-07-19 14:06:12_ ] [10baaa6](<https://github.com/dimaslanjaka/safelink/commit/10baaa6>)
    
    test(extractDomain): add unit tests and improve robustness
    
    - Added `extractDomain.test.ts` with multiple test cases for different URL formats
    - Enhanced `extractDomain` to handle:
      - Non-string input
      - Empty or malformed URLs
      - Edge cases like missing hostname
    - Ensured `undefined` is returned when domain extraction fails
- [ _2025-07-19 14:10:26_ ] [47f5f17](<https://github.com/dimaslanjaka/safelink/commit/47f5f17>)
    
    test(string): add unit tests and fix type for string.ts
    
    - Added unit tests for:
      - bufferToString
      - capitalizer (with custom separators)
      - escapeRegex (method 1 and 2)
      - streamToString using a Readable stream
    - Updated type definition of streamToString to accept NodeJS.ReadableStream
- [ _2025-07-19 14:12:59_ ] [755bb0d](<https://github.com/dimaslanjaka/safelink/commit/755bb0d>)
    
    fix(parseQuery): improve accuracy and add unit tests
    
    - Ensure hash query parameters override search params
    - Safely check for existence of key using `hasOwnProperty`
    - Return undefined for missing keys instead of falling back to entire object
    - Added comprehensive unit tests covering:
      - Empty and invalid URLs
      - Query string parsing
      - Hash parsing
      - Key-specific query extraction
      - Precedence of hash over search
- [ _2025-07-19 14:22:26_ ] [dcd5dda](<https://github.com/dimaslanjaka/safelink/commit/dcd5dda>)
    
    test(safelink): add unit tests and refactor direct tests
    
    - Added comprehensive unit tests for the `safelink` class covering:
      - Initialization and option merging
      - URL exclusion logic with strings and regex
      - Encoding and HTML anonymization
    - Moved direct script tests (`index.test.ts` and `safelink.test.ts`) to `test/*.direct.ts`
      - Updated imports to point to `../src` instead of local
    - Verified HTML parsing behavior preserves excluded links and anonymizes others
- [ _2025-07-19 14:25:01_ ] [c056e37](<https://github.com/dimaslanjaka/safelink/commit/c056e37>)
    
    test(toURL): add unit tests and improve fallback handling
    
    - Added unit tests for `toURL`, `isValidHttpUrl`, and `fixUrl` covering:
      - Valid and invalid URL inputs
      - Handling of URL objects
      - Normalization of slashes in URLs
    - Updated `toURL` to explicitly return null when input is not a supported URL pattern
- [ _2025-07-19 14:40:40_ ] [398b410](<https://github.com/dimaslanjaka/safelink/commit/398b410>) fix(parse): correct type import for NodeJS.ReadStream in parse method
- [ _2025-07-19 14:46:28_ ] [3a8dc3b](<https://github.com/dimaslanjaka/safelink/commit/3a8dc3b>)
    
    docs(readme): improve structure, examples, and formatting
    
    - Clarified installation instructions for both npm and yarn
    - Refined usage documentation with clear code samples for browser and Node.js
    - Added Gulp integration example with updated formatting and comments
    - Improved formatting consistency across code blocks, tables, and sections
    - Updated examples to reflect real output and enhance readability
- [ _2025-07-19 15:24:48_ ] [4ac69fd](<https://github.com/dimaslanjaka/safelink/commit/4ac69fd>)
    
    build: support modern bundlers (Vite, Webpack) via rollup build
    
    - Added rollup config to bundle safelink-browser-module for both CJS and ESM
    - Exported `browser_module` in package.json with proper types and dual module formats
    - Extended README with example usage for modern frameworks (e.g., Vite/Webpack)
    - Updated build script to include rollup
    - Added necessary dev dependencies: rollup, @rollup/plugin-* and rollup-plugin-dts
- [ _2025-07-19 15:25:41_ ] [4bc96b8](<https://github.com/dimaslanjaka/safelink/commit/4bc96b8>)
    
    chore: upgrade Yarn to version 4.9.2 and enable global cache
    
    - Updated .yarnrc.yml to enable global cache and changed Yarn path to 4.9.2.
    - Updated package.json to reflect the new Yarn version in packageManager.
### 1.1.19

- [ _2023-09-06 07:08:04_ ] [72e5d15](<https://github.com/dimaslanjaka/safelink/commit/72e5d15>) add import test
- [ _2023-09-06 07:29:47_ ] [392acce](<https://github.com/dimaslanjaka/safelink/commit/392acce>)
    
    fix: miss-configured types
    - recreate types manual from dist
- [ _2023-09-06 07:33:27_ ] [10a6704](<https://github.com/dimaslanjaka/safelink/commit/10a6704>) update packer
- [ _2023-09-06 08:49:52_ ] [1561979](<https://github.com/dimaslanjaka/safelink/commit/1561979>) split parse url to new function
- [ _2023-09-06 08:51:23_ ] [32e54a0](<https://github.com/dimaslanjaka/safelink/commit/32e54a0>) split parse url to new function
- [ _2023-09-06 08:53:36_ ] [121fdf6](<https://github.com/dimaslanjaka/safelink/commit/121fdf6>)
    
    chore(minor): v1.2.0
    - split parse url to new function
- [ _2023-09-07 00:34:22_ ] [c66d5f5](<https://github.com/dimaslanjaka/safelink/commit/c66d5f5>) update hostname type
- [ _2023-09-07 00:36:54_ ] [26c8440](<https://github.com/dimaslanjaka/safelink/commit/26c8440>) try apply global vars
- [ _2023-09-07 00:40:22_ ] [da35016](<https://github.com/dimaslanjaka/safelink/commit/da35016>) ignore dist on monorepo
- [ _2023-09-07 06:37:20_ ] [794976b](<https://github.com/dimaslanjaka/safelink/commit/794976b>) add intellij idea key binding
- [ _2023-09-07 06:47:08_ ] [f7d4b5b](<https://github.com/dimaslanjaka/safelink/commit/f7d4b5b>) import yarn config
- [ _2023-09-07 06:49:43_ ] [e678a41](<https://github.com/dimaslanjaka/safelink/commit/e678a41>) update missing definition files
- [ _2023-09-07 06:50:24_ ] [a6a6159](<https://github.com/dimaslanjaka/safelink/commit/a6a6159>) ignore lock file
- [ _2023-09-07 06:53:28_ ] [9625faa](<https://github.com/dimaslanjaka/safelink/commit/9625faa>) eslint --fix
- [ _2023-09-07 06:56:08_ ] [0d494e1](<https://github.com/dimaslanjaka/safelink/commit/0d494e1>) refactor: disable tabs
- [ _2023-09-07 06:56:31_ ] [682a0cd](<https://github.com/dimaslanjaka/safelink/commit/682a0cd>) change types and downgrade prettier@^2
- [ _2023-09-07 07:05:25_ ] [a10ed34](<https://github.com/dimaslanjaka/safelink/commit/a10ed34>) moved globals contents to index
- [ _2023-09-07 07:14:51_ ] [b6b6701](<https://github.com/dimaslanjaka/safelink/commit/b6b6701>) update custom types
- [ _2023-09-07 07:16:08_ ] [599d3f1](<https://github.com/dimaslanjaka/safelink/commit/599d3f1>) fix: NodeJS definition file imports
- [ _2023-09-07 07:19:44_ ] [98a9023](<https://github.com/dimaslanjaka/safelink/commit/98a9023>) ignore yarn version cache
### 1.1.16

- [ _2023-02-18 17:09:01_ ] [76d3341](<https://github.com/dimaslanjaka/safelink/commit/76d3341>) chore: merge from monorepo
- [ _2023-02-18 17:09:51_ ] [811fcd4](<https://github.com/dimaslanjaka/safelink/commit/811fcd4>) chore: update dependencies
- [ _2023-02-20 08:41:49_ ] [c5e2d66](<https://github.com/dimaslanjaka/safelink/commit/c5e2d66>) chore(deps):
- [ _2023-02-20 09:00:19_ ] [2366702](<https://github.com/dimaslanjaka/safelink/commit/2366702>) chore:
- [ _2023-02-20 09:01:28_ ] [569daa7](<https://github.com/dimaslanjaka/safelink/commit/569daa7>) chore:
- [ _2023-02-21 00:55:49_ ] [31b1105](<https://github.com/dimaslanjaka/safelink/commit/31b1105>) chore:
- [ _2023-02-21 09:46:41_ ] [ff635c3](<https://github.com/dimaslanjaka/safelink/commit/ff635c3>) chore: ignore tsbuildinfo files to packed
- [ _2023-02-28 03:32:19_ ] [183a662](<https://github.com/dimaslanjaka/safelink/commit/183a662>) feat: add @types/markdown-it
- [ _2023-04-14 02:03:07_ ] [4de4b56](<https://github.com/dimaslanjaka/safelink/commit/4de4b56>) chore: using wildcard version git-command-helper
- [ _2023-04-18 17:36:55_ ] [f484e25](<https://github.com/dimaslanjaka/safelink/commit/f484e25>) chore: update dependencies
- [ _2023-04-18 18:09:14_ ] [4f63e04](<https://github.com/dimaslanjaka/safelink/commit/4f63e04>) chore: bump v1.1.18
- [ _2023-04-20 14:56:38_ ] [054e546](<https://github.com/dimaslanjaka/safelink/commit/054e546>) chore: change cross-spawn source
- [ _2023-04-28 17:24:19_ ] [99d6ae7](<https://github.com/dimaslanjaka/safelink/commit/99d6ae7>) chore: update build
- [ _2023-05-07 04:22:31_ ] [7f8cc5a](<https://github.com/dimaslanjaka/safelink/commit/7f8cc5a>) chore: update dependencies
- [ _2023-05-07 09:26:31_ ] [e045886](<https://github.com/dimaslanjaka/safelink/commit/e045886>) chore: moved `persistent-cache` to dev
- [ _2023-05-08 11:14:10_ ] [32c13a2](<https://github.com/dimaslanjaka/safelink/commit/32c13a2>) refactor: re-order dependencies
- [ _2023-05-09 18:46:27_ ] [76946a5](<https://github.com/dimaslanjaka/safelink/commit/76946a5>) chore: update dependencies
- [ _2023-05-26 00:16:50_ ] [1dbeeb2](<https://github.com/dimaslanjaka/safelink/commit/1dbeeb2>) chore: update dependencies
- [ _2023-05-26 00:22:08_ ] [f20f7ab](<https://github.com/dimaslanjaka/safelink/commit/f20f7ab>) chore: update dependencies
- [ _2023-08-20 07:00:40_ ] [e8d6899](<https://github.com/dimaslanjaka/safelink/commit/e8d6899>) docs: add samples
- [ _2023-08-20 07:01:01_ ] [5e411cb](<https://github.com/dimaslanjaka/safelink/commit/5e411cb>) fix: table
- [ _2023-08-27 17:42:56_ ] [d757e86](<https://github.com/dimaslanjaka/safelink/commit/d757e86>) drop tsBuildInfoFile
- [ _2023-08-27 17:45:23_ ] [f9559f6](<https://github.com/dimaslanjaka/safelink/commit/f9559f6>) drop references
- [ _2023-08-27 17:48:52_ ] [cf8d3e2](<https://github.com/dimaslanjaka/safelink/commit/cf8d3e2>) fix partial type validation
- [ _2023-08-27 17:50:16_ ] [1405ccc](<https://github.com/dimaslanjaka/safelink/commit/1405ccc>) simplify validate
- [ _2023-08-27 17:51:17_ ] [a37ff2e](<https://github.com/dimaslanjaka/safelink/commit/a37ff2e>) make return Nullable
- [ _2023-08-27 17:51:50_ ] [15a129a](<https://github.com/dimaslanjaka/safelink/commit/15a129a>) validate property using `in` operator
- [ _2023-08-27 17:53:02_ ] [1e500b7](<https://github.com/dimaslanjaka/safelink/commit/1e500b7>) simplify validate
- [ _2023-08-27 17:54:18_ ] [432eaf1](<https://github.com/dimaslanjaka/safelink/commit/432eaf1>) force cast to dynamic object
- [ _2023-08-27 17:54:50_ ] [bd15bed](<https://github.com/dimaslanjaka/safelink/commit/bd15bed>) chore: update build
- [ _2023-08-27 17:55:45_ ] [525ab8b](<https://github.com/dimaslanjaka/safelink/commit/525ab8b>) enable declaration
- [ _2023-08-31 10:26:04_ ] [dc7626c](<https://github.com/dimaslanjaka/safelink/commit/dc7626c>) update typescript
- [ _2023-09-03 18:57:20_ ] [c616967](<https://github.com/dimaslanjaka/safelink/commit/c616967>) update dependencies
- [ _2023-09-04 05:15:38_ ] [4044979](<https://github.com/dimaslanjaka/safelink/commit/4044979>) downgrade typescript
- [ _2023-09-05 00:47:00_ ] [830d978](<https://github.com/dimaslanjaka/safelink/commit/830d978>) update linter modules
- [ _2023-09-05 01:35:39_ ] [279d84c](<https://github.com/dimaslanjaka/safelink/commit/279d84c>) ignore *.tsbuildinfo
- [ _2023-09-05 01:36:03_ ] [7820a2e](<https://github.com/dimaslanjaka/safelink/commit/7820a2e>) update build
- [ _2023-09-05 02:00:55_ ] [02dad73](<https://github.com/dimaslanjaka/safelink/commit/02dad73>)
    
    fix(TS2550): add lib es2020
    - Property 'matchAll' does not exist on type 'string'
    - Property 'fromEntries' does not exist on type 'ObjectConstructor
- [ _2023-09-05 02:01:36_ ] [04328a2](<https://github.com/dimaslanjaka/safelink/commit/04328a2>) disable typechecking, enable esmodule interop
- [ _2023-09-05 02:03:59_ ] [1cc4b13](<https://github.com/dimaslanjaka/safelink/commit/1cc4b13>) fix(window const): add lib DOM
- [ _2023-09-05 02:09:33_ ] [2148e75](<https://github.com/dimaslanjaka/safelink/commit/2148e75>) update build
- [ _2023-09-06 06:14:21_ ] [2b43d67](<https://github.com/dimaslanjaka/safelink/commit/2b43d67>) update build
- [ _2023-09-06 06:18:38_ ] [570bc07](<https://github.com/dimaslanjaka/safelink/commit/570bc07>) add declaration dir
- [ _2023-09-06 06:19:46_ ] [beef52e](<https://github.com/dimaslanjaka/safelink/commit/beef52e>) fixed build
- [ _2023-09-06 06:31:46_ ] [631dd88](<https://github.com/dimaslanjaka/safelink/commit/631dd88>) add declaration dir
### 1.1.15

- [ _2023-02-17 23:56:54_ ] [13511c1](<https://github.com/dimaslanjaka/safelink/commit/13511c1>) chore: update from monorepo
- [ _2023-02-17 23:57:33_ ] [22b11a4](<https://github.com/dimaslanjaka/safelink/commit/22b11a4>) chore: update deps
- [ _2023-02-18 17:03:12_ ] [fba0925](<https://github.com/dimaslanjaka/safelink/commit/fba0925>) docs: recommend install as dev
### 1.1.14

- [ _2023-02-10 19:39:04_ ] [c3feda1](<https://github.com/dimaslanjaka/safelink/commit/c3feda1>) fix: fix module resolutions
- [ _2023-02-12 18:20:24_ ] [4cd36c4](<https://github.com/dimaslanjaka/safelink/commit/4cd36c4>) fix: resolve module resolutions
### 1.1.13

- [ _2023-01-01 01:10:07_ ] [e82a341](<https://github.com/dimaslanjaka/safelink/commit/e82a341>) move inconsistent checksum to optional packages
- [ _2023-01-01 01:16:58_ ] [29bf15c](<https://github.com/dimaslanjaka/safelink/commit/29bf15c>) update docs
- [ _2023-01-01 01:49:45_ ] [5e86fa1](<https://github.com/dimaslanjaka/safelink/commit/5e86fa1>) update docs
- [ _2023-01-22 15:39:11_ ] [d98a27b](<https://github.com/dimaslanjaka/safelink/commit/d98a27b>) chore(deps): update dependencies
- [ _2023-01-22 16:56:57_ ] [8ec10dd](<https://github.com/dimaslanjaka/safelink/commit/8ec10dd>) chore(script): remove postinstall
- [ _2023-01-22 17:00:13_ ] [8fa5c06](<https://github.com/dimaslanjaka/safelink/commit/8fa5c06>) chore(script): rename postbuild to pack
- [ _2023-01-22 18:02:19_ ] [edaad9e](<https://github.com/dimaslanjaka/safelink/commit/edaad9e>) chore(webpack): fix dependencies
- [ _2023-01-22 18:07:08_ ] [b7da1bc](<https://github.com/dimaslanjaka/safelink/commit/b7da1bc>) feat(license): change to MIT
- [ _2023-01-22 21:33:21_ ] [1a29a89](<https://github.com/dimaslanjaka/safelink/commit/1a29a89>) chore(deps): update deps
- [ _2023-01-22 23:59:15_ ] [d1e09df](<https://github.com/dimaslanjaka/safelink/commit/d1e09df>) chore(dist): update bundle
- [ _2023-01-23 03:05:01_ ] [7803ff8](<https://github.com/dimaslanjaka/safelink/commit/7803ff8>) fix(deps): fix module resolutions
- [ _2023-01-23 03:10:32_ ] [c727224](<https://github.com/dimaslanjaka/safelink/commit/c727224>) refactor(ci): remove prebuild script
- [ _2023-01-23 03:51:54_ ] [6edeb5f](<https://github.com/dimaslanjaka/safelink/commit/6edeb5f>) fix(script): remove preupdate script
- [ _2023-01-23 04:18:09_ ] [b6df36c](<https://github.com/dimaslanjaka/safelink/commit/b6df36c>) add recommendation
- [ _2023-01-23 05:04:40_ ] [2f56bc0](<https://github.com/dimaslanjaka/safelink/commit/2f56bc0>) feat: add glob
- [ _2023-01-23 05:05:38_ ] [efbcca4](<https://github.com/dimaslanjaka/safelink/commit/efbcca4>) fix(dist): update build
- [ _2023-01-23 05:28:23_ ] [9c1987b](<https://github.com/dimaslanjaka/safelink/commit/9c1987b>) refactor(dist): fresh build with new dependencies
- [ _2023-01-23 06:33:10_ ] [a034f87](<https://github.com/dimaslanjaka/safelink/commit/a034f87>)
    
    refactor: renaming static-blog-generator branches
    
    master -> beta
    release -> master
- [ _2023-01-23 19:18:09_ ] [5e59acd](<https://github.com/dimaslanjaka/safelink/commit/5e59acd>) chore: update tarball
- [ _2023-01-24 12:21:32_ ] [fe41f6e](<https://github.com/dimaslanjaka/safelink/commit/fe41f6e>) chore(deps): update dependencies
- [ _2023-01-24 13:19:09_ ] [38a9251](<https://github.com/dimaslanjaka/safelink/commit/38a9251>) chore(deps): update submodules and dependencies
- [ _2023-01-24 16:28:29_ ] [8e967d2](<https://github.com/dimaslanjaka/safelink/commit/8e967d2>) chore(deps): update dependencies
- [ _2023-01-24 18:49:16_ ] [58a94df](<https://github.com/dimaslanjaka/safelink/commit/58a94df>) chore(dist): update dependencies
- [ _2023-01-24 18:50:45_ ] [58db45b](<https://github.com/dimaslanjaka/safelink/commit/58db45b>) feat(ci): init CI for monorepo
- [ _2023-01-24 19:11:17_ ] [acc3286](<https://github.com/dimaslanjaka/safelink/commit/acc3286>) chore(deps): installing non sbg module from registry with wildcard version
- [ _2023-01-24 23:18:15_ ] [d72dd7c](<https://github.com/dimaslanjaka/safelink/commit/d72dd7c>) chore(dist): update deps
- [ _2023-01-25 01:19:20_ ] [80db377](<https://github.com/dimaslanjaka/safelink/commit/80db377>) chore(dist): fresh pack
- [ _2023-01-25 12:23:40_ ] [e6bbd1a](<https://github.com/dimaslanjaka/safelink/commit/e6bbd1a>) chore(deps): update dependencies
- [ _2023-01-25 13:03:28_ ] [ca10029](<https://github.com/dimaslanjaka/safelink/commit/ca10029>) chore(dist): update build
- [ _2023-01-25 13:51:29_ ] [03dcf79](<https://github.com/dimaslanjaka/safelink/commit/03dcf79>) chore(ci): update build actions
- [ _2023-01-25 16:30:16_ ] [8f98307](<https://github.com/dimaslanjaka/safelink/commit/8f98307>) chore(dist): update git-command-helper API
- [ _2023-01-25 16:30:39_ ] [c2c798a](<https://github.com/dimaslanjaka/safelink/commit/c2c798a>) chore(dist): update git-command-helper API
- [ _2023-01-25 16:51:29_ ] [54ccfd6](<https://github.com/dimaslanjaka/safelink/commit/54ccfd6>) chore: update build and dependencies
- [ _2023-01-26 05:35:06_ ] [c65cea6](<https://github.com/dimaslanjaka/safelink/commit/c65cea6>) test: fixed CLI test using npx
- [ _2023-01-28 14:09:26_ ] [123e613](<https://github.com/dimaslanjaka/safelink/commit/123e613>) chore(deps): update dependencies
- [ _2023-01-28 17:34:57_ ] [a2a4899](<https://github.com/dimaslanjaka/safelink/commit/a2a4899>) refactor(hbx): init ci
- [ _2023-01-30 12:42:22_ ] [43ce14f](<https://github.com/dimaslanjaka/safelink/commit/43ce14f>) chore(deps): update dependencies
- [ _2023-01-30 18:40:02_ ] [165c1f6](<https://github.com/dimaslanjaka/safelink/commit/165c1f6>) fix(ci): re-bootstrap using lerna
- [ _2023-01-31 13:41:32_ ] [66cc59b](<https://github.com/dimaslanjaka/safelink/commit/66cc59b>) chore: update dependencies
- [ _2023-01-31 13:47:08_ ] [884819f](<https://github.com/dimaslanjaka/safelink/commit/884819f>) fix(ci): change token
- [ _2023-01-31 21:45:35_ ] [f95c8dd](<https://github.com/dimaslanjaka/safelink/commit/f95c8dd>) fix: prepare using yarn
- [ _2023-02-02 05:09:10_ ] [481fb1c](<https://github.com/dimaslanjaka/safelink/commit/481fb1c>) refactor: migrate using yarn workspace
- [ _2023-02-02 15:08:31_ ] [f7b72e4](<https://github.com/dimaslanjaka/safelink/commit/f7b72e4>) chore: try build with yarn
- [ _2023-02-02 17:33:33_ ] [efa454d](<https://github.com/dimaslanjaka/safelink/commit/efa454d>)
    
    refactor: update and pack
    
    add non-included submodules
    update dependencies
    create new tarball packs
- [ _2023-02-02 17:49:28_ ] [97193a5](<https://github.com/dimaslanjaka/safelink/commit/97193a5>) chore: change highlight.js to fixed version 11.7.0
- [ _2023-02-02 22:02:26_ ] [5188dee](<https://github.com/dimaslanjaka/safelink/commit/5188dee>) refactor: delete unused tarball
- [ _2023-02-02 22:13:23_ ] [4a860f1](<https://github.com/dimaslanjaka/safelink/commit/4a860f1>) remove unused files
- [ _2023-02-03 18:59:12_ ] [3ea47ef](<https://github.com/dimaslanjaka/safelink/commit/3ea47ef>) chore(deps): update dependencies
- [ _2023-02-03 21:32:15_ ] [264179c](<https://github.com/dimaslanjaka/safelink/commit/264179c>) chore: create fresh tarballs
- [ _2023-02-03 21:54:47_ ] [e5a3c19](<https://github.com/dimaslanjaka/safelink/commit/e5a3c19>) refactor: update packer
- [ _2023-02-04 08:10:29_ ] [df944da](<https://github.com/dimaslanjaka/safelink/commit/df944da>) refactor: remove .yarn caches
- [ _2023-02-04 14:36:17_ ] [a4c2bd8](<https://github.com/dimaslanjaka/safelink/commit/a4c2bd8>) chore: update dependencies and packer
- [ _2023-02-04 19:12:41_ ] [f096111](<https://github.com/dimaslanjaka/safelink/commit/f096111>) refactor: pack using yarn
- [ _2023-02-04 22:04:01_ ] [eb8338b](<https://github.com/dimaslanjaka/safelink/commit/eb8338b>) chore: update dependencies
- [ _2023-02-05 23:02:23_ ] [f2f39ef](<https://github.com/dimaslanjaka/safelink/commit/f2f39ef>) chore: fresh build
- [ _2023-02-06 18:53:10_ ] [438afe3](<https://github.com/dimaslanjaka/safelink/commit/438afe3>) chore: update dependencies
- [ _2023-02-07 11:10:33_ ] [584861e](<https://github.com/dimaslanjaka/safelink/commit/584861e>) chore(deps): update dependencies
- [ _2023-02-08 18:33:31_ ] [2b7c984](<https://github.com/dimaslanjaka/safelink/commit/2b7c984>) chore: fresh stable build
- [ _2023-02-10 19:11:52_ ] [df5f989](<https://github.com/dimaslanjaka/safelink/commit/df5f989>) refactor: install yarn version
### 1.1.12

- [ _2022-12-31 22:38:09_ ] [8eeda8a](<https://github.com/dimaslanjaka/safelink/commit/8eeda8a>) update deps
- [ _2022-12-31 23:08:30_ ] [ff2e631](<https://github.com/dimaslanjaka/safelink/commit/ff2e631>) update deps
### 1.1.11

- [ _2022-12-29 16:06:22_ ] [24d1142](<https://github.com/dimaslanjaka/safelink/commit/24d1142>) update task
- [ _2022-12-29 16:32:31_ ] [2fde010](<https://github.com/dimaslanjaka/safelink/commit/2fde010>) update docs
- [ _2022-12-29 16:40:29_ ] [90de175](<https://github.com/dimaslanjaka/safelink/commit/90de175>) update typedoc
- [ _2022-12-29 16:43:18_ ] [b8b3363](<https://github.com/dimaslanjaka/safelink/commit/b8b3363>) update typedocs
- [ _2022-12-29 16:45:17_ ] [c3333a8](<https://github.com/dimaslanjaka/safelink/commit/c3333a8>) rename `tests` to `src-docs`
- [ _2022-12-29 16:53:59_ ] [7920b72](<https://github.com/dimaslanjaka/safelink/commit/7920b72>) update deps
- [ _2022-12-29 16:57:21_ ] [e7c87fe](<https://github.com/dimaslanjaka/safelink/commit/e7c87fe>) update deps
- [ _2022-12-29 18:24:59_ ] [dcb3e45](<https://github.com/dimaslanjaka/safelink/commit/dcb3e45>) update deps
- [ _2022-12-31 20:25:39_ ] [4614820](<https://github.com/dimaslanjaka/safelink/commit/4614820>) Update postinstall.js
- [ _2022-12-31 21:02:21_ ] [1027a10](<https://github.com/dimaslanjaka/safelink/commit/1027a10>) Update .prettierrc.json
- [ _2022-12-31 22:31:37_ ] [055d6d7](<https://github.com/dimaslanjaka/safelink/commit/055d6d7>) prepare update 1.1.12
### 1.1.10

- [ _2022-12-26 12:58:46_ ] [5c7522e](<https://github.com/dimaslanjaka/safelink/commit/5c7522e>) update changelog
- [ _2022-12-26 13:02:29_ ] [074689d](<https://github.com/dimaslanjaka/safelink/commit/074689d>) rename `README.md` to lowercase
- [ _2022-12-26 13:13:41_ ] [c3d4870](<https://github.com/dimaslanjaka/safelink/commit/c3d4870>) Update script.js
- [ _2022-12-27 18:13:26_ ] [f6eadd8](<https://github.com/dimaslanjaka/safelink/commit/f6eadd8>) update scripts
- [ _2022-12-28 03:17:12_ ] [32d231a](<https://github.com/dimaslanjaka/safelink/commit/32d231a>) Update readme.md
- [ _2022-12-28 03:23:55_ ] [e7ef4a8](<https://github.com/dimaslanjaka/safelink/commit/e7ef4a8>) update deps
- [ _2022-12-28 03:25:15_ ] [b7b2260](<https://github.com/dimaslanjaka/safelink/commit/b7b2260>) Update readme.md
- [ _2022-12-28 03:29:52_ ] [311f600](<https://github.com/dimaslanjaka/safelink/commit/311f600>) Update readme.md
- [ _2022-12-28 03:31:19_ ] [1cd8dca](<https://github.com/dimaslanjaka/safelink/commit/1cd8dca>) Update readme.md
- [ _2022-12-28 03:33:15_ ] [9aef05f](<https://github.com/dimaslanjaka/safelink/commit/9aef05f>) Update readme.md
- [ _2022-12-28 03:33:41_ ] [fabe245](<https://github.com/dimaslanjaka/safelink/commit/fabe245>) Update readme.md
- [ _2022-12-28 03:34:49_ ] [b32220a](<https://github.com/dimaslanjaka/safelink/commit/b32220a>) Update readme.md
- [ _2022-12-28 03:35:18_ ] [103c90c](<https://github.com/dimaslanjaka/safelink/commit/103c90c>) Update readme.md
- [ _2022-12-28 03:47:23_ ] [1abb55d](<https://github.com/dimaslanjaka/safelink/commit/1abb55d>) update changelog
- [ _2022-12-28 03:49:27_ ] [1861105](<https://github.com/dimaslanjaka/safelink/commit/1861105>) update deps
- [ _2022-12-28 03:50:28_ ] [f33f6b5](<https://github.com/dimaslanjaka/safelink/commit/f33f6b5>) update deps
- [ _2022-12-28 13:29:54_ ] [b45016f](<https://github.com/dimaslanjaka/safelink/commit/b45016f>) Update readme.md
- [ _2022-12-28 13:30:38_ ] [0802620](<https://github.com/dimaslanjaka/safelink/commit/0802620>) Update readme.md
- [ _2022-12-28 13:36:54_ ] [b8061cc](<https://github.com/dimaslanjaka/safelink/commit/b8061cc>) Update readme.md
- [ _2022-12-28 13:38:17_ ] [f2a41d7](<https://github.com/dimaslanjaka/safelink/commit/f2a41d7>) Update readme.md
- [ _2022-12-29 12:27:34_ ] [c07e62c](<https://github.com/dimaslanjaka/safelink/commit/c07e62c>) add lib dom
- [ _2022-12-29 12:32:54_ ] [491a749](<https://github.com/dimaslanjaka/safelink/commit/491a749>) rename lib.dom.d.ts
- [ _2022-12-29 12:51:38_ ] [c3da040](<https://github.com/dimaslanjaka/safelink/commit/c3da040>) rename lib.dom.d.ts
- [ _2022-12-29 12:58:33_ ] [d18f2a0](<https://github.com/dimaslanjaka/safelink/commit/d18f2a0>) update docs
- [ _2022-12-29 13:12:04_ ] [c27ea0e](<https://github.com/dimaslanjaka/safelink/commit/c27ea0e>) using my global typedocs
- [ _2022-12-29 13:17:02_ ] [f5863f5](<https://github.com/dimaslanjaka/safelink/commit/f5863f5>) migrate to our global docs
- [ _2022-12-29 13:18:14_ ] [794a2bc](<https://github.com/dimaslanjaka/safelink/commit/794a2bc>) update scripts
- [ _2022-12-29 13:18:50_ ] [44e4511](<https://github.com/dimaslanjaka/safelink/commit/44e4511>) fix merge conflict
- [ _2022-12-29 13:19:35_ ] [4b07f7e](<https://github.com/dimaslanjaka/safelink/commit/4b07f7e>) fix merge conflict
- [ _2022-12-29 13:20:20_ ] [6d5a019](<https://github.com/dimaslanjaka/safelink/commit/6d5a019>) update nodemon config
- [ _2022-12-29 13:20:54_ ] [5ffe197](<https://github.com/dimaslanjaka/safelink/commit/5ffe197>) update nodemon config
- [ _2022-12-29 13:22:24_ ] [a7c9192](<https://github.com/dimaslanjaka/safelink/commit/a7c9192>) fix merge conflict
- [ _2022-12-29 13:26:33_ ] [1cdf7ae](<https://github.com/dimaslanjaka/safelink/commit/1cdf7ae>) add exclusion
- [ _2022-12-29 13:49:19_ ] [0e1783a](<https://github.com/dimaslanjaka/safelink/commit/0e1783a>) update project references
- [ _2022-12-29 13:53:29_ ] [5fb4928](<https://github.com/dimaslanjaka/safelink/commit/5fb4928>) update callback
- [ _2022-12-29 13:58:33_ ] [dd725d1](<https://github.com/dimaslanjaka/safelink/commit/dd725d1>) index.ts rename to serve.ts
- [ _2022-12-29 14:11:24_ ] [1d955d5](<https://github.com/dimaslanjaka/safelink/commit/1d955d5>) re-init eslint
- [ _2022-12-29 14:14:37_ ] [461a369](<https://github.com/dimaslanjaka/safelink/commit/461a369>) using typedoc api than cli
- [ _2022-12-29 14:17:34_ ] [5f51f56](<https://github.com/dimaslanjaka/safelink/commit/5f51f56>) fix spawn import conflict
- [ _2022-12-29 14:26:39_ ] [dab2911](<https://github.com/dimaslanjaka/safelink/commit/dab2911>) update postbuild
- [ _2022-12-29 14:54:20_ ] [d56dc9a](<https://github.com/dimaslanjaka/safelink/commit/d56dc9a>) update deps, docs builder
- [ _2022-12-29 15:00:59_ ] [5c41e15](<https://github.com/dimaslanjaka/safelink/commit/5c41e15>) fix miss-configured paths
- [ _2022-12-29 15:25:28_ ] [a6dce30](<https://github.com/dimaslanjaka/safelink/commit/a6dce30>) builder using javascript instead typescript
- [ _2022-12-29 15:38:35_ ] [e19a0fd](<https://github.com/dimaslanjaka/safelink/commit/e19a0fd>) update docs builder
- [ _2022-12-29 15:40:30_ ] [02f864c](<https://github.com/dimaslanjaka/safelink/commit/02f864c>) run changelog.js first
- [ _2022-12-29 15:45:27_ ] [1e2f289](<https://github.com/dimaslanjaka/safelink/commit/1e2f289>) update test
- [ _2022-12-29 15:45:44_ ] [c2f2739](<https://github.com/dimaslanjaka/safelink/commit/c2f2739>) update changelog
- [ _2022-12-29 15:50:13_ ] [84bee86](<https://github.com/dimaslanjaka/safelink/commit/84bee86>) update docs
- [ _2022-12-29 15:52:43_ ] [d1e2841](<https://github.com/dimaslanjaka/safelink/commit/d1e2841>) update project docs
- [ _2022-12-29 15:55:28_ ] [f21956f](<https://github.com/dimaslanjaka/safelink/commit/f21956f>) fix infinite loop
- [ _2022-12-29 15:57:41_ ] [1e51695](<https://github.com/dimaslanjaka/safelink/commit/1e51695>) update build
- [ _2022-12-29 16:00:20_ ] [2bbb5ac](<https://github.com/dimaslanjaka/safelink/commit/2bbb5ac>) update deps
### 1.1.9

- [ _2022-12-26 12:35:58_ ] [5253b1d](<https://github.com/dimaslanjaka/safelink/commit/5253b1d>) declare to global scope `safelink` and `safelinkify`
- [ _2022-12-26 12:55:41_ ] [050a356](<https://github.com/dimaslanjaka/safelink/commit/050a356>)
    
    export safelink and safelinkify to global scrope
    - update docs
- [ _2022-12-26 12:55:50_ ] [28be9cc](<https://github.com/dimaslanjaka/safelink/commit/28be9cc>)
    
    export safelink and safelinkify to global scrope
    - update docs
### 1.1.8

- [ _2022-12-21 11:48:28_ ] [7fcb525](<https://github.com/dimaslanjaka/safelink/commit/7fcb525>) add changelog builder
- [ _2022-12-21 11:53:31_ ] [62ab8f2](<https://github.com/dimaslanjaka/safelink/commit/62ab8f2>) Update changelog
- [ _2022-12-21 12:02:39_ ] [20064ec](<https://github.com/dimaslanjaka/safelink/commit/20064ec>) Update docs and changelog
- [ _2022-12-21 12:06:25_ ] [6323d22](<https://github.com/dimaslanjaka/safelink/commit/6323d22>) Update docs
- [ _2022-12-21 12:27:37_ ] [fe68ba9](<https://github.com/dimaslanjaka/safelink/commit/fe68ba9>) Update docs
- [ _2022-12-21 12:48:00_ ] [2a3ea1a](<https://github.com/dimaslanjaka/safelink/commit/2a3ea1a>) using customized package cross-spawn
- [ _2022-12-21 13:10:23_ ] [534a6e6](<https://github.com/dimaslanjaka/safelink/commit/534a6e6>) Update docs
- [ _2022-12-21 13:17:22_ ] [fd76b3b](<https://github.com/dimaslanjaka/safelink/commit/fd76b3b>) Update docs
- [ _2022-12-21 13:19:47_ ] [858ead5](<https://github.com/dimaslanjaka/safelink/commit/858ead5>) Update build
### 1.1.7

- [ _2022-12-21 10:18:48_ ] [9d5848d](<https://github.com/dimaslanjaka/safelink/commit/9d5848d>) Update docs
- [ _2022-12-21 10:23:57_ ] [13adeeb](<https://github.com/dimaslanjaka/safelink/commit/13adeeb>) move types to globals
### 1.1.6

- [ _2022-11-20 11:38:32_ ] [7bc960f](<https://github.com/dimaslanjaka/safelink/commit/7bc960f>) Update README.md
- [ _2022-11-20 11:41:15_ ] [8d3c848](<https://github.com/dimaslanjaka/safelink/commit/8d3c848>) Update README.md
- [ _2022-12-21 10:12:29_ ] [694c87c](<https://github.com/dimaslanjaka/safelink/commit/694c87c>) update deps and scripts
- [ _2022-12-21 10:13:04_ ] [377a912](<https://github.com/dimaslanjaka/safelink/commit/377a912>) move and export all types from/to globals
- [ _2022-12-21 10:14:48_ ] [9051509](<https://github.com/dimaslanjaka/safelink/commit/9051509>) Update README.md
- [ _2022-12-21 10:16:11_ ] [3faabe5](<https://github.com/dimaslanjaka/safelink/commit/3faabe5>) Update README.md
- [ _2022-12-21 10:16:56_ ] [98d00d5](<https://github.com/dimaslanjaka/safelink/commit/98d00d5>) push release too
### 1.1.5

- [ _2022-11-09 16:30:14_ ] [b5b6896](<https://github.com/dimaslanjaka/safelink/commit/b5b6896>) add OR
- [ _2022-11-09 16:31:28_ ] [ae6fca5](<https://github.com/dimaslanjaka/safelink/commit/ae6fca5>) add null validation
- [ _2022-11-09 16:32:08_ ] [6011523](<https://github.com/dimaslanjaka/safelink/commit/6011523>) Update safelink.yml
- [ _2022-11-09 16:33:27_ ] [61c0d03](<https://github.com/dimaslanjaka/safelink/commit/61c0d03>) Using npm
- [ _2022-11-09 16:37:43_ ] [ecc409f](<https://github.com/dimaslanjaka/safelink/commit/ecc409f>) add commits
- [ _2022-11-09 16:38:18_ ] [abd46eb](<https://github.com/dimaslanjaka/safelink/commit/abd46eb>) update build
- [ _2022-11-09 16:53:11_ ] [d63681d](<https://github.com/dimaslanjaka/safelink/commit/d63681d>) Update safelink.yml
- [ _2022-11-09 16:53:44_ ] [5acfae9](<https://github.com/dimaslanjaka/safelink/commit/5acfae9>) Update safelink.yml
- [ _2022-11-09 16:54:14_ ] [96ba98c](<https://github.com/dimaslanjaka/safelink/commit/96ba98c>) Update safelink.yml
- [ _2022-11-09 16:59:58_ ] [600ae45](<https://github.com/dimaslanjaka/safelink/commit/600ae45>) Update safelink.yml
- [ _2022-11-09 17:06:39_ ] [4c865fe](<https://github.com/dimaslanjaka/safelink/commit/4c865fe>) update build
### 1.1.4

- [ _2022-10-17 01:49:39_ ] [3cafc9d](<https://github.com/dimaslanjaka/safelink/commit/3cafc9d>) Update README.md
- [ _2022-10-17 01:55:33_ ] [5298e34](<https://github.com/dimaslanjaka/safelink/commit/5298e34>) Update CHANGELOG.md
- [ _2022-10-17 01:58:21_ ] [2974c3a](<https://github.com/dimaslanjaka/safelink/commit/2974c3a>) update docs
- [ _2022-10-26 09:03:33_ ] [d50f681](<https://github.com/dimaslanjaka/safelink/commit/d50f681>) update dependencies
### 1.1.3

- [ _2022-05-21 11:32:57_ ] [bcde9f0](<https://github.com/dimaslanjaka/safelink/commit/bcde9f0>) update 1.1.3 ES5
- [ _2022-05-21 11:33:54_ ] [35da245](<https://github.com/dimaslanjaka/safelink/commit/35da245>) compile to es5
- [ _2022-05-25 00:25:15_ ] [eed24bc](<https://github.com/dimaslanjaka/safelink/commit/eed24bc>) +lib
- [ _2022-05-28 15:39:28_ ] [d50c52d](<https://github.com/dimaslanjaka/safelink/commit/d50c52d>) fix module resolutions
- [ _2022-05-28 15:47:45_ ] [eacf6bb](<https://github.com/dimaslanjaka/safelink/commit/eacf6bb>) fix build
- [ _2022-05-28 17:52:09_ ] [311c604](<https://github.com/dimaslanjaka/safelink/commit/311c604>) update d.ts
- [ _2022-05-31 07:40:04_ ] [786d238](<https://github.com/dimaslanjaka/safelink/commit/786d238>) export options
- [ _2022-06-03 07:40:56_ ] [1322357](<https://github.com/dimaslanjaka/safelink/commit/1322357>) migrate to `yarn v2`
- [ _2022-06-03 08:03:10_ ] [4313451](<https://github.com/dimaslanjaka/safelink/commit/4313451>) fix `yarn v2` exclusions
- [ _2022-06-03 08:32:17_ ] [3bdbb35](<https://github.com/dimaslanjaka/safelink/commit/3bdbb35>) update module resolutions
- [ _2022-06-03 08:51:04_ ] [f9564bf](<https://github.com/dimaslanjaka/safelink/commit/f9564bf>) enable global cache
- [ _2022-06-10 16:37:52_ ] [301f8a4](<https://github.com/dimaslanjaka/safelink/commit/301f8a4>) using `npm` instead of `yarn`
- [ _2022-06-14 18:29:13_ ] [29b7fae](<https://github.com/dimaslanjaka/safelink/commit/29b7fae>) fresh build
- [ _2022-06-14 18:29:42_ ] [b3b8803](<https://github.com/dimaslanjaka/safelink/commit/b3b8803>) add test unit
- [ _2022-06-14 18:31:01_ ] [3db17d7](<https://github.com/dimaslanjaka/safelink/commit/3db17d7>) fresh install
- [ _2022-06-14 18:34:14_ ] [aa36bea](<https://github.com/dimaslanjaka/safelink/commit/aa36bea>) fresh install
- [ _2022-10-17 00:55:56_ ] [3344980](<https://github.com/dimaslanjaka/safelink/commit/3344980>) convert parse to async
- [ _2022-10-17 00:59:02_ ] [6447426](<https://github.com/dimaslanjaka/safelink/commit/6447426>) -test
- [ _2022-10-17 01:16:56_ ] [c98019c](<https://github.com/dimaslanjaka/safelink/commit/c98019c>) update dependencies
- [ _2022-10-17 01:40:24_ ] [6753a42](<https://github.com/dimaslanjaka/safelink/commit/6753a42>) fix nulled process
- [ _2022-10-17 01:43:15_ ] [1bd954d](<https://github.com/dimaslanjaka/safelink/commit/1bd954d>) add docs
- [ _2022-10-17 01:44:54_ ] [9e460f4](<https://github.com/dimaslanjaka/safelink/commit/9e460f4>) update docs
- [ _2022-10-17 01:45:16_ ] [8aa82c4](<https://github.com/dimaslanjaka/safelink/commit/8aa82c4>) update docs
### 1.1.2

- [ _2022-05-19 11:19:01_ ] [5b3eb76](<https://github.com/dimaslanjaka/safelink/commit/5b3eb76>) fix anonymizing same link on non-hyperlink
- [ _2022-05-19 11:21:52_ ] [bdfa182](<https://github.com/dimaslanjaka/safelink/commit/bdfa182>) update docs
- [ _2022-05-19 11:24:45_ ] [0a24dcd](<https://github.com/dimaslanjaka/safelink/commit/0a24dcd>) update docs
- [ _2022-05-19 11:26:16_ ] [a87c735](<https://github.com/dimaslanjaka/safelink/commit/a87c735>) update docs
- [ _2022-05-21 10:14:05_ ] [41facd5](<https://github.com/dimaslanjaka/safelink/commit/41facd5>) export interface Nullable
### 1.1.1

- [ _2022-05-19 10:31:47_ ] [de49114](<https://github.com/dimaslanjaka/safelink/commit/de49114>) update 1.1.1
- [ _2022-05-19 10:35:02_ ] [58e9c38](<https://github.com/dimaslanjaka/safelink/commit/58e9c38>) update docs
- [ _2022-05-19 10:35:35_ ] [80cd1ec](<https://github.com/dimaslanjaka/safelink/commit/80cd1ec>) update docs
- [ _2022-05-19 10:35:42_ ] [96a7465](<https://github.com/dimaslanjaka/safelink/commit/96a7465>) update docs
- [ _2022-05-19 10:48:47_ ] [73ea90c](<https://github.com/dimaslanjaka/safelink/commit/73ea90c>) update docs
- [ _2022-05-19 10:49:28_ ] [e18de77](<https://github.com/dimaslanjaka/safelink/commit/e18de77>) update docs
- [ _2022-05-19 11:17:25_ ] [2482a80](<https://github.com/dimaslanjaka/safelink/commit/2482a80>) fix anonymizing same link on non-hyperlink
- [ _2022-05-19 11:17:46_ ] [2e64dce](<https://github.com/dimaslanjaka/safelink/commit/2e64dce>) fix anonymizing same link on non-hyperlink
### 1.1.0

- [ _2022-05-19 08:59:17_ ] [2611fef](<https://github.com/dimaslanjaka/safelink/commit/2611fef>) update changelog
- [ _2022-05-19 09:03:15_ ] [8e3977b](<https://github.com/dimaslanjaka/safelink/commit/8e3977b>) fix documenter
- [ _2022-05-19 10:22:24_ ] [4b1be16](<https://github.com/dimaslanjaka/safelink/commit/4b1be16>) fix nodejs process
- [ _2022-05-19 10:26:25_ ] [546e33d](<https://github.com/dimaslanjaka/safelink/commit/546e33d>) Update README.md
- [ _2022-05-19 10:26:57_ ] [8a2fb17](<https://github.com/dimaslanjaka/safelink/commit/8a2fb17>) update docs
- [ _2022-05-19 10:28:55_ ] [b5d6362](<https://github.com/dimaslanjaka/safelink/commit/b5d6362>) fix update
- [ _2022-05-19 10:30:25_ ] [c910922](<https://github.com/dimaslanjaka/safelink/commit/c910922>) update 1.1.1
### 1.0.9

- [ _2022-05-19 08:57:37_ ] [2ec240d](<https://github.com/dimaslanjaka/safelink/commit/2ec240d>) +changelog
### 1.0.8

- [ _2022-05-19 06:42:08_ ] [b7ab961](<https://github.com/dimaslanjaka/safelink/commit/b7ab961>) update linux
- [ _2022-05-19 08:24:16_ ] [772e5dc](<https://github.com/dimaslanjaka/safelink/commit/772e5dc>) Update README.md
- [ _2022-05-19 08:40:03_ ] [db5f5ca](<https://github.com/dimaslanjaka/safelink/commit/db5f5ca>) fix for nodeJS
- [ _2022-05-19 08:40:33_ ] [46a521f](<https://github.com/dimaslanjaka/safelink/commit/46a521f>) fix
- [ _2022-05-19 08:53:37_ ] [df13456](<https://github.com/dimaslanjaka/safelink/commit/df13456>) fix nodejs process
- [ _2022-05-19 08:53:49_ ] [9a68d2b](<https://github.com/dimaslanjaka/safelink/commit/9a68d2b>) update docs
- [ _2022-05-19 08:55:51_ ] [e607c06](<https://github.com/dimaslanjaka/safelink/commit/e607c06>) update docs
- [ _2022-05-19 08:55:57_ ] [76cec9f](<https://github.com/dimaslanjaka/safelink/commit/76cec9f>) update docs
### 1.0.7

- [ _2022-04-26 01:12:56_ ] [74f2cad](<https://github.com/dimaslanjaka/safelink/commit/74f2cad>) update docs
- [ _2022-04-26 01:13:12_ ] [89431f1](<https://github.com/dimaslanjaka/safelink/commit/89431f1>) update docs
- [ _2022-04-26 01:22:18_ ] [9c850a7](<https://github.com/dimaslanjaka/safelink/commit/9c850a7>) Update README.md
- [ _2022-04-26 04:40:09_ ] [89ac38b](<https://github.com/dimaslanjaka/safelink/commit/89ac38b>) Update README.md
- [ _2022-04-26 14:30:25_ ] [458bd2c](<https://github.com/dimaslanjaka/safelink/commit/458bd2c>) [gh-pages] +toastr
- [ _2022-05-04 04:41:07_ ] [37c3fb0](<https://github.com/dimaslanjaka/safelink/commit/37c3fb0>) fix deps
- [ _2022-05-04 05:07:05_ ] [054611e](<https://github.com/dimaslanjaka/safelink/commit/054611e>) +encode single url
- [ _2022-05-04 05:10:04_ ] [01f504e](<https://github.com/dimaslanjaka/safelink/commit/01f504e>) +string type for dynamic typescript
### 1.0.6

- [ _2022-04-26 00:44:01_ ] [c962efc](<https://github.com/dimaslanjaka/safelink/commit/c962efc>) improve summoner
- [ _2022-04-26 01:02:26_ ] [294d5f9](<https://github.com/dimaslanjaka/safelink/commit/294d5f9>) [fix][1.0.7] `resolveQueryUrl`
- [ _2022-04-26 01:03:55_ ] [3653aac](<https://github.com/dimaslanjaka/safelink/commit/3653aac>) -log
- [ _2022-04-26 01:04:53_ ] [3946a35](<https://github.com/dimaslanjaka/safelink/commit/3946a35>) skip non-exist search and hashes
### 1.0.5

- [ _2022-04-24 20:31:41_ ] [5747ffa](<https://github.com/dimaslanjaka/safelink/commit/5747ffa>) prepare update 1.0.6
- [ _2022-04-24 20:34:30_ ] [0d54a08](<https://github.com/dimaslanjaka/safelink/commit/0d54a08>) update docs
### 1.0.4

- [ _2022-04-24 08:00:47_ ] [b689834](<https://github.com/dimaslanjaka/safelink/commit/b689834>) update docs
- [ _2022-04-24 08:27:16_ ] [4243ec6](<https://github.com/dimaslanjaka/safelink/commit/4243ec6>) +log summoner
- [ _2022-04-24 12:07:35_ ] [7ecd564](<https://github.com/dimaslanjaka/safelink/commit/7ecd564>) reload after summoner closed
- [ _2022-04-24 12:29:27_ ] [0e12853](<https://github.com/dimaslanjaka/safelink/commit/0e12853>) [dev] fix summoner
- [ _2022-04-24 12:42:18_ ] [be3db52](<https://github.com/dimaslanjaka/safelink/commit/be3db52>) anonymize only for url start with http/s
- [ _2022-04-24 12:45:12_ ] [1a1ccaa](<https://github.com/dimaslanjaka/safelink/commit/1a1ccaa>) [ejs] responsive improvement
- [ _2022-04-24 12:50:50_ ] [001deea](<https://github.com/dimaslanjaka/safelink/commit/001deea>) [filter] only process url with protocols
- [ _2022-04-24 12:53:00_ ] [3bdf2db](<https://github.com/dimaslanjaka/safelink/commit/3bdf2db>) [dev] fix `MaxListenersExceededWarning`
- [ _2022-04-24 12:55:36_ ] [2c9960f](<https://github.com/dimaslanjaka/safelink/commit/2c9960f>) [node] filter improvement
- [ _2022-04-24 13:02:55_ ] [0b59ef4](<https://github.com/dimaslanjaka/safelink/commit/0b59ef4>) migrate build to gulp
- [ _2022-04-24 13:15:55_ ] [a7f28a3](<https://github.com/dimaslanjaka/safelink/commit/a7f28a3>) [migrate] prefer old builder, webpack on-fly
- [ _2022-04-24 13:21:49_ ] [91a5238](<https://github.com/dimaslanjaka/safelink/commit/91a5238>) [webpack] improvement log
- [ _2022-04-24 13:27:13_ ] [7b6bb11](<https://github.com/dimaslanjaka/safelink/commit/7b6bb11>) [gulp] detach `index.ts`
- [ _2022-04-24 13:29:28_ ] [1f841c1](<https://github.com/dimaslanjaka/safelink/commit/1f841c1>) Update gulpfile.ts
- [ _2022-04-24 13:54:47_ ] [69e9ee1](<https://github.com/dimaslanjaka/safelink/commit/69e9ee1>) split webpack watcher
- [ _2022-04-24 14:20:24_ ] [0759d51](<https://github.com/dimaslanjaka/safelink/commit/0759d51>)
    
    [webpack] integrate `webpack` watcher to `browser-sync`
    [webpack] watcher improvements
- [ _2022-04-24 14:53:04_ ] [acd17c6](<https://github.com/dimaslanjaka/safelink/commit/acd17c6>) [dev] bring barck old watcher
- [ _2022-04-24 15:01:47_ ] [1383db2](<https://github.com/dimaslanjaka/safelink/commit/1383db2>) update docs
- [ _2022-04-24 15:02:25_ ] [9822e8c](<https://github.com/dimaslanjaka/safelink/commit/9822e8c>) Update README.md
- [ _2022-04-24 16:59:23_ ] [e3f1a1b](<https://github.com/dimaslanjaka/safelink/commit/e3f1a1b>) detach private script from compiler
- [ _2022-04-24 17:00:19_ ] [c6ca0e6](<https://github.com/dimaslanjaka/safelink/commit/c6ca0e6>) update compiled
- [ _2022-04-24 17:10:22_ ] [f89cf49](<https://github.com/dimaslanjaka/safelink/commit/f89cf49>) restore docs index
### 1.0.3

- [ _2022-04-23 04:04:59_ ] [ee55c98](<https://github.com/dimaslanjaka/safelink/commit/ee55c98>) update 1.0.3
- [ _2022-04-23 04:05:42_ ] [5544bd6](<https://github.com/dimaslanjaka/safelink/commit/5544bd6>) update 1.0.3
- [ _2022-04-23 05:11:07_ ] [6b18aaa](<https://github.com/dimaslanjaka/safelink/commit/6b18aaa>) prepare redirector
- [ _2022-04-23 19:34:27_ ] [53ed674](<https://github.com/dimaslanjaka/safelink/commit/53ed674>) Update README.md
- [ _2022-04-23 19:37:35_ ] [5d7f3ed](<https://github.com/dimaslanjaka/safelink/commit/5d7f3ed>) Update README.md
- [ _2022-04-23 19:41:03_ ] [b1516da](<https://github.com/dimaslanjaka/safelink/commit/b1516da>) Update README.md
- [ _2022-04-23 19:41:37_ ] [cee579e](<https://github.com/dimaslanjaka/safelink/commit/cee579e>) Update README.md
- [ _2022-04-23 20:23:25_ ] [4201016](<https://github.com/dimaslanjaka/safelink/commit/4201016>) skip CNAME
- [ _2022-04-23 20:54:47_ ] [5570edc](<https://github.com/dimaslanjaka/safelink/commit/5570edc>) Update README.md
- [ _2022-04-23 23:49:18_ ] [b6153b3](<https://github.com/dimaslanjaka/safelink/commit/b6153b3>) fix yarn start
- [ _2022-04-24 01:23:12_ ] [848022d](<https://github.com/dimaslanjaka/safelink/commit/848022d>) fix file watchers
- [ _2022-04-24 01:23:47_ ] [4dd3fca](<https://github.com/dimaslanjaka/safelink/commit/4dd3fca>) [windows] eol
- [ _2022-04-24 01:34:55_ ] [2ac5c01](<https://github.com/dimaslanjaka/safelink/commit/2ac5c01>) fix import by typescript
- [ _2022-04-24 01:58:38_ ] [2d508ec](<https://github.com/dimaslanjaka/safelink/commit/2d508ec>) fix node instance
- [ _2022-04-24 02:15:49_ ] [9682678](<https://github.com/dimaslanjaka/safelink/commit/9682678>) +fix fs webpack, +nodemon ignore
- [ _2022-04-24 02:22:23_ ] [095009f](<https://github.com/dimaslanjaka/safelink/commit/095009f>) fix nodemon
- [ _2022-04-24 02:29:52_ ] [3fc9d30](<https://github.com/dimaslanjaka/safelink/commit/3fc9d30>) remove dumper
- [ _2022-04-24 04:45:01_ ] [cb3d57d](<https://github.com/dimaslanjaka/safelink/commit/cb3d57d>) +ribbon
- [ _2022-04-24 05:07:19_ ] [2ce0af3](<https://github.com/dimaslanjaka/safelink/commit/2ce0af3>) [node] fix process content from string
- [ _2022-04-24 05:23:16_ ] [4fe6f3f](<https://github.com/dimaslanjaka/safelink/commit/4fe6f3f>) [node] fix parsing from string
- [ _2022-04-24 05:27:13_ ] [70a8997](<https://github.com/dimaslanjaka/safelink/commit/70a8997>) [gulp] dont copy d.ts
- [ _2022-04-24 05:29:24_ ] [45a42d7](<https://github.com/dimaslanjaka/safelink/commit/45a42d7>) Update README.md
- [ _2022-04-24 05:30:32_ ] [23e23d1](<https://github.com/dimaslanjaka/safelink/commit/23e23d1>) Update README.md
- [ _2022-04-24 06:08:37_ ] [2a33248](<https://github.com/dimaslanjaka/safelink/commit/2a33248>) fix index docs
- [ _2022-04-24 07:03:18_ ] [4e16d79](<https://github.com/dimaslanjaka/safelink/commit/4e16d79>) -nodemon no more limitation of watched files
- [ _2022-04-24 07:09:10_ ] [465d757](<https://github.com/dimaslanjaka/safelink/commit/465d757>) update docs
- [ _2022-04-24 07:27:01_ ] [cf8aced](<https://github.com/dimaslanjaka/safelink/commit/cf8aced>) update docs
- [ _2022-04-24 07:28:13_ ] [29a3116](<https://github.com/dimaslanjaka/safelink/commit/29a3116>) Update README.md
- [ _2022-04-24 07:30:06_ ] [2b69679](<https://github.com/dimaslanjaka/safelink/commit/2b69679>) Update README.md
- [ _2022-04-24 07:33:04_ ] [e92c6cf](<https://github.com/dimaslanjaka/safelink/commit/e92c6cf>) migrate to subfolder
### 1.0.2

- [ _2022-04-23 02:06:58_ ] [d55f1fd](<https://github.com/dimaslanjaka/safelink/commit/d55f1fd>) update 1.0.2
- [ _2022-04-23 02:10:01_ ] [ad07842](<https://github.com/dimaslanjaka/safelink/commit/ad07842>) +docs
- [ _2022-04-23 03:14:51_ ] [addce76](<https://github.com/dimaslanjaka/safelink/commit/addce76>) +layout redirector
### 0.0.0

- [ _2022-04-23 00:37:50_ ] [2e489c4](<https://github.com/dimaslanjaka/safelink/commit/2e489c4>) Update safelink.yml
- [ _2022-04-23 00:47:49_ ] [5fad709](<https://github.com/dimaslanjaka/safelink/commit/5fad709>) +submodule
- [ _2022-04-23 00:49:56_ ] [4a0be51](<https://github.com/dimaslanjaka/safelink/commit/4a0be51>) update deployment
- [ _2022-04-23 00:51:40_ ] [235d262](<https://github.com/dimaslanjaka/safelink/commit/235d262>) [workflow] update
- [ _2022-04-23 01:15:41_ ] [f9687a2](<https://github.com/dimaslanjaka/safelink/commit/f9687a2>) [workflow] test
- [ _2022-04-23 01:17:32_ ] [62e09f3](<https://github.com/dimaslanjaka/safelink/commit/62e09f3>) [workflow] test
- [ _2022-04-23 01:28:34_ ] [2266479](<https://github.com/dimaslanjaka/safelink/commit/2266479>) [workflow] test
- [ _2022-04-23 01:40:39_ ] [4034239](<https://github.com/dimaslanjaka/safelink/commit/4034239>) + .nojekyll
- [ _2022-04-23 01:43:18_ ] [a711a54](<https://github.com/dimaslanjaka/safelink/commit/a711a54>) fix bundle location
- [ _2022-04-23 01:53:21_ ] [36caf76](<https://github.com/dimaslanjaka/safelink/commit/36caf76>) [workflow] just test
- [ _2022-04-23 02:04:22_ ] [8af8a28](<https://github.com/dimaslanjaka/safelink/commit/8af8a28>) fix EJSHelper location