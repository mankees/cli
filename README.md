# mankees - mankee see, mankee do

`mankees` is a simple terminal tool which allows you to execute custom scripts stashed at your `~/.mankees/` quickly. This makes it ideal for implementing quick utilities using Node.js.

## Usage

Install the utility via NPM globally (ie. `npm install mankees -g`). `mankees -s` to see mankees available online. `mankees -i somename` to install one. After that you can simply invoke `mankees somename` or `mankees -h somename` to see help included.

## Authoring

`mankees` uses NPM as its plugin registry. Simply publish your plugin there. In order to make it discoverable, perform the following steps:

1. Add `mankees` keyword to `package.json` keywords (ie. `keywords: ["mankees"]`)
2. Prefix the plugin with word `mankees-`. This is a convention that allows us avoid polluting NPM too much. The actual plugin name will be the remainder (ie. for `mankees-init` it is `init`).

## License

mankees is available under MIT. See LICENSE for more details.

