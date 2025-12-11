An overview/list of all the useful links and tech tools used at the _organization of De Sering_.

Using [homer](https://github.com/bastienwirtz/homer).
Hosted using GitHub Pages at start.desering.org.

## Contribution
Edit `config.yml` and `customizations.css`.

> You can even edit them in your browser to see the result imediately!
> Open https://start.desering.org, open DevTools, locate `config.yml`, edit and enable "Local Overrides". Then, you can refresh the  page, but your local copy will be used. Then you can copy these additions here.

## Deployment
To be as simple as possible we run homer using GitHub Pages, since it's static. The instance is created and configured using GitHub Actions.
This happens on every push commit to main (merged PR).

## Custom favicon
Homer project seems to not support custom favicon by default.

As sugested in [Homer docs subpage](https://github.com/bastienwirtz/homer/blob/main/public/assets/icons/README.md) let's use [RealFaviconGenerator](https://realfavicongenerator.net/) for generating a favicon bundle:

The setings are already in `favicon-settings.json` and the deployment step generates a favicon bundle based on an icon from the `media` repository (see GitHub Actions file).

You can check whether the deployed favicon bundle is correct with
`$ npx realfavicon check https://start.desering.org`

## Local GitHub Action runner
To test locally you can run an the build action with:
`$ act -j build -P ubuntu-latest=ghcr.io/catthehacker/ubuntu:act-latest`

using ["act locally"](https://github.com/nektos/act) runner.
