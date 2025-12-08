An overview/list of all the tools used for _advanced volunteering_.
The tools are mostly tech tools.

Hosted using GitHub Pages.

## Deployment
To be as simple as possible we run homer using GitHub Pages, since it's static. The instance is created and configured using GitHub Actions.
This happens on every push commit to main (merged PR).

## Custom favicon
Homer project seems to not support custom favicon by default.

To add a custom favicon:
- generate a "favicon bundle" as specified in the [Homer docs subpage](https://github.com/bastienwirtz/homer/blob/main/public/assets/icons/README.md)
- replace the `favicon.zip` file
It will be extracted into correct path during deployment.
