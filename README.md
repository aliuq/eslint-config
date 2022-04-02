# @aliuq/eslint-config

## Thanks

Used Antfu's [@antfu/eslint-config-basic](https://github.com/antfu/eslint-config/tree/master/packages/basic) and referenced from his structure, but modified to fit my needs.

see more at [@antfu/eslint-config](https://github.com/antfu/eslint-config)

## Usage

### Install

```bash
pnpm add -D eslint @aliuq/eslint-config
```

### Config `.eslintrc`

```json
{
  "extends": "@aliuq"
}
```

> You don't need `.eslintignore` normally as it has been provided by the preset.

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint ."
  }
}
```

### Config VS Code auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## License

MIT
