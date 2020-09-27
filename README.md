# eslint-conformance

> @eslint-conformance

[npm registry](https://www.npmjs.com/package/eslint-conformance)

## Overview

## Install

`npx install-peerdeps --dev --exact eslint-conformance`

Install will taken place in '`devDependencies`'.

For Installing without `npx` please see the section [Alternative Install](# altnerative install without npx)

Create a .eslintrc file in the root of your project's directory (it should live where package.json does). Your .eslintrc file should look like this

```json
{
  "extends": ["conformance"]
}
```

### End User Notes

- You can alternatively put this object in your package.json under the property "eslintConfig":
- When installing linting tools you should always do `--exact`, for example `yarn add --dev --exact prettier` should be the install

You can add two scripts to your package.json to lint and/or fix:

```json
"scripts": {
  "lint": "eslint .",
  "lint:fix": "eslint . --fix"
}
```

Now you can manually lint your code by running npm run lint and fix all fixable issues with npm run lint:fix.

### Create React App

Run `$ npx install-peerdeps --dev eslint-conformance`

Replace "extends": "react-app" with "extends": "conformance"

### With Gatsby

Run `$ npx install-peerdeps --dev eslint-conformance`

## Alternative Install without `npx`

If you can not use `npx` (this invokes a seperate package, `install-peerdeps` you can use the following command for example:
` npm info "$PKG@latest" peerDependencies --json | command sed 's/[\{\},]//g ; s/: /@/g' | xargs npm install --save-dev "$PKG@latest"`

You can also manually add the `peerDependencies`, here is the dependencies as of `v1.0.0`

```json
{
  "babel-eslint": "^10.1.0",
  "eslint": "^7.8.1",
  "eslint-config-airbnb": "^18.2.0",
  "eslint-config-prettier": "^6.11.0",
  "eslint-plugin-html": "^6.1.0",
  "eslint-plugin-import": "^2.22.0",
  "eslint-plugin-jsx-a11y": "^6.3.1",
  "eslint-plugin-prettier": "^3.1.4",
  "eslint-plugin-react": "^7.20.6",
  "eslint-plugin-react-hooks": "^4.1.2",
  "prettier": "^2.1.1"
}
```

## License

ISC
