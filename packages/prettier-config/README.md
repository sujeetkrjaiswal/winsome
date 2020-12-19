# Winsome Prettier Config

Opinionated Sharable Prettier Config

## Installation

```shell
npm install --save-dev prettier @winsome/prettier-config
```

## Usage

### Adding in your `package.json`

```json
{
  "prettier": "@winsome/prettier-config"
}
```

### Using in .prettierrc

```
"@winsome/prettier-config"
```

## Extending

This configuration is not intended to be changed, but if you have a setup where modification is required, it is possible. Prettier does not offer an "extends" mechanism as you might be familiar from tools such as ESLint.

To extend a configuration you will need to use a `prettier.config.js` or `.prettierrc.js` file that exports an object:

```js
module.exports = {
  ...require("@winsome/prettier-config"),
  semi: false,
}