# strapi-provider-upload-rackspace

## Configurations

Your configuration is passed down to the client initialization. (e.g: `createClient(config)`). The implementation is based on the package `pkgcloud`. You can read the docs [here](https://github.com/pkgcloud/pkgcloud#storage).

See the [using a provider](https://strapi.io/documentation/developer-docs/latest/plugins/upload.html#using-a-provider) documentation for information on installing and using a provider. And see the [environment variables](https://strapi.io/documentation/developer-docs/latest/concepts/configurations.html#environment-variables) for setting and using environment variables in your configs.

**Example**

`./config/plugins.js`

```js
module.exports = ({ env }) => ({
  // ...
  upload: {
    provider: 'rackspace',
    providerOptions: {
      username: env('RACKSPACE_USERNAME'),
      apiKey: env('RACKSPACE_KEY'),
      region: env('RACKSPACE_REGION'),
      container: env('RACKSPACE_CONTAINER'),
    },
  },
  // ...
});
```

## Resources

- [License](LICENSE)

## Links

- [Strapi website](https://strapi.io/)
- [Strapi community on Slack](https://slack.strapi.io)
- [Strapi news on Twitter](https://twitter.com/strapijs)
