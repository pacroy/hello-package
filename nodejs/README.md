# hello

This is a hello world demo Node.js package.

## Build & Publish

1. Install [Node version manager (nvm)](https://github.com/nvm-sh/nvm#installing-and-updating).
2. Install the latest LTS version of Node.js and npm.

   ```sh
   nvm install --lts --default --latest-npm
   nvm ls
   nvm use 18
   ```

3. Install and configure [npmrc](https://www.npmjs.com/package/npmrc).

   ```sh
   npm install --global npmrc
   npmrc
   npmrc -c new_profile_name
   ```

4. Configure npm registry.

   **Automatic**
   
   ```sh
   npm login --registry=https://registry.npmjs.org --scope=@your_username
   ```

   **Manual**

   Create an [access token](https://www.npmjs.com/settings/pacroy/tokens) and then use commands:

   ```sh
   npm config set @your_username:registry https://registry.npmjs.org/
   npm config set //registry.npmjs.org/:_authToken your_access_token
   npm whomai
   ```

5. Publish the package.

   ```sh
   npm publish --access public
   ```

### Troubleshooting

- When logging in npm registry using automatic method, if you get an error message `xdg-open: not found` then try to install it using command `sudo apt install xdg-utils` first.
- When publishing the package, if you get `403 Forbidden` with error message `You cannot publish over the previously published versions` then you need to bump up the package version first. You can use command `npm version patch|minor|major` or manually update the *package.json* file.
- If you unpublished a package versiom, you wouldn't be able to publish it again witin 24 hours even with `--force` flag.

## Install

```sh
npm install @pacroy/hello
```

## Usage

```js
const hello = require("@pacroy/hello")
hello()
```

## Test

```sh
cd test
node test.js
```

## References

- [Creating Node.js modules | npm Docs](https://docs.npmjs.com/creating-node-js-modules)
- [Downloading and installing Node.js and npm | npm Docs](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [Unpublishing packages from the registry | npm Docs](https://docs.npmjs.com/unpublishing-packages-from-the-registry)
