# Demonstration of Next 7 not working with next-sass

To try it out:
```bash
git clone https://github.com/JonAbrams/next-7-sass-fail.git
cd next-7-sass-fail
npm install
npm start
```

It will likely print out:
```
$ npm start

> next-7-sass-fail@1.0.0 start /Users/jon/code/next-7-test
> next

(node:8214) DeprecationWarning: Tapable.plugin is deprecated. Use new API on `.hooks` instead
[hardsource:6c715589] Using 4 MB of disk space.
[hardsource:6c715589] Writing new cache 6c715589...
[hardsource:9444bbfc] Writing new cache 9444bbfc...
[hardsource:6c715589] Tracking node dependencies with: package-lock.json.
[hardsource:9444bbfc] Tracking node dependencies with: package-lock.json.

Compiling

● client █████████████████████████ module and chunk tree optimization (77%) unnamed compat plugin 
 

● server █████████████████████████ module and chunk tree optimization (77%) unnamed compat plugin 
 

Error: Chunk.entrypoints: Use Chunks.groupsIterable and filter by instanceof Entrypoint instead
    at Chunk.get (/Users/jon/code/next-7-test/node_modules/webpack/lib/Chunk.js:824:9)
    at /Users/jon/code/next-7-test/node_modules/extract-text-webpack-plugin/dist/index.js:176:48
    at Array.forEach (<anonymous>)
    at /Users/jon/code/next-7-test/node_modules/extract-text-webpack-plugin/dist/index.js:171:18
    at AsyncSeriesHook.eval [as callAsync] (eval at create (/Users/jon/code/next-7-test/node_modules/tapable/lib/HookCodeFactory.js:32:10), <anonymous>:12:1)
    at AsyncSeriesHook.lazyCompileHook (/Users/jon/code/next-7-test/node_modules/tapable/lib/Hook.js:154:20)
    at Compilation.seal (/Users/jon/code/next-7-test/node_modules/webpack/lib/Compilation.js:1214:27)
    at hooks.make.callAsync.err (/Users/jon/code/next-7-test/node_modules/webpack/lib/Compiler.js:547:17)
    at _done (eval at create (/Users/jon/code/next-7-test/node_modules/tapable/lib/HookCodeFactory.js:32:10), <anonymous>:9:1)
    at _err2 (eval at create (/Users/jon/code/next-7-test/node_modules/tapable/lib/HookCodeFactory.js:32:10), <anonymous>:50:22)
    at Promise.all.then (/Users/jon/code/next-7-test/node_modules/webpack/lib/DynamicEntryPlugin.js:73:20)
    at <anonymous>
    at process._tickCallback (internal/process/next_tick.js:160:7)
Error: Chunk.entrypoints: Use Chunks.groupsIterable and filter by instanceof Entrypoint instead
    at Chunk.get (/Users/jon/code/next-7-test/node_modules/webpack/lib/Chunk.js:824:9)
    at /Users/jon/code/next-7-test/node_modules/extract-text-webpack-plugin/dist/index.js:176:48
    at Array.forEach (<anonymous>)
    at /Users/jon/code/next-7-test/node_modules/extract-text-webpack-plugin/dist/index.js:171:18
    at AsyncSeriesHook.eval [as callAsync] (eval at create (/Users/jon/code/next-7-test/node_modules/tapable/lib/HookCodeFactory.js:32:10), <anonymous>:12:1)
    at AsyncSeriesHook.lazyCompileHook (/Users/jon/code/next-7-test/node_modules/tapable/lib/Hook.js:154:20)
    at Compilation.seal (/Users/jon/code/next-7-test/node_modules/webpack/lib/Compilation.js:1214:27)
    at hooks.make.callAsync.err (/Users/jon/code/next-7-test/node_modules/webpack/lib/Compiler.js:547:17)
    at _done (eval at create (/Users/jon/code/next-7-test/node_modules/tapable/lib/HookCodeFactory.js:32:10), <anonymous>:9:1)
    at _err2 (eval at create (/Users/jon/code/next-7-test/node_modules/tapable/lib/HookCodeFactory.js:32:10), <anonymous>:50:22)
    at Promise.all.then (/Users/jon/code/next-7-test/node_modules/webpack/lib/DynamicEntryPlugin.js:73:20)
    at <anonymous>
    at process._tickCallback (internal/process/next_tick.js:160:7)
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! next-7-sass-fail@1.0.0 start: `next`
npm ERR! Exit status 1
npm ERR! 
npm ERR! Failed at the next-7-sass-fail@1.0.0 start script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in:
npm ERR!     /Users/jon/.npm/_logs/2018-09-19T18_20_47_012Z-debug.log
```
