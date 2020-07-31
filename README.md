# Next.js Issue with Webpack 5 and JSConfig

The repo reproduces an issue with Next.js and Webpack 5 inside of a monorepo.

To see the error run the following commands

```shell
# Install / link dependencies
yarn

# Navigate to the Next.js app
cd packages/next-app

# Run the application
yarn dev
```

The following error will appear in the terminal:

`Module not found: Your application tried to access components, but it isn't declared in your dependencies; this makes the require call ambiguous and unsound.`

`components` is a folder at the root of the next-app package and should get resolved by the `jsconfig.json`.