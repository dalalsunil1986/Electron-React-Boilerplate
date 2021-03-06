# [Deprecated]~~Electron-React-Boilerplate~~

No longer maintained.

![](./docs/screenshot.png)
# How to develop
1. `npm i`
2. `npm start`
3. open application in build directory
4. add some react components and styles
5. reload application (⌘+R)

# Electron api calling
To call Electron's api, it is necessary to use window.require because, browserify rewrites require statement.

ex) `var remote = window.require( 'remote' );`

## Refactoring

Run `npm run refactor` to refactor the code in accordance to [jscs preset](http://jscs.info/overview#presets) specified in the `.jscsrc` file.

## Linting

Run `npm run lint` to run a linter through the codebase. The linter will check
the codebase as specified in the [configuration file named `.eslintrc`](http://eslint.org/docs/user-guide/configuring). Fix all reported
errors prior to committing code.

An example of a `.eslintrc` follows:

```json
{
  "ecmaFeatures": {
    "blockBindings": true,
    "jsx": true
  },
  "rules": {
    "semi": 2
  }
}
```
