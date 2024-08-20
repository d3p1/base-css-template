<div align=center>

# [BASE CSS TEMPLATE]

[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
[![Release](https://github.com/d3p1/base-css-template/actions/workflows/release.yml/badge.svg)](https://github.com/d3p1/base-css-template/actions/workflows/release.yml)
[![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release)

</div>

## Introduction

A [repository aimed at serving as a template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) to implement projects using `CSS`, providing basic configurations for using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) and [Prettier](https://prettier.io/). It also includes a setup for use within a [Dev Container](https://code.visualstudio.com/docs/devcontainers/containers), featuring optimized [VSCode](https://code.visualstudio.com/) configurations for working with these technologies. Lastly, it incorporates [GitHub Actions](https://github.com/features/actions) that automate the project [release](./.github/workflows/release.yml).

## Usage

This [template repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) is ready for immediate use with basic configurations for various technologies.

## Brief technical overview

We will proceed with detailed information about the various technologies used:

- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/): This repository comes with [`commitlint`](https://commitlint.js.org/) and [`husky`](https://typicode.github.io/husky/) installed, along with the [`@d3p1/commitlint-config` configuration](https://github.com/d3p1/commitlint-config), to enforce commits to follow the format: `<type>(<scope>): <description> [<issue-number>]`

- [Prettier](https://prettier.io/): This repository includes `prettier` for maintaining code with a consistent style.

- [GitHub Actions](https://github.com/features/actions): The [release workflow](.github/workflows/release.yml) uses [Semantic Release](https://github.com/semantic-release/semantic-release) (in reality, it uses the [`d3p1/semantic-releasify@v1` action](https://github.com/d3p1/semantic-releasify) to facilitate its use). Since the [Semantic Release](https://github.com/semantic-release/semantic-release) bot creates a tag for each release, updates the `CHANGELOG.md`, and generates a release, it's necessary for the branch to not be protected so that the bot can add its changes without issues. As this repository is intended to serve as a template for personal repositories, this isn't a major concern, as non-contributors (and in personal repositories, typically, the only contributor is the repository owner) won't be able to `push` directly to the default branch or approve PRs from forks made to submit changes.

## Changelog

Detailed changes for each release are documented in [`CHANGELOG.md`](./CHANGELOG.md).

## License

This work is published under [MIT License](./LICENSE).

## Author

Always happy to receive a greeting on:

- [LinkedIn](https://www.linkedin.com/in/cristian-marcelo-de-picciotto/)
- [Web](https://d3p1.dev/)
