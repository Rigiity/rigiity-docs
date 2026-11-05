# Rigiity Docs

The documentation source for Rigiity: the Organization Handbook, product documentation, and guides. Built with [Mintlify](https://www.mintlify.com) and published at `docs.rigiity.com`.

## Local preview

This repo is developed with [Bun](https://bun.com). The Mintlify CLI is run through Bun with a pinned version, chosen per the release-age policy in the handbook's dependency audit checklist:

```sh
bunx mint@4.2.1133 dev --no-open
```

The preview serves at `http://localhost:3000` with hot reload. Search requires `mint login` and is not needed for local work.

## Updating the pinned CLI version

Before bumping the pin, check the package's publish history on the npm registry and pick a version at least 7 days old, unless the newer version has been audited directly per the [dependency audit checklist](https://docs.rigiity.com/handbook/tech-protocols/security-guidelines#evaluating-new-dependencies-and-tools).

## Publishing

The workflow is two-branch:

- `dev` is the development branch: content is written locally, committed, and pushed freely. Nothing publishes from it.
- `main` is the deployment branch: Mintlify builds the live site from it. When `dev` is presentable, we merge it into `main` and push; which will publish.

## Licensing

See [LICENSE](LICENSE): documentation text is CC BY-NC-SA 4.0; logos and visual assets are all rights reserved.

## Contributing

Changes go through pull requests. Content is reviewed and merged by management or an approved reviewer. If something in the docs is wrong or unclear, that is a bug in our documentation: open an issue or pull request.
