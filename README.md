This plugin provides a custom `checkout` hook that overrides Buildkite's default behavior and uses a [treeless clone](https://github.blog/2020-12-21-get-up-to-speed-with-partial-clone-and-shallow-clone/#user-content-treeless-clones) for the repository and all its submodules.

Currently, we use it in [gutenberg-mobile](https://github.com/wordpress-mobile/gutenberg-mobile/pull/6719) where it brought down the checkout time from ~5m 45s to ~30s.
