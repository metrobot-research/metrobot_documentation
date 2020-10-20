# metrobot_documentation

[![Generic badge](static/img/powered-by-vercel.svg)](https://vercel.com?utm_source=metrobot-research&utm_campaign=oss)

Documentation for the Metrobot project. This website is built using [Docusaurus 2](https://v2.docusaurus.io/). 

### Updating Documentation
Add/update markdown (`.md`) files in the `docs` folder. Be sure to add:

```markdown
---
id: <Page ID>
title: <Page Title>
---
```

Update `sidebars.js` to include the new `id`:

```js
module.exports = {
  sidebar: {
    General: ['overview', 'devdocs', 'your-new-id'], // General header with two pages w/ id overview and devdocs
  },
};

```

### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

This command starts a local development server and open up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

```
$ GIT_USER=<Your GitHub username> USE_SSH=true yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
