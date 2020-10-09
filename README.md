Base CRA Template optimized for a DomoApp.
- The manifest and thumbnail are provided in the `public` folder.
- The proxy server is setup with `@domoinc/ryuu-proxy` for local development to your domo instance.
- An upload script has been added to the package.json for easy upload.

Steps to get going
1) Use the domoapps cli to login to your Domo instance `domo login`
2) Upload your base app to your Domo instance using `yarn upload` or `npm run upload`
3) The project will build, add all assets to the `build` folder, and then upload the assets to Domo
4) The `manifest.json` file in the `build` folder will be modified by the domoapps cli to include an `id` property. You will want to copy this `id` into the manifest in your `public` folder so that it doesn't continue to create a new `id` on each upload
5) If you intend to use AppDB, make sure to also add a `proxyId` to the `manifest.json` file in your `public` folder. See [documentation](https://developer.domo.com/docs/dev-studio/step4#Set%20Up%20Your%20Proxy) for more info.

# cra-template

This is the official base template for [Create React App](https://github.com/facebook/create-react-app).

If you don't specify a template (for example, `--template typescript`), this template will be used by default.

For more information, please refer to:

- [Getting Started](https://create-react-app.dev/docs/getting-started) – How to create a new app.
- [User Guide](https://create-react-app.dev) – How to develop apps bootstrapped with Create React App.
