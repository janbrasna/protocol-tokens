# Protocol Tokens

Design tokens for Protocol, Mozilla’s design system.     _JavaScript · JSON · CSS · SCSS_

[![Current npm package version.](https://img.shields.io/npm/v/@mozilla-protocol/tokens)](https://www.npmjs.com/package/@mozilla-protocol/tokens)

[ᴄʜᴀɴɢᴇʟᴏɢ](https://github.com/mozilla/protocol-tokens/blob/main/CHANGELOG.md)

---

## Installation

Protocol design tokens are available as [`@mozilla-protocol/tokens`](https://www.npmjs.com/package/@mozilla-protocol/tokens) npm package.

The recommended way to use and install design tokens may vary depending on your project; the most common are documented below.

### JavaScript package installation

Using [npm](https://www.npmjs.com/):

```
npm install @mozilla-protocol/tokens --save
```

Using [yarn](https://yarnpkg.com/en/):

```
yarn add @mozilla-protocol/tokens
```

### JavaScript

In JavaScript, design token names are formatted in [lower camelCase](http://wiki.c2.com/?CamelCase).

```js
const tokens = require('@mozilla-protocol/tokens/dist/index');
console.log(tokens.colorBlueLighter); // rgb(0, 0, 0)
```

In JSON, design token names are formatted in [kebab-case](http://wiki.c2.com/?KebabCase).

```js
const tokens = require('@mozilla-protocol/tokens/dist/index.json');
console.log(tokens['color-black']); // rgb(0, 0, 0)
```

### Sass

Sass variables and map keys are formatted in [kebab-case](http://wiki.c2.com/?KebabCase).

```scss
// Using variables
@import '~@mozilla-protocol/tokens/dist/index';

a {
  color: $color-black;
}
```

### Sass, with CSS Custom Properties

Custom properties are formatted in [kebab-case](http://wiki.c2.com/?KebabCase).

```scss
// Omit .css at the end of the file
@import '~@mozilla-protocol/tokens/dist/colors/colors.custom-properties';

a {
  color: var(--color-black);
}
```

## Publishing

To publish to the npmjs registry you'll need access to the mozilla-protocol org on npmjs.com.
First run `gulp` to compile the package locally. You can check your local `dist`
folder to verify it has the up-to-date tokens. Then run `npm publish`.


## Contributing

### [Code of conduct](https://www.mozilla.org/en-US/about/governance/policies/participation/)

We have a [code of conduct](https://www.mozilla.org/en-US/about/governance/policies/participation/),
please follow it in all your interactions with the project.

### [Contributing guide](https://github.com/mozilla/protocol-tokens/blob/master/CONTRIBUTING.md)

Read the [contributing guide](https://github.com/mozilla/protocol-tokens/blob/master/CONTRIBUTING.md)
to learn how to propose changes and understand our development process.

### [License](https://github.com/mozilla/protocol-tokens/blob/master/LICENSE.md)

The protocol-tokens project is available under the [MPL-2.0](https://github.com/mozilla/protocol-tokens/blob/master/LICENSE.md).
