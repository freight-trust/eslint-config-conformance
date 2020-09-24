# eslint-conformance

> npm --save-dev eslint-conformance

[npm registry](https://www.npmjs.com/package/eslint-conformance)

## Overview 

` npx install-peerdeps --dev eslint-conformance `

You can see in your package.json there are now a big list of '`devDependencies`'.


Create a .eslintrc file in the root of your project's directory (it should live where package.json does). Your .eslintrc file should look like this:

```json
{
  "extends": [
    "conformance"
  ]
}
```

Tip: You can alternatively put this object in your package.json under the property "eslintConfig":. This makes one less file in your project.

You can add two scripts to your package.json to lint and/or fix:

```json
"scripts": {
  "lint": "eslint .",
  "lint:fix": "eslint . --fix"
},
```

Now you can manually lint your code by running npm run lint and fix all fixable issues with npm run lint:fix. 


### With Create React App

Run `npx install-peerdeps --dev eslint-conformance`

Replace "extends": "react-app" with "extends": "conformance"

### With Gatsby

Run npx install-peerdeps --dev eslint-conformance
If you have an existing .prettierrc file, delete it.
follow the Local / Per Project Install steps above

## License 

ISC 
