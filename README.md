# frontline-sass-snippets

[Frontline Sass](https://github.com/Threespot/frontline-sass) snippets for [Atom](https://atom.io/) and [VS Code](https://code.visualstudio.com/).

## Install

### Atom

```shell
apm install frontline-sass-snippets
```

https://atom.io/packages/frontline-sass-snippets

### VS Code

```shell
code --install-extension threespot.frontline-sass-snippets
```

https://marketplace.visualstudio.com/items?itemName=Threespot.frontline-sass-snippets

## Snippets

Snippets for the main variables, functions and mixins, as well as the selector mixins.

See [documentation](http://threespot.github.io/frontline-sass/documentation/) for a comprehensive list.

## Publishing Updates

VS Code snippets are generated using the [`convert-atom-snippets-to-vscode`](https://github.com/binaryoung/convert-atom-snippets-to-vscode) module. Any added snippet files will also need to be added to the `package.json` `contributes.snippets` key.

```
node node_modules/convert-atom-snippets-to-vscode/src/command.js snippets/ vs-snippets/
```

### Create a new version using npm

```
npm version patch
```

### Publish to atom

```
apm publish --tag v1.0.1
```

### Publish to VS Marketplace

```
vsce publish v1.0.1
```

### Push release to Github

```
git push --tags
```
