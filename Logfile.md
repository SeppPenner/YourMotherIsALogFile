I have NVM running on Windows (https://github.com/coreybutler/nvm-windows), version 1.1.12, node version 21.4.0 and tried to follow https://github.com/eclipse-sparkplug/sparkplug/blob/develop/tck/UserGuide.adoc:

```bash
npm install -g yarn
corepack enable
yarn install
```

throws some errors with `yarn install` (AND again I know why I hate all that node.js shit)

```log
➤ YN0000: ┌ Resolution step
➤ YN0061: │ @babel/plugin-proposal-private-property-in-object@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-private-property-in-object instead.
➤ YN0061: │ core-js@npm:3.16.2 is deprecated: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
➤ YN0061: │ core-js@npm:2.6.12 is deprecated: core-js@<3.23.3 is no longer maintained and not recommended for usage due to the number of issues. Because of the V8 engine whims, feature detection in old core-js versions could cause a slowdown up to 100x even if nothing is polyfilled. Some versions have web compatibility issues. Please, upgrade your dependencies to the actual version of core-js.
➤ YN0061: │ popper.js@npm:1.16.1 is deprecated: You can find the new Popper v2 at @popperjs/core, this package is dedicated to the legacy v1
➤ YN0061: │ @babel/plugin-proposal-private-methods@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-private-methods instead.
➤ YN0061: │ @babel/plugin-proposal-nullish-coalescing-operator@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-nullish-coalescing-operator instead.
➤ YN0061: │ @babel/plugin-proposal-class-properties@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-class-properties instead.
➤ YN0061: │ @babel/plugin-proposal-optional-chaining@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-optional-chaining instead.
➤ YN0061: │ @babel/plugin-proposal-logical-assignment-operators@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-logical-assignment-operators instead.
➤ YN0061: │ @babel/plugin-proposal-class-static-block@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-class-static-block instead.
➤ YN0061: │ @babel/plugin-proposal-numeric-separator@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-numeric-separator instead.
➤ YN0061: │ @babel/plugin-proposal-export-namespace-from@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-export-namespace-from instead.
➤ YN0061: │ @babel/plugin-proposal-json-strings@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-json-strings instead.
➤ YN0061: │ @babel/plugin-proposal-unicode-property-regex@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-unicode-property-regex instead.
➤ YN0061: │ @babel/plugin-proposal-object-rest-spread@npm:7.14.7 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-object-rest-spread instead.
➤ YN0061: │ querystring@npm:0.2.1 is deprecated: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
➤ YN0061: │ @babel/plugin-proposal-optional-catch-binding@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-optional-catch-binding instead.
➤ YN0061: │ @babel/plugin-proposal-async-generator-functions@npm:7.14.9 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-async-generator-functions instead.
➤ YN0061: │ ufo@npm:0.7.9 is deprecated: security: please use latest version
➤ YN0032: │ fsevents@npm:2.3.2: Implicit dependencies on node-gyp are discouraged
➤ YN0032: │ fsevents@npm:2.3.2: Implicit dependencies on node-gyp are discouraged
➤ YN0061: │ svgo@npm:1.3.2 is deprecated: This SVGO version is no longer supported. Upgrade to v2.x.x.
➤ YN0061: │ flatten@npm:1.0.3 is deprecated: flatten is deprecated in favor of utility frameworks such as lodash.
➤ YN0061: │ stable@npm:0.1.8 is deprecated: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility
➤ YN0061: │ @babel/plugin-proposal-dynamic-import@npm:7.14.5 is deprecated: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-dynamic-import instead.
➤ YN0061: │ consolidate@npm:0.15.1 is deprecated: Please upgrade to consolidate v1.0.0+ as it has been modernized with several long-awaited fixes implemented. Maintenance is supported by Forward Email at https://forwardemail.net ; follow/watch https://github.com/ladjs/consolidate for updates and release changelog
➤ YN0061: │ @npmcli/move-file@npm:1.1.2 is deprecated: This functionality has been moved to @npmcli/fs
➤ YN0061: │ source-map-resolve@npm:0.5.3 is deprecated: See https://github.com/lydell/source-map-resolve#deprecated
➤ YN0061: │ source-map-url@npm:0.4.1 is deprecated: See https://github.com/lydell/source-map-url#deprecated
➤ YN0061: │ urix@npm:0.1.0 is deprecated: Please see https://github.com/lydell/urix#deprecated
➤ YN0061: │ querystring@npm:0.2.0 is deprecated: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
➤ YN0061: │ resolve-url@npm:0.2.1 is deprecated: https://github.com/lydell/resolve-url#deprecated
➤ YN0061: │ chokidar@npm:2.1.8 is deprecated: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
➤ YN0061: │ fsevents@npm:1.2.13 is deprecated: The v1 package contains DANGEROUS / INSECURE binaries. Upgrade to safe fsevents v2
➤ YN0032: │ nan@npm:2.15.0: Implicit dependencies on node-gyp are discouraged
➤ YN0032: │ evp_bytestokey@npm:1.0.3: Implicit dependencies on node-gyp are discouraged
➤ YN0002: │ @nuxt/webpack@npm:2.15.8 doesn't provide @vue/compiler-sfc (p606e8), requested by vue-loader
➤ YN0002: │ bootstrap-vue@npm:2.21.2 doesn't provide jquery (p718d2), requested by bootstrap
➤ YN0002: │ bootstrap-vue@npm:2.21.2 doesn't provide vue (p679d5), requested by portal-vue
➤ YN0002: │ nuxt@npm:2.15.8 doesn't provide consola (p2d844), requested by @nuxt/components
➤ YN0002: │ webconsole@workspace:. doesn't provide jquery (p7075c), requested by bootstrap
➤ YN0002: │ webconsole@workspace:. doesn't provide popper.js (paffe7), requested by bootstrap
➤ YN0000: │ Some peer dependencies are incorrectly met; run yarn explain peer-requirements <hash> for details, where <hash> is the six-letter p-prefixed code
➤ YN0000: └ Completed in 6s 710ms
➤ YN0000: ┌ Fetch step
➤ YN0013: │ @babel/helper-validator-option@npm:7.14.5 can't be found in the cache and will be fetched from the remote r
➤ YN0013: │ @babel/helper-wrap-function@npm:7.14.5 can't be found in the cache and will be fetched from the remote regi
➤ YN0013: │ @babel/helpers@npm:7.15.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ @babel/highlight@npm:7.14.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ @babel/parser@npm:7.15.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-bugfix-v8-spread-parameters-in-optional-chaining@npm:7.14.5 can't be found in the cache and w
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-async-generator-functions@npm:7.14.9 can't be found in the cache and will be fetched
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-class-properties@npm:7.14.5 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-class-static-block@npm:7.14.5 can't be found in the cache and will be fetched from t
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-decorators@npm:7.14.5 can't be found in the cache and will be fetched from the remot
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-dynamic-import@npm:7.14.5 can't be found in the cache and will be fetched from the r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-export-namespace-from@npm:7.14.5 can't be found in the cache and will be fetched fro
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-json-strings@npm:7.14.5 can't be found in the cache and will be fetched from the rem
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-logical-assignment-operators@npm:7.14.5 can't be found in the cache and will be fetc
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-nullish-coalescing-operator@npm:7.14.5 can't be found in the cache and will be fetch
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-numeric-separator@npm:7.14.5 can't be found in the cache and will be fetched from th
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-object-rest-spread@npm:7.14.7 can't be found in the cache and will be fetched from t
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-optional-catch-binding@npm:7.14.5 can't be found in the cache and will be fetched fr
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-optional-chaining@npm:7.14.5 can't be found in the cache and will be fetched from th
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-private-methods@npm:7.14.5 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-private-property-in-object@npm:7.14.5 can't be found in the cache and will be fetche
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-proposal-unicode-property-regex@npm:7.14.5 can't be found in the cache and will be fetched fr
➤ YN0013: │ @babel/plugin-syntax-async-generators@npm:7.8.4 can't be found in the cache and will be fetched from the re
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-class-properties@npm:7.12.13 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-class-static-block@npm:7.14.5 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-decorators@npm:7.14.5 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-dynamic-import@npm:7.8.3 can't be found in the cache and will be fetched from the remo
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-export-namespace-from@npm:7.8.3 can't be found in the cache and will be fetched from t
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-json-strings@npm:7.8.3 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-jsx@npm:7.14.5 can't be found in the cache and will be fetched from the remote registr
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-logical-assignment-operators@npm:7.10.4 can't be found in the cache and will be fetche
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-nullish-coalescing-operator@npm:7.8.3 can't be found in the cache and will be fetched
➤ YN0013: │ @babel/plugin-syntax-numeric-separator@npm:7.10.4 can't be found in the cache and will be fetched from the
➤ YN0013: │ @babel/plugin-syntax-object-rest-spread@npm:7.8.3 can't be found in the cache and will be fetched from the
➤ YN0013: │ @babel/plugin-syntax-optional-catch-binding@npm:7.8.3 can't be found in the cache and will be fetched from
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-optional-chaining@npm:7.8.3 can't be found in the cache and will be fetched from the r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-private-property-in-object@npm:7.14.5 can't be found in the cache and will be fetched
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-syntax-top-level-await@npm:7.14.5 can't be found in the cache and will be fetched from the re
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-arrow-functions@npm:7.14.5 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-async-to-generator@npm:7.14.5 can't be found in the cache and will be fetched from
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-block-scoped-functions@npm:7.14.5 can't be found in the cache and will be fetched f
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-block-scoping@npm:7.15.3 can't be found in the cache and will be fetched from the r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-classes@npm:7.14.9 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-computed-properties@npm:7.14.5 can't be found in the cache and will be fetched from
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-destructuring@npm:7.14.7 can't be found in the cache and will be fetched from the r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-dotall-regex@npm:7.14.5 can't be found in the cache and will be fetched from the re
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-duplicate-keys@npm:7.14.5 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-exponentiation-operator@npm:7.14.5 can't be found in the cache and will be fetched
➤ YN0013: │ @babel/plugin-transform-for-of@npm:7.14.5 can't be found in the cache and will be fetched from the remote r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-function-name@npm:7.14.5 can't be found in the cache and will be fetched from the r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-literals@npm:7.14.5 can't be found in the cache and will be fetched from the remote
➤ YN0013: │ @babel/plugin-transform-member-expression-literals@npm:7.14.5 can't be found in the cache and will be fetch
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-modules-amd@npm:7.14.5 can't be found in the cache and will be fetched from the rem
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-modules-commonjs@npm:7.15.0 can't be found in the cache and will be fetched from th
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-modules-systemjs@npm:7.14.5 can't be found in the cache and will be fetched from th
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-modules-umd@npm:7.14.5 can't be found in the cache and will be fetched from the rem
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-named-capturing-groups-regex@npm:7.14.9 can't be found in the cache and will be fet
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-new-target@npm:7.14.5 can't be found in the cache and will be fetched from the remo
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-object-super@npm:7.14.5 can't be found in the cache and will be fetched from the re
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-parameters@npm:7.14.5 can't be found in the cache and will be fetched from the remo
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-property-literals@npm:7.14.5 can't be found in the cache and will be fetched from t
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-regenerator@npm:7.14.5 can't be found in the cache and will be fetched from the rem
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-reserved-words@npm:7.14.5 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-runtime@npm:7.15.0 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-shorthand-properties@npm:7.14.5 can't be found in the cache and will be fetched fro
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-spread@npm:7.14.6 can't be found in the cache and will be fetched from the remote r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-sticky-regex@npm:7.14.5 can't be found in the cache and will be fetched from the re
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-template-literals@npm:7.14.5 can't be found in the cache and will be fetched from t
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-typeof-symbol@npm:7.14.5 can't be found in the cache and will be fetched from the r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-unicode-escapes@npm:7.14.5 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/plugin-transform-unicode-regex@npm:7.14.5 can't be found in the cache and will be fetched from the r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/preset-env@npm:7.15.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/preset-modules@npm:0.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/runtime@npm:7.15.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/template@npm:7.14.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/traverse@npm:7.15.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @babel/types@npm:7.15.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ @babel/types@npm:7.23.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @csstools/convert-colors@npm:1.4.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @isaacs/cliui@npm:8.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nodelib/fs.scandir@npm:2.1.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nodelib/fs.stat@npm:2.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nodelib/fs.walk@npm:1.2.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @npmcli/agent@npm:2.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @npmcli/fs@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @npmcli/move-file@npm:1.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/babel-preset-app@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/builder@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/cli@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/components@npm:2.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ @nuxt/config@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ @nuxt/core@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/devalue@npm:1.2.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ @nuxt/friendly-errors-webpack-plugin@npm:2.5.1 can't be found in the cache and will be fetched from the rem
➤ YN0013: │ @nuxt/generator@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ @nuxt/loading-screen@npm:2.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/opencollective@npm:0.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/server@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/telemetry@npm:1.3.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/utils@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/vue-app@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/vue-renderer@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxt/webpack@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @nuxtjs/youch@npm:4.2.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @pkgjs/parseargs@npm:0.11.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @polka/url@npm:1.0.0-next.17 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @types/html-minifier-terser@npm:5.1.2 can't be found in the cache and will be fetched from the remote regis
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @types/json-schema@npm:7.0.9 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @types/node@npm:16.6.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @types/q@npm:1.5.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @types/source-list-map@npm:0.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @types/tapable@npm:1.0.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @types/uglify-js@npm:3.13.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @types/webpack-sources@npm:3.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @types/webpack@npm:4.41.30 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/babel-helper-vue-jsx-merge-props@npm:1.2.1 can't be found in the cache and will be fetched from the re
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/babel-plugin-transform-vue-jsx@npm:1.2.1 can't be found in the cache and will be fetched from the remo
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/babel-preset-jsx@npm:1.2.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/babel-sugar-composition-api-inject-h@npm:1.2.1 can't be found in the cache and will be fetched from th
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/babel-sugar-composition-api-render-instance@npm:1.2.4 can't be found in the cache and will be fetched
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/babel-sugar-functional-vue@npm:1.2.2 can't be found in the cache and will be fetched from the remote r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/babel-sugar-inject-h@npm:1.2.2 can't be found in the cache and will be fetched from the remote registr
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/babel-sugar-v-model@npm:1.2.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/babel-sugar-v-on@npm:1.2.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @vue/component-compiler-utils@npm:3.2.2 can't be found in the cache and will be fetched from the remote reg
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/ast@npm:1.9.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/floating-point-hex-parser@npm:1.9.0 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/helper-api-error@npm:1.9.0 can't be found in the cache and will be fetched from the remote r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/helper-buffer@npm:1.9.0 can't be found in the cache and will be fetched from the remote regi
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/helper-code-frame@npm:1.9.0 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/helper-fsm@npm:1.9.0 can't be found in the cache and will be fetched from the remote registr
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/helper-module-context@npm:1.9.0 can't be found in the cache and will be fetched from the rem
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/helper-wasm-bytecode@npm:1.9.0 can't be found in the cache and will be fetched from the remo
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/helper-wasm-section@npm:1.9.0 can't be found in the cache and will be fetched from the remot
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/ieee754@npm:1.9.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/leb128@npm:1.9.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/utf8@npm:1.9.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/wasm-edit@npm:1.9.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/wasm-gen@npm:1.9.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/wasm-opt@npm:1.9.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/wasm-parser@npm:1.9.0 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/wast-parser@npm:1.9.0 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @webassemblyjs/wast-printer@npm:1.9.0 can't be found in the cache and will be fetched from the remote regis
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @xtuc/ieee754@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ @xtuc/long@npm:4.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ abbrev@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ accepts@npm:1.3.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ acorn-walk@npm:8.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ acorn@npm:6.4.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ acorn@npm:8.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ agent-base@npm:7.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ aggregate-error@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ajv-errors@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ajv-keywords@npm:3.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ajv@npm:6.12.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ alphanum-sort@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-align@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-escapes@npm:4.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-html@npm:0.0.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-regex@npm:2.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-regex@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-regex@npm:4.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-regex@npm:5.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-regex@npm:5.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-regex@npm:6.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-styles@npm:2.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-styles@npm:3.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-styles@npm:4.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ansi-styles@npm:6.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ anymatch@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ anymatch@npm:3.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ aproba@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ arg@npm:5.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ argparse@npm:1.0.10 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ arr-diff@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ arr-flatten@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ arr-union@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ array-union@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ array-unique@npm:0.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ asn1.js@npm:5.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ assert@npm:1.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ assign-symbols@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ async-each@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ at-least-node@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ atob@npm:2.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ autoprefixer@npm:9.8.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ babel-loader@npm:8.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ babel-plugin-dynamic-import-node@npm:2.3.3 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ babel-plugin-polyfill-corejs2@npm:0.2.2 can't be found in the cache and will be fetched from the remote reg
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ babel-plugin-polyfill-corejs3@npm:0.2.4 can't be found in the cache and will be fetched from the remote reg
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ babel-plugin-polyfill-regenerator@npm:0.2.2 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ balanced-match@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ base64-js@npm:1.5.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ base@npm:0.11.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ big.js@npm:5.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ binary-extensions@npm:1.13.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ binary-extensions@npm:2.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ bindings@npm:1.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ bl@npm:4.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ bluebird@npm:3.7.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ bn.js@npm:4.12.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ bn.js@npm:5.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ boolbase@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ bootstrap-vue@npm:2.21.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ bootstrap@npm:4.6.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ boxen@npm:5.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ brace-expansion@npm:1.1.11 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ brace-expansion@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ braces@npm:2.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ braces@npm:3.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ brorand@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ browserify-aes@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ browserify-cipher@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ browserify-des@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ browserify-rsa@npm:4.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ browserify-sign@npm:4.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ browserify-zlib@npm:0.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ browserslist@npm:4.16.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ buffer-from@npm:1.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ buffer-json@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ buffer-xor@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ buffer@npm:4.9.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ buffer@npm:5.7.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ builtin-status-codes@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ bytes@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cacache@npm:12.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ cacache@npm:15.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ cacache@npm:18.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cache-base@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cache-loader@npm:4.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ call-bind@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ caller-callsite@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ caller-path@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ callsites@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ camel-case@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ camel-case@npm:4.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ camelcase@npm:5.3.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ camelcase@npm:6.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ caniuse-api@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ caniuse-lite@npm:1.0.30001251 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ chalk@npm:1.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ chalk@npm:2.4.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ chalk@npm:4.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ chardet@npm:0.7.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ chokidar@npm:2.1.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ chokidar@npm:3.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ chownr@npm:1.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ chownr@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ chrome-trace-event@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ci-info@npm:3.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cipher-base@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ class-utils@npm:0.3.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ clean-css@npm:4.2.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ clean-stack@npm:2.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cli-boxes@npm:2.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cli-cursor@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cli-width@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ clipboard@npm:2.0.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ coa@npm:2.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ collection-visit@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ color-convert@npm:1.9.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ color-convert@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ color-name@npm:1.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ color-name@npm:1.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ color-string@npm:1.6.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ color@npm:3.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ colorette@npm:1.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ commander@npm:2.20.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ commander@npm:4.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ commander@npm:6.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ commist@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ commondir@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ component-emitter@npm:1.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ compressible@npm:2.0.18 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ compression@npm:1.7.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ concat-map@npm:0.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ concat-stream@npm:1.6.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ concat-stream@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ connect@npm:3.7.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ consola@npm:2.15.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ console-browserify@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ consolidate@npm:0.15.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ constants-browserify@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ convert-source-map@npm:1.8.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cookie@npm:0.3.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ copy-concurrently@npm:1.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ copy-descriptor@npm:0.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ core-js-compat@npm:3.16.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ core-js@npm:2.6.12 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ core-js@npm:3.16.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ core-util-is@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cosmiconfig@npm:5.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ crc@npm:3.8.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ create-ecdh@npm:4.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ create-hash@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ create-hmac@npm:1.1.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ create-require@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cross-spawn@npm:7.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ crypto-browserify@npm:3.12.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-blank-pseudo@npm:0.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-color-names@npm:0.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-declaration-sorter@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-has-pseudo@npm:0.10.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-loader@npm:4.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-prefers-color-scheme@npm:3.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-select-base-adapter@npm:0.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-select@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-select@npm:4.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-tree@npm:1.0.0-alpha.37 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-tree@npm:1.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-what@npm:3.4.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ css-what@npm:5.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cssdb@npm:4.4.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cssesc@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cssesc@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cssnano-preset-default@npm:4.0.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cssnano-util-get-arguments@npm:4.0.0 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cssnano-util-get-match@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cssnano-util-raw-cache@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cssnano-util-same-parent@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cssnano@npm:4.1.11 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ csso@npm:4.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cuint@npm:0.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ cyclist@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ de-indent@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ debug@npm:2.6.9 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ debug@npm:4.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ debug@npm:4.3.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ decode-uri-component@npm:0.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ deepmerge@npm:4.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ define-properties@npm:1.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ define-property@npm:0.2.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ define-property@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ define-property@npm:2.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ defu@npm:2.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ defu@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ defu@npm:5.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ delegate@npm:3.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ depd@npm:1.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ des.js@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ destr@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ destroy@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ detect-indent@npm:5.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ devalue@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ diffie-hellman@npm:5.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ dir-glob@npm:3.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ dom-converter@npm:0.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ dom-serializer@npm:0.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ dom-serializer@npm:1.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ domain-browser@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ domelementtype@npm:1.3.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ domelementtype@npm:2.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ domhandler@npm:4.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ domutils@npm:1.7.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ domutils@npm:2.7.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ dot-case@npm:3.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ dot-prop@npm:5.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ dotenv@npm:9.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ duplexer@npm:0.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ duplexify@npm:3.7.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ duplexify@npm:4.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ eastasianwidth@npm:0.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ee-first@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ electron-to-chromium@npm:1.3.812 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ elliptic@npm:6.5.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ emoji-regex@npm:7.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ emoji-regex@npm:8.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ emoji-regex@npm:9.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ emojis-list@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ encodeurl@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ encoding@npm:0.1.13 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ end-of-stream@npm:1.4.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ enhanced-resolve@npm:4.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ entities@npm:2.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ env-paths@npm:2.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ err-code@npm:2.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ errno@npm:0.1.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ error-ex@npm:1.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ error-stack-parser@npm:2.0.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ es-abstract@npm:1.18.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ es-to-primitive@npm:1.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ escalade@npm:3.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ escape-html@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ escape-string-regexp@npm:1.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ eslint-scope@npm:4.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ esprima@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ esrecurse@npm:4.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ estraverse@npm:4.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ estraverse@npm:5.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ esutils@npm:2.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ etag@npm:1.8.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ events@npm:3.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ eventsource-polyfill@npm:0.9.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ evp_bytestokey@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ execa@npm:5.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ exit@npm:0.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ expand-brackets@npm:2.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ exponential-backoff@npm:3.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ extend-shallow@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ extend-shallow@npm:3.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ external-editor@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ extglob@npm:2.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ extract-css-chunks-webpack-plugin@npm:4.9.0 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fast-deep-equal@npm:3.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fast-glob@npm:3.2.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fast-json-stable-stringify@npm:2.1.0 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fastq@npm:1.11.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ figgy-pudding@npm:3.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ figures@npm:3.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ file-loader@npm:6.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ file-uri-to-path@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fill-range@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fill-range@npm:7.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ filter-obj@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ finalhandler@npm:1.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ find-cache-dir@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ find-cache-dir@npm:3.3.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ find-up@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ find-up@npm:4.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ flat@npm:5.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ flatten@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ flush-write-stream@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ for-in@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ foreground-child@npm:3.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fragment-cache@npm:0.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fresh@npm:0.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ from2@npm:2.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fs-extra@npm:8.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fs-extra@npm:9.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fs-memo@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fs-minipass@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fs-minipass@npm:3.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fs-monkey@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fs-write-stream-atomic@npm:1.0.10 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fs.realpath@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fsevents@npm:1.2.13 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fsevents@npm:2.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fsevents@patch:fsevents@npm%3A1.2.13#~builtin<compat/fsevents>::version=1.2.13&hash=1cc4b2 can't be found i
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ fsevents@patch:fsevents@npm%3A2.3.2#~builtin<compat/fsevents>::version=2.3.2&hash=1cc4b2 can't be found in
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ function-bind@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ gensync@npm:1.0.0-beta.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ get-intrinsic@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ get-port-please@npm:2.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ get-stream@npm:6.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ get-value@npm:2.0.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ git-config-path@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ git-up@npm:4.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ git-url-parse@npm:11.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ glob-parent@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ glob-parent@npm:5.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ glob@npm:10.3.10 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ glob@npm:7.1.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ globals@npm:11.12.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ globby@npm:11.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ good-listener@npm:1.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ graceful-fs@npm:4.2.11 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ graceful-fs@npm:4.2.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ gzip-size@npm:6.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ hable@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ hard-source-webpack-plugin@npm:0.13.1 can't be found in the cache and will be fetched from the remote regis
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has-ansi@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has-bigints@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has-flag@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has-flag@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has-symbols@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has-tostringtag@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has-value@npm:0.3.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has-value@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ has-values@npm:0.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has-values@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ has@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ hash-base@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ hash-sum@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ hash-sum@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ hash.js@npm:1.1.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ he@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ help-me@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ hex-color-regex@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ hmac-drbg@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ hsl-regex@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ hsla-regex@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ html-entities@npm:1.4.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ html-minifier-terser@npm:5.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ html-minifier@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ html-tags@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ html-webpack-plugin@npm:4.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ htmlparser2@npm:6.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ http-cache-semantics@npm:4.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ http-errors@npm:1.7.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ http-proxy-agent@npm:7.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ https-browserify@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ https-proxy-agent@npm:7.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ human-signals@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ iconv-lite@npm:0.4.24 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ iconv-lite@npm:0.6.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ icss-utils@npm:4.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ieee754@npm:1.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ iferr@npm:0.1.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ignore@npm:5.1.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ import-cwd@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ import-fresh@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ import-from@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ imurmurhash@npm:0.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ indent-string@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ indexes-of@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ infer-owner@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ inflight@npm:1.0.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ inherits@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ inherits@npm:2.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ inherits@npm:2.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ini@npm:1.3.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ inquirer@npm:7.3.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ internal-slot@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ip@npm:1.1.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ip@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-absolute-url@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-accessor-descriptor@npm:0.1.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-accessor-descriptor@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-arrayish@npm:0.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-arrayish@npm:0.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-bigint@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-binary-path@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-binary-path@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-boolean-object@npm:1.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-buffer@npm:1.1.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-callable@npm:1.2.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-color-stop@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-core-module@npm:2.6.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-data-descriptor@npm:0.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-data-descriptor@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-date-object@npm:1.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-descriptor@npm:0.1.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-descriptor@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-directory@npm:0.3.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-docker@npm:2.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-extendable@npm:0.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-extendable@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ is-extglob@npm:2.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-fullwidth-code-point@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-fullwidth-code-point@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-glob@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-glob@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-lambda@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-negative-zero@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-number-object@npm:1.0.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-number@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-number@npm:7.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-obj@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-plain-obj@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-plain-object@npm:2.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-regex@npm:1.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-resolvable@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-ssh@npm:1.3.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-stream@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-string@npm:1.0.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-symbol@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-windows@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ is-wsl@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ isarray@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ isexe@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ isexe@npm:3.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ isobject@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ isobject@npm:3.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ jackspeak@npm:2.3.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ jest-worker@npm:26.6.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ jiti@npm:1.11.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ js-tokens@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ js-yaml@npm:3.14.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ jsesc@npm:0.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ jsesc@npm:2.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ json-parse-better-errors@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ json-schema-traverse@npm:0.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ json5@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ json5@npm:2.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ jsonfile@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ jsonfile@npm:6.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ kind-of@npm:3.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ kind-of@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ kind-of@npm:5.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ kind-of@npm:6.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ last-call-webpack-plugin@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ launch-editor-middleware@npm:2.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ launch-editor@npm:2.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ leven@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ loader-runner@npm:2.4.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ loader-runner@npm:4.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ loader-utils@npm:1.4.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ loader-utils@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ locate-path@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ locate-path@npm:5.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lodash._reinterpolate@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ lodash.debounce@npm:4.0.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ lodash.kebabcase@npm:4.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lodash.memoize@npm:4.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ lodash.template@npm:4.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lodash.templatesettings@npm:4.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lodash.uniq@npm:4.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lodash@npm:4.17.21 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lower-case@npm:1.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lower-case@npm:2.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lru-cache@npm:10.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lru-cache@npm:4.1.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lru-cache@npm:5.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ lru-cache@npm:6.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ make-dir@npm:1.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ make-dir@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ make-dir@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ make-fetch-happen@npm:13.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ map-age-cleaner@npm:0.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ map-cache@npm:0.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ map-visit@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ md5.js@npm:1.3.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mdn-data@npm:2.0.14 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mdn-data@npm:2.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mem@npm:8.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ memfs@npm:3.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ memory-fs@npm:0.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ memory-fs@npm:0.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ merge-source-map@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ merge-stream@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ merge2@npm:1.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ micromatch@npm:3.1.10 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ micromatch@npm:4.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ miller-rabin@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mime-db@npm:1.49.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mime-types@npm:2.1.32 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mime@npm:1.6.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mime@npm:2.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mimic-fn@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mimic-fn@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minimalistic-assert@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minimalistic-crypto-utils@npm:1.0.1 can't be found in the cache and will be fetched from the remote registr
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minimatch@npm:3.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minimatch@npm:9.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minimist@npm:1.2.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minipass-collect@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minipass-collect@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minipass-fetch@npm:3.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minipass-flush@npm:1.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minipass-pipeline@npm:1.2.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minipass-sized@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minipass@npm:3.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minipass@npm:5.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minipass@npm:7.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ minizlib@npm:2.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mississippi@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mixin-deep@npm:1.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mkdirp@npm:0.5.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mkdirp@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ move-concurrently@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mqtt-packet@npm:6.10.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mqtt@npm:4.2.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ms@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ms@npm:2.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ms@npm:2.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mustache@npm:2.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ mute-stream@npm:0.0.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ nan@npm:2.15.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ nanoid@npm:3.1.25 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ nanomatch@npm:1.2.13 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ negotiator@npm:0.6.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ negotiator@npm:0.6.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ neo-async@npm:2.6.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ no-case@npm:2.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ no-case@npm:3.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ node-fetch@npm:2.6.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ node-gyp@npm:10.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ node-html-parser@npm:3.3.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ node-libs-browser@npm:2.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ node-object-hash@npm:1.4.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ node-releases@npm:1.1.75 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ node-res@npm:5.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ nopt@npm:7.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ normalize-path@npm:2.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ normalize-path@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ normalize-range@npm:0.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ normalize-url@npm:1.9.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ normalize-url@npm:3.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ normalize-url@npm:6.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ npm-run-path@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ nth-check@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ nth-check@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ num2fraction@npm:1.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ nuxt-clipboard2@npm:0.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ nuxt@npm:2.15.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ object-assign@npm:4.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ object-copy@npm:0.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ object-inspect@npm:1.11.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ object-keys@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ object-visit@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ object.assign@npm:4.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ object.getownpropertydescriptors@npm:2.1.2 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ object.pick@npm:1.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ object.values@npm:1.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ on-finished@npm:2.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ on-headers@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ once@npm:1.4.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ onetime@npm:5.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ opener@npm:1.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ optimize-css-assets-webpack-plugin@npm:5.0.8 can't be found in the cache and will be fetched from the remot
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ os-browserify@npm:0.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ os-tmpdir@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ p-defer@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ p-limit@npm:2.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ p-limit@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ p-locate@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ p-locate@npm:4.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ p-map@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ p-try@npm:2.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ paho-mqtt@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ pako@npm:1.0.11 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ parallel-transform@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ param-case@npm:2.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ param-case@npm:3.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ parse-asn1@npm:5.1.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ parse-git-config@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ parse-json@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ parse-path@npm:4.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ parse-url@npm:6.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ parseurl@npm:1.3.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pascal-case@npm:3.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pascalcase@npm:0.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ path-browserify@npm:0.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ path-dirname@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ path-exists@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ path-exists@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ path-is-absolute@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ path-key@npm:3.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ path-parse@npm:1.0.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ path-scurry@npm:1.10.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ path-type@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pbkdf2@npm:3.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ picomatch@npm:2.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pify@npm:2.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pify@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pify@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pify@npm:5.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pkg-dir@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pkg-dir@npm:4.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pnp-webpack-plugin@npm:1.7.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ popper.js@npm:1.16.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ portal-vue@npm:2.1.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ posix-character-classes@npm:0.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-attribute-case-insensitive@npm:4.0.2 can't be found in the cache and will be fetched from the remot
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-calc@npm:7.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-color-functional-notation@npm:2.0.1 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-color-gray@npm:5.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-color-hex-alpha@npm:5.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-color-mod-function@npm:3.0.3 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-color-rebeccapurple@npm:4.0.1 can't be found in the cache and will be fetched from the remote regis
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-colormin@npm:4.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-convert-values@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-custom-media@npm:7.0.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-custom-properties@npm:8.0.11 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-custom-selectors@npm:5.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-dir-pseudo-class@npm:5.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-discard-comments@npm:4.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-discard-duplicates@npm:4.0.2 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-discard-empty@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-discard-overridden@npm:4.0.1 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-double-position-gradients@npm:1.0.0 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-env-function@npm:2.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-focus-visible@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-focus-within@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-font-variant@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-gap-properties@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-image-set-function@npm:3.0.1 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-import-resolver@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-import@npm:12.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-initial@npm:3.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-lab-function@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-load-config@npm:2.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-loader@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-logical@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-media-minmax@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-merge-longhand@npm:4.0.11 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-merge-rules@npm:4.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-minify-font-values@npm:4.0.2 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-minify-gradients@npm:4.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-minify-params@npm:4.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-minify-selectors@npm:4.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-modules-extract-imports@npm:2.0.0 can't be found in the cache and will be fetched from the remote r
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-modules-local-by-default@npm:3.0.3 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-modules-scope@npm:2.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-modules-values@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-nesting@npm:7.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-normalize-charset@npm:4.0.1 can't be found in the cache and will be fetched from the remote registr
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-normalize-display-values@npm:4.0.2 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-normalize-positions@npm:4.0.2 can't be found in the cache and will be fetched from the remote regis
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-normalize-repeat-style@npm:4.0.2 can't be found in the cache and will be fetched from the remote re
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-normalize-string@npm:4.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-normalize-timing-functions@npm:4.0.2 can't be found in the cache and will be fetched from the remot
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-normalize-unicode@npm:4.0.1 can't be found in the cache and will be fetched from the remote registr
➤ YN0013: │ postcss-normalize-url@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ postcss-normalize-whitespace@npm:4.0.2 can't be found in the cache and will be fetched from the remote regi
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-ordered-values@npm:4.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-overflow-shorthand@npm:2.0.0 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-page-break@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-place@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-preset-env@npm:6.7.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-pseudo-class-any-link@npm:6.0.0 can't be found in the cache and will be fetched from the remote reg
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-reduce-initial@npm:4.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-reduce-transforms@npm:4.0.2 can't be found in the cache and will be fetched from the remote registr
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-replace-overflow-wrap@npm:3.0.0 can't be found in the cache and will be fetched from the remote reg
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-selector-matches@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-selector-not@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-selector-parser@npm:3.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-selector-parser@npm:5.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-selector-parser@npm:6.0.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-svgo@npm:4.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-unique-selectors@npm:4.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-url@npm:8.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-value-parser@npm:3.3.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-value-parser@npm:4.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss-values-parser@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ postcss@npm:7.0.36 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ prepend-http@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ prettier@npm:1.19.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pretty-bytes@npm:5.6.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pretty-error@npm:2.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pretty-time@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ proc-log@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ process-nextick-args@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ process@npm:0.11.10 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ promise-inflight@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ promise-retry@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ proper-lockfile@npm:4.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ protocols@npm:1.4.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ prr@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pseudomap@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ public-encrypt@npm:4.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pump@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pump@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ pumpify@npm:1.5.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ punycode@npm:1.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ punycode@npm:1.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ punycode@npm:2.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ q@npm:1.5.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ qs@npm:6.10.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ query-string@npm:4.3.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ query-string@npm:6.14.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ querystring-es3@npm:0.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ querystring@npm:0.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ querystring@npm:0.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ queue-microtask@npm:1.2.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ randombytes@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ randomfill@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ range-parser@npm:1.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ rc9@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ read-cache@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ readable-stream@npm:2.3.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ readable-stream@npm:3.6.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ readdirp@npm:2.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ readdirp@npm:3.6.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ regenerate-unicode-properties@npm:8.2.0 can't be found in the cache and will be fetched from the remote reg
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ regenerate@npm:1.4.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ regenerator-runtime@npm:0.13.9 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ regenerator-transform@npm:0.14.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ regex-not@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ regexpu-core@npm:4.7.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ regjsgen@npm:0.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ regjsparser@npm:0.6.9 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ reinterval@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ relateurl@npm:0.2.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ remove-trailing-separator@npm:1.1.0 can't be found in the cache and will be fetched from the remote registr
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ renderkid@npm:2.0.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ repeat-element@npm:1.1.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ repeat-string@npm:1.6.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ resolve-from@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ resolve-url@npm:0.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ resolve@npm:1.20.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ resolve@patch:resolve@npm%3A1.20.0#~builtin<compat/resolve>::version=1.20.0&hash=00b1ff can't be found in t
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ restore-cursor@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ret@npm:0.1.15 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ retry@npm:0.12.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ reusify@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ rgb-regex@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ rgba-regex@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ rimraf@npm:2.7.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ rimraf@npm:3.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ripemd160@npm:2.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ run-async@npm:2.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ run-parallel@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ run-queue@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ rxjs@npm:6.6.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ safe-buffer@npm:5.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ safe-buffer@npm:5.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ safe-regex@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ safer-buffer@npm:2.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ sax@npm:1.2.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ schema-utils@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ schema-utils@npm:2.7.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ schema-utils@npm:3.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ scule@npm:0.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ select@npm:1.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ semver@npm:5.7.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ semver@npm:6.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ semver@npm:7.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ semver@npm:7.3.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ send@npm:0.17.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ serialize-javascript@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0013: │ serialize-javascript@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ serialize-javascript@npm:5.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ serve-placeholder@npm:1.2.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ serve-static@npm:1.14.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ server-destroy@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ set-value@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ setimmediate@npm:1.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ setprototypeof@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ sha.js@npm:2.4.11 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ shebang-command@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ shebang-regex@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ shell-quote@npm:1.7.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ side-channel@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ signal-exit@npm:3.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ signal-exit@npm:4.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ simple-swizzle@npm:0.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ sirv@npm:1.0.14 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ slash@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ smart-buffer@npm:4.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ snapdragon-node@npm:2.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ snapdragon-util@npm:3.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ snapdragon@npm:0.8.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ socks-proxy-agent@npm:8.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ socks@npm:2.7.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ sort-keys@npm:1.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ sort-keys@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ source-list-map@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ source-map-resolve@npm:0.5.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ source-map-support@npm:0.5.19 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ source-map-url@npm:0.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ source-map@npm:0.5.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ source-map@npm:0.5.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ source-map@npm:0.6.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ source-map@npm:0.7.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ split-on-first@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ split-string@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ split2@npm:3.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ sprintf-js@npm:1.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ssri@npm:10.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ssri@npm:6.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ssri@npm:8.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ stable@npm:0.1.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ stack-trace@npm:0.0.10 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ stackframe@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ static-extend@npm:0.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ statuses@npm:1.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ std-env@npm:2.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ stream-browserify@npm:2.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ stream-each@npm:1.2.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ stream-http@npm:2.8.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ stream-shift@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ strict-uri-encode@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ strict-uri-encode@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ string-width@npm:2.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ string-width@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ string-width@npm:4.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ string-width@npm:5.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ string.prototype.trimend@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ string.prototype.trimstart@npm:1.0.4 can't be found in the cache and will be fetched from the remote regist
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ string_decoder@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ string_decoder@npm:1.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ strip-ansi@npm:3.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ strip-ansi@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ strip-ansi@npm:5.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ strip-ansi@npm:6.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ strip-ansi@npm:6.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ strip-ansi@npm:7.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ strip-final-newline@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ style-resources-loader@npm:1.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ stylehacks@npm:4.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ supports-color@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ supports-color@npm:5.5.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ supports-color@npm:6.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ supports-color@npm:7.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ svg-tags@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ svgo@npm:1.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ tapable@npm:1.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ tar@npm:6.1.10 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ tar@npm:6.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ terser-webpack-plugin@npm:1.4.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ terser-webpack-plugin@npm:4.2.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ terser@npm:4.8.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ terser@npm:5.7.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ text-table@npm:0.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ thread-loader@npm:3.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ through2@npm:2.0.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ through@npm:2.3.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ time-fix-plugin@npm:2.0.7 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ timers-browserify@npm:2.0.12 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ timsort@npm:0.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ tiny-emitter@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ tmp@npm:0.0.33 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ to-arraybuffer@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ to-fast-properties@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ to-object-path@npm:0.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ to-regex-range@npm:2.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ to-regex-range@npm:5.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ to-regex@npm:3.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ toidentifier@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ totalist@npm:1.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ts-pnp@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ tslib@npm:1.14.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ tslib@npm:2.3.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ tty-browserify@npm:0.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ type-fest@npm:0.20.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ type-fest@npm:0.21.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ typedarray@npm:0.0.6 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ua-parser-js@npm:0.7.28 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ufo@npm:0.7.9 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ uglify-js@npm:3.14.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unbox-primitive@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unfetch@npm:4.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unicode-canonical-property-names-ecmascript@npm:1.0.4 can't be found in the cache and will be fetched from
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unicode-match-property-ecmascript@npm:1.0.4 can't be found in the cache and will be fetched from the remote
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unicode-match-property-value-ecmascript@npm:1.2.0 can't be found in the cache and will be fetched from the
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unicode-property-aliases-ecmascript@npm:1.1.0 can't be found in the cache and will be fetched from the remo
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ union-value@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ uniq@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ uniqs@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unique-filename@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unique-filename@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unique-slug@npm:2.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unique-slug@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ universalify@npm:0.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ universalify@npm:2.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unpipe@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unquote@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ unset-value@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ upath@npm:1.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ upath@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ upper-case@npm:1.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ uri-js@npm:4.4.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ urix@npm:0.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ url-loader@npm:4.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ url@npm:0.11.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ use@npm:3.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ util-deprecate@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ util.promisify@npm:1.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ util.promisify@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ util@npm:0.10.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ util@npm:0.11.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ utila@npm:0.4.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ utils-merge@npm:1.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ uuid@npm:8.3.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vary@npm:1.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vendors@npm:1.0.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vm-browserify@npm:1.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-client-only@npm:2.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-clipboard2@npm:0.2.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-clipboard2@npm:0.3.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-functional-data-merge@npm:3.1.0 can't be found in the cache and will be fetched from the remote registr
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-hot-reload-api@npm:2.3.4 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-loader@npm:15.9.8 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-meta@npm:2.4.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-no-ssr@npm:1.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-router@npm:3.5.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-server-renderer@npm:2.6.14 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-style-loader@npm:4.1.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-template-compiler@npm:2.6.14 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue-template-es2015-compiler@npm:1.9.1 can't be found in the cache and will be fetched from the remote regi
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vue@npm:2.6.14 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ vuex@npm:3.6.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ watchpack-chokidar2@npm:2.0.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ watchpack@npm:1.7.5 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ webpack-bundle-analyzer@npm:4.4.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ webpack-dev-middleware@npm:4.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ webpack-hot-middleware@npm:2.25.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ webpack-node-externals@npm:3.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ webpack-sources@npm:1.4.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ webpack@npm:4.46.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ webpackbar@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ which-boxed-primitive@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ which@npm:2.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ which@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ widest-line@npm:3.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ worker-farm@npm:1.7.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ wrap-ansi@npm:6.2.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ wrap-ansi@npm:7.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ wrap-ansi@npm:8.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ wrappy@npm:1.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ write-file-atomic@npm:2.4.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ write-json-file@npm:2.3.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ ws@npm:7.5.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ xtend@npm:4.0.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ xxhashjs@npm:0.2.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ y18n@npm:4.0.3 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ yallist@npm:2.1.2 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ yallist@npm:3.1.1 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ yallist@npm:4.0.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0013: │ yocto-queue@npm:0.1.0 can't be found in the cache and will be fetched from the remote registry
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0001: │ Error [ERR_STREAM_PREMATURE_CLOSE]: Premature close
    at PassThrough.onclose (node:internal/streams/end-of-stream:154:30)
    at PassThrough.emit (node:events:519:28)
    at emitCloseNT (node:internal/streams/destroy:147:10)
    at process.processTicksAndRejections (node:internal/process/task_queues:81:21)
➤ YN0000: └ Completed in 10s 88ms
➤ YN0000: Failed with errors in 16s 804ms
```

Does anyone have an idea here?