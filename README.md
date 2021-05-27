# To reproduce

- Install typescript: `yarn install`
- Run command `yarn tsc --build --watch` (or the alias `yarn watch`)
- Re-save one of the files `a.js`, `b.ts` or `tsconfig.json` to trigger an infinite loop on the watcher, constantly switching between the two console outputs `File change detected. Starting incremental compilation...` and `Found 0 errors. Watching for file changes.`

Tested on MacOS 11.4
