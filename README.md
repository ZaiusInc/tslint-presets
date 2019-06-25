# Zaius TSLint Presets
This NPM package includes Zaius's preferred [TSLint](https://palantir.github.io/tslint/) rules for Node and React projects.

## Installation
Install the package as a dev dependency using yarn or npm.
```bash
# yarn:
yarn add -D zaius-tslint

# npm:
npm install -D zaius-tslint
```

## Usage
After adding the package to your project, create or update your `tslint.json` file in the root of your project and extend the desired preset. For Node projects:

```json
{
  "extends": "zaius-tslint/node.json",
  "rules": {}
}
```

and for React projects:

```json
{
  "extends": "zaius-tslint/react.json",
  "rules": {}
}
```

## Best Practices and Overrides
Certain projects may need overrides to the presets. Overrides or additional rules can be added to the `rules` object.

Please try to minimize overrides! For one-off situtations you can ignore a single line with:
```typescript
// tslint:disable-next-line:rule-name
```

Start a discussion if you believe a change should be made to the preset for all projects.
