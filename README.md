[![](https://ptkdev.it/img/github/eslintplugin_snakecasejs.png)](https://www.npmjs.com/package/eslint-plugin-snakecasejs)

# ESLint Plugin snakecasejs

[![](https://img.shields.io/badge/license-MIT-brightgreen.svg)](#) [![](https://img.shields.io/badge/powered%20by-eslint-46aef7.svg)](https://www.npmjs.com/package/eslint) [![](https://img.shields.io/badge/version-v1.2.1-lightgrey.svg)](https://github.com/ptkdev/eslint-plugin-snakecasejs/releases) [![](https://img.shields.io/badge/chat%20on-slack-orange.svg)](http://slack.ptkdev.io) [![](https://img.shields.io/badge/chat%20on-discord-7289da.svg)](http://discord.ptkdev.io) [![](https://img.shields.io/badge/blog-medium-2AE176.svg)](http://blog.ptkdev.io) [![](https://img.shields.io/badge/twitter-ptkdevio-2AA3EF.svg)](https://twitter.com/ptkdevio)

[![](https://img.shields.io/badge/donate-patreon-F87668.svg)](http://patreon.ptkdev.io) [![](https://img.shields.io/badge/donate-paypal-46AFE0.svg)](http://paypal.ptkdev.io) [![](https://img.shields.io/badge/buy%20me-coffee-4B788C.svg)](http://coffee.ptkdev.io) [![](https://img.shields.io/badge/help-support@ptkdev.io-fbbc05.svg)](mailto:support@ptkdev.io)

## What does it do
This is to enforce a style of snake_case in your project, rather than just disabling camelCase.

## Features
* [✓] Easy to use
* [✓] MIT License
* [✓] Compatible with latest version of ESLint
* [✓] Compatible with CamelCase (Class name or similar)
* [✓] Compatible with --fix (convert automatically camelCase to snake_case)
* [✓] White list array for methods or variables with camelCase syntax from other libraries/npm package.

## Fast setup
1. Install eslint: `npm install eslint --save-dev`
2. Install snakecasejs plugin: `npm install eslint-plugin-snakecasejs --save-dev`
3. Create `.eslintrc.json` file with:
```
{
    "plugins": [
        "snakecasejs"
    ],
    "rules":
    {
        "snakecasejs/snakecasejs": "error",
        "snakecasejs/whitelist": []
    }
}
```
4. If it works add a star :star: at this project :heart:
5. If you want to help me: **[donate on paypal](http://paypal.ptkdev.io)** or become a **[backer on patreon](http://patreon.ptkdev.io)**.

NOTE: switch `error` to `warn` if you don't need snake_case as mandatory rules.

For advanced configuration see [INSTALL.md](https://github.com/ptkdev/eslint-plugin-snakecasejs/blob/master/INSTALL.md).

## --fix
This eslint parameter fix simple rules of linter and with this plugin convert all camelCase variables or function name to snake_case. 
Fix command support whitelist. Run this command in your project directory:
- `eslint ./ --cache --ignore-pattern .gitignore --fix`

**WARNING:** You need install eslint globally for this feature: `npm install eslint -g`

## White list
Ignore words, variables, methods, class name without snake_case syntax. Add rules: `"snakecasejs/whitelist": []` with array of variables or method with camelCase that you can not convert to snake_case (external library naming convention). 

Plugin ignore check on this words. Example: `"snakecasejs/whitelist": ["externalPath","setNumber"]`

# License

MIT LICENSE

Copyright (c) 2018 Patryk Rzucidło (PTKDev)
