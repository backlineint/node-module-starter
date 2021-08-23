# Node Module Starter

My preferred setup and tooling for a new Node JS module

## Contributing

### Prerequisites

Steps below assume that you have [NodeJS](https://nodejs.org/) installed. We
recommend using [NVM](https://github.com/nvm-sh/nvm) to manage the NodeJS
version on your local system.

In order to prepare your system for contribution you'll need to complete this
checklist:

1. Run `nvm use` to switch to the expected version of npm. Run `nvm install` if
   you need to update your npm.
2. Run `npm i` to install dependencies.

### Formatting and Linting

VSCode users can format code on save using the
[Eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
and
[Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
extensions. These extensions will be suggested when loading the project if they
have not already been installed. An example settings file is included in
`.vscode/example.settings.json`. Save this file as `.vscode/settings.json` or
incorporate the contents into your existing settings.json file to enable format
on save in your project.

Formatting on save is highly recommended as it should resolve most formatting
issues before the pre-commit hook runs.

Formatting and linting can also be run manually using the following commands:

- `npm run eslint` - checks linting
- `npm run eslint:fix` - attempts to fix any linting issues
- `npm run prettier` - checks formatting
- `npm run prettier:fix` - attempts to fix any formatting issues

## Testing

This project is configured to run [Jest](https://facebook.github.io/jest/) tests
via `npm run test`. All new code is expected to be covered by tests and these
tests will run as part of our CI process.

Tests should be added in a `__tests__` directory adjacent to the file they are
testing and the files should be named `<fileName>.test.ts`.

## Documentation

Documentation is provided by [TypeDoc](https://typedoc.org/).

To generate documentation run `npm run typedoc` The result will be in the `docs`
folder.
