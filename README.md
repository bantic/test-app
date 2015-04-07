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


These are the changes that were made to package.json to get this to work:
https://github.com/bantic/test-app/compare/ad175b3cae5a49d4231caab787000e509da045b4...89d3f6cecb1597ca9fae5e137c8ef549b82d6382
