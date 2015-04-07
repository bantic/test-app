# Test-app

This app demonstrates usage of ember-cli with a `node_modules`
directory somewhere other than in the project's root.

## Installation

  * clone this
  * `cd test-app`
  * `npm install`
  * `mv node_modules ../some/other/directory`
  * `export NODE_PATH=/abs/path/to/some/other/directory/node_modules`
    (so node's `require` works for modules installed in your
node_modules, wherever they are)
  * `export EMBER_NODE_PATH=/abs/path/to/some/other/directory/node_modules` (so ember's addon discovery works for addons in your node_modules)
  * (`export`-ing relative paths will also work)
  * in some other directory: clone
    https://github.com/jakehow/ember-cli/tree/node-module-path-support,
and `npm link` it
  * (back in test-app) `npm link ember-cli`
  * `ember serve`
