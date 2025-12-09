An overview/list of all the tools used for _advanced volunteering_.
The tools are mostly tech tools.

Hosted using GitHub Pages.

## Contribution
Edit `config.yml` and `customizations.css`.

> You can even edit them in your browser to see the result imediately!
> Open https://start.desering.org, open DevTools, locate `config.yml`, edit and enable "Local Overrides". Then, you can refresh the  page, but your local copy will be used. Then you can copy these additions here.

## Deployment
To be as simple as possible we run homer using GitHub Pages, since it's static. The instance is created and configured using GitHub Actions.
This happens on every push commit to main (merged PR).

## Custom favicon
Homer project seems to not support custom favicon by default.

To add a custom favicon:
- generate a "favicon bundle" as specified in the [Homer docs subpage](https://github.com/bastienwirtz/homer/blob/main/public/assets/icons/README.md)
- replace the `favicon.zip` file

It will be extracted into correct path during deployment.