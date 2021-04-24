Here are some of the common errors you may experience with the plugin and how to resolve.

## Installation/Update Warnings

When installing or updating the plugin, you may see entries like this:

```bash
npm WARN deprecated node-xmpp-client@3.2.0: this package is deprecated please use https://www.npmjs.com/package/@xmpp/client
npm WARN deprecated node-pre-gyp@0.15.0: Please upgrade to @mapbox/node-pre-gyp: the non-scoped node-pre-gyp package is deprecated and only the @mapbox scoped package will recieve updates in the future
npm WARN deprecated node-xmpp-core@5.0.9: this package is deprecated please use https://github.com/xmppjs/xmpp.js
npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
npm WARN deprecated node-xmpp-tls-connect@1.0.1: this package is deprecated please use https://github.com/xmppjs/xmpp.js
npm WARN deprecated har-validator@5.1.5: this library is no longer supported
```

or warnings about `canvas`:

```bash
node-pre-gyp ERR! command "/usr/local/bin/node" "/home/pi/deebot/node_modules/.bin/node-pre-gyp" "install" "--fallback-to-build"
node-pre-gyp ERR! cwd /home/pi/deebot/node_modules/canvas
node-pre-gyp ERR! node -v v14.16.1
node-pre-gyp ERR! node-pre-gyp -v v0.15.0
node-pre-gyp ERR! not ok 
Failed to execute '/usr/local/bin/node /usr/local/lib/node_modules/npm/node_modules/node-gyp/bin/node-gyp.js configure --fallback-to-build --module=/home/pi/deebot/node_modules/canvas/build/Release/canvas.node --module_name=canvas --module_path=/home/pi/deebot/node_modules/canvas/build/Release --napi_version=7 --node_abi_napi=napi --napi_build_version=0 --node_napi_label=node-v83' (1)
npm notice created a lockfile as package-lock.json. You should commit this file.
npm WARN optional SKIPPING OPTIONAL DEPENDENCY: canvas@2.7.0 (node_modules/canvas):
npm WARN optional SKIPPING OPTIONAL DEPENDENCY: canvas@2.7.0 install: `node-pre-gyp install --fallback-to-build`
npm WARN optional SKIPPING OPTIONAL DEPENDENCY: Exit status 1
```

All of these messages can be safely ignored since the plugin will still install and function correctly.