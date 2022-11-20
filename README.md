# little-world-prettier-config
Shared [Prettier](https://prettier.io/) config to be used across applicable Little World repos.

Prettier has language support for JavaScript, JSX, Angular, Vue, Flow, TypeScript, CSS, HTML, JSON, GraphQL, Markdown and YAML.

To update, add or remove [options](https://prettier.io/docs/en/options.html), edit the `index.json` file.

## Using the config

To use this shared prettier config in a repository, add the prettier property to your `package.json`:

```
{
  "name": "little-world-repo",
  // ...
  "prettier": "a-little-world/little-world-prettier-config"
  // ...
}

```

## Publish updates

Whenever the share config is updated, the version must be bumped and that new version must be published via npm.

Bump the version number by editing the `version` in `package.json`

To publish run the following command in your terminal when at the root of the cloned repo:
`npm publish`