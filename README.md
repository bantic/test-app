# Test-app

This app demonstrates usage of ember-cli with a `node_modules`
directory somewhere other than in the project's root.

## Installation

  * `git clone https://github.com/bantic/test-app.git`
  * `cd test-app`
  * `npm install`
  * `mv node_modules ../some/other/directory`
  * `export NODE_PATH=/abs/path/to/some/other/directory/node_modules`
  * `export EMBER_NODE_PATH=/abs/path/to/some/other/directory/node_modules`
  * (in some other directory) clone
    https://github.com/jakehow/ember-cli/tree/node-module-path-support,
and `npm link` it
  * ensure your `ember` command-line tool is the one linked from the repo on the previous step
  * `ember serve`
