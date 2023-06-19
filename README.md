# Adding GitHub based codeblocks

```bash
npx create-docusaurus@2.4.1 testDriven classic
cd testDriven
```

```bash
yarn add @saucelabs/theme-github-codeblock
```

## Modify `themes`

Edit `docusaurus-config.json`.  If you do not have any existing `themes`, add a themes section just above `presets`

```json
  themes: ['@saucelabs/theme-github-codeblock'],
```

```bash
yarn build
```

# Website

This website is built using [Docusaurus 2](https://docusaurus.io/), a modern static website generator.

### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```
$ USE_SSH=true yarn deploy
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
