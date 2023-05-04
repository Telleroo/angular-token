# Notice

Original [README](https://github.com/neroniaky/angular-token).

We needed to fork this repository as it is not being maintained anymore (according to its [npm](https://www.npmjs.com/package/angular-token) page).

To make it installable trough `npm i` we needed to add add some additional steps:

## Build

```sh
npm run build:package
```

This will do a clean package build to the `./dist/angular-token` folder.

## Publish

We are using [Github Packages](https://docs.github.com/en/packages) to host this package. The repository is associated with the Telleroo organization, and can only be used with an authentication token.

### Prerequisites

- [Create a Github token with the required permissions](https://docs.github.com/en/packages/learn-github-packages/about-permissions-for-github-packages#about-scopes-and-permissions-for-package-registries).
- Set the token as an environment variable called `GITHUB_TOKEN`.

### Publishing

```sh
cd ./dist/angular-token
npm publish
```