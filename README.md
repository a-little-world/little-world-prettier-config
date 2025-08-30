# little-world-prettier-config

Shared [Prettier](https://prettier.io/) config to be used across applicable Little World repos.

Prettier has language support for JavaScript, JSX, Angular, Vue, Flow, TypeScript, CSS, HTML, JSON, GraphQL, Markdown and YAML.

To update, add or remove [options](https://prettier.io/docs/en/options.html), edit the `index.json` file.

## Using the config

To use this shared prettier config in a repository, first install the config: ` npm install --save-dev @a-little-world/little-world-prettier-config`.

Then add the prettier property to your `package.json`:

```
{
  "name": "little-world-repo",
  // ...
  "prettier": "@a-little-world/little-world-prettier-config"
  // ...
}

```

Then to make it play nicely with eslint, you need to ensure the following is set in your eslint config (in the consumer repository)

```
  extends: [
    'prettier',
  ],
  plugins: ['prettier'], // make sure its at the end of list
```

## Publish updates

Whenever the share config is updated, the version must be bumped and that new version must be published via npm.

Bump the version number by editing the `version` in `package.json`

To publish run the following command in your terminal when at the root of the cloned repo:
`npm publish`
