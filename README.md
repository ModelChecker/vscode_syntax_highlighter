VS Code can only load json grammars, so yaml based grammars must be converted to json. The js-yaml package and command-line tool makes this easy.

# Install js-yaml as a development only dependency in your extension
$ npm install js-yaml --save-dev

# Use the command-line tool to convert the yaml grammar to json
$ npx js-yaml syntaxes/mcil.tmLanguage.yaml > syntaxes/mcil.tmLanguage.json

# Build and publish with vsce
https://codevsce package.visualstudio.com/api/working-with-extensions/publishing-extension

# Install extension from vsix
https://code.visualstudio.com/docs/editor/extension-marketplace#_install-from-a-vsix