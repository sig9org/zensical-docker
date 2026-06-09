# Docker image of Zensical

This is [Zensical](https://zensical.org/) as a Docker container image.

## How to Use

```sh
docker run --rm -v ${PWD}:/docs sig9/zensical:0.0.45 zensical build --clean
```

## DockerHub Supported tags

- [0.0.45](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.45/)
- [0.0.44](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.44/)
- [0.0.43](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.43/)
- [0.0.42](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.42/)
- [0.0.41](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.41/)
- [0.0.40](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.40/)
- [0.0.39](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.39/)
- [0.0.38](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.38/)
- [0.0.37](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.37/)
- [0.0.36](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.36/)
- [0.0.35](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.35/)
- [0.0.34](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.34/)
- [0.0.33](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.33/)
- [0.0.32](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.32/)
- [0.0.31](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.31/)
- [0.0.30](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.30/)
- [0.0.29](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.29/)
- [0.0.28](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.28/)
- [0.0.27](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.27/)
- [0.0.26](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.26/)
- [0.0.25](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.25/)
- [0.0.24](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.24/)
- [0.0.23](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.23/)
- [0.0.22](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.22/)
- [0.0.21](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.21/)
- [0.0.20](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.20/)
- [0.0.19](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.19/)
- [0.0.18](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.18/)
- [0.0.17](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.17/)
- [0.0.16](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.16/)
- [0.0.15](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.15/)
- [0.0.14](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.14/)
- [0.0.13](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.13/)
- [0.0.12](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.12/)
- [0.0.11](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.11/)
- [0.0.10](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.10/)
- [0.0.9](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.9/)
- [0.0.8](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.8/)
- [0.0.7](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.7/)
- [0.0.6](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.6/)
- [0.0.5](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.5/)
- [0.0.4](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.4/)
- [0.0.3](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.3/)
- [0.0.2](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.2/)
- [0.0.1](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.1/)
- [0.0.0](https://hub.docker.com/repository/docker/sig9/zensical/tags/0.0.0/)

## Example CI/CD Configuration for GitLab Pages (.gitlab-ci.yml)

```yaml
stages:
    - build

build-job:
    stage: build
    script:
        - docker run --user $(id -u):$(id -g) --rm -v ${PWD}:/docs sig9/zensical:0.0.45 zensical build --clean
        - rm -rf /var/www/html/*
        - cp -R site/* /var/www/html/
```

## References

- Official
    - [Zensical](https://zensical.org/)
    - [Zensical Documentation](https://zensical.org/docs/get-started/)
    - [Backlog](https://github.com/orgs/zensical/projects/2/views/1)
    - [GitHub](https://github.com/zensical/zensical)
    - [PyPi](https://pypi.org/project/zensical/) ([History](https://pypi.org/project/zensical/#history))
    - [DockerHub](https://hub.docker.com/r/zensical/zensical)
- Unofficial
    - DockerHub
        - [sig9/zensical](https://hub.docker.com/r/sig9/zensical)
    - GitHub
        - [Docker image of Zensical](https://github.com/sig9org/zensical-docker)
        - [Template for Zensical](https://github.com/sig9org/zensical-template)

## Releases

- [0.0.45](https://github.com/zensical/zensical/releases/tag/v0.0.45) (2026/06/09)
    - This version reverts a behavior change in link validation that was introduced in 0.0.44 which is causing false positives.
- [0.0.44](https://github.com/zensical/zensical/releases/tag/v0.0.44) (2026/06/05)
    - This version fixes several bugs related to link validation and macros, and ensures that dotfiles are not removed from the site directory during generation.
- [0.0.43](https://github.com/zensical/zensical/releases/tag/v0.0.42) (2026/05/19)
    - This version fixes further edge cases in link validation, and adds support for UTF-8 encoding with byte-order-marks.
- [0.0.42](https://github.com/zensical/zensical/releases/tag/v0.0.42) (2026/05/15)
    - This version includes a number of bug fixes and refactorings to improve the stability and accuracy of link validation, and fixes a reload loop when the custom_dir, which is auto-watched, is explicitly added to watch. Moreover, GLightbox is now only downloaded when needed, which fixes an issue when using Zensical in air-gapped environments.
- [0.0.41](https://github.com/zensical/zensical/releases/tag/v0.0.41) (2026/05/09)
    - This version adds support for [integrating tabular data](https://zensical.org/docs/setup/extensions/macros/#reading-tabular-data) as Markdown tables, covering the functionality of the [mkdocs-table-reader-plugin](https://pypi.org/project/mkdocs-table-reader-plugin/), as well as the [watch](https://zensical.org/docs/setup/basics/#watch) option to automatically rebuild on changes in unmonitored files. Table reading is implemented as part of [macros](https://zensical.org/docs/setup/extensions/macros/), which we shipped in [0.0.40](https://github.com/zensical/zensical/releases/tag/v0.0.40).
    - Additionally, the stability of link [validation](https://zensical.org/docs/setup/validation/) has been drastically improved, reducing the rate of false positives. We're working on support for validating links using [autorefs](https://mkdocstrings.github.io/autorefs/), which we'll provide in one of the next versions.
- [0.0.40](https://github.com/zensical/zensical/releases/tag/v0.0.40) (2026/05/05)
    - This version adds support for [macros](https://zensical.org/docs/setup/extensions/macros/), covering the functionality of the mkdocs-macros-plugin. Macros allow you to define custom variables and functions that can be used in your Markdown files, making it easier to manage and reuse content across your documentation.
    - We've implemented macros support as a Python Markdown extension, since it's essentially a Markdown preprocessor that doesn't need to be aware of the rest of Zensical's rendering process, except for the current page and configuration. The benefit is that it can now also be used in Python docstrings to build API documentation with [mkdocstrings](https://mkdocstrings.github.io/).
- [0.0.39](https://github.com/zensical/zensical/releases/tag/v0.0.39) (2026/05/02)
    - This version fixes several bugs related to link validation and lightbox configuration.
- [0.0.38](https://github.com/zensical/zensical/releases/tag/v0.0.38) (2026/04/30)
    - This version adds [link and footnote validation](https://zensical.org/docs/setup/validation/) and [strict mode](https://zensical.org/docs/setup/validation/#strict-mode) – two of the most frequently requested features. Zensical now checks all internal references at build time and reports issues with precise source locations, so broken links don't make it into your published documentation. Unlike MkDocs, which only validates final rendered links, Zensical also checks for unresolved references, as well as unused and shadowed definitions – covering the full lifecycle of a reference from definition to use.
- [0.0.37](https://github.com/zensical/zensical/releases/tag/v0.0.37) (2026/04/27)
    -This version adds support for installable themes. You can now bundle your theme overrides and package them into a custom theme which can be installed via pip.
    - As of now, we closely mirror the process used by MkDocs, where themes just need to register themselves in the mkdocs.themes entrypoint, to allow users that already have derivations of Material for MkDocs to run them on Zensical. In the coming months, with the advent of the [component system](https://zensical.org/about/roadmap/#component-system), we'll make this process much more flexible and foster reuse at the component level. For now, this is a first step to allow sharing of theme overrides and default configurations inside organizations with dozens or even thousands of projects.
- [0.0.36](https://github.com/zensical/zensical/releases/tag/v0.0.36) (2026/04/24)
    - This version adds the missing update of the user interface that should've been included with [v0.0.35]().
- [0.0.35](https://github.com/zensical/zensical/releases/tag/v0.0.35) (2026/04/24)
    - Please update to v0.0.36 – this version is missing some changes to the user interface for the new features.
    - This version adds native support for [GLightbox](https://biati-digital.github.io/glightbox/), a JavaScript lightbox library to add zoom and gallery features to images. Images can be automatically annotated with the new glightbox Markdown extension.
- [0.0.34](https://github.com/zensical/zensical/releases/tag/v0.0.34) (2026/04/21)
    - This version moves Zensical to the latest version of [ZRX](https://github.com/zensical/zrx), the foundation for Zensical and its ecosystem. It includes the module system, as well as a ground up rewrite of the scheduler and streaming API. We did extensive testing with several hundred projects we obtained from GitHub, so we don't expect any issues. However, if you encounter any problems, please let us know.
    - Moreover, this version ships support for usage of TOML v1.1.0 in zensical.toml, which allows new lines in inline tables. Thus, configuration files can now be made more readable, especially when they contain long lists of items.
- [0.0.33](https://github.com/zensical/zensical/releases/tag/v0.0.33) (2026/04/14)
    - This version updates our official [Docker image](https://hub.docker.com/r/zensical/zensical) to be based on Alpine Linux for better compatibility and ease of use. It also adds all recommended Markdown Extensions to the generated zensical.toml file when bootstrapping a project with zensical new, ensuring a smoother setup experience. Additionally, the [user interface](https://github.com/zensical/ui) is updated to [v0.0.13](https://github.com/zensical/ui/releases/tag/v0.0.13), which includes two bug fixes for anchor links in the table of contents.
- [0.0.32](https://github.com/zensical/zensical/releases/tag/v0.0.32) (2026/04/07)
    - This version fixes a bug where Markdown files used as snippets were included into auto-generated navigation, and a bug with prefix stripping when the site URL contains a path component. Additionally, the Pygments dependency was updated to mitigate a vulnerability.
- [0.0.31](https://github.com/zensical/zensical/releases/tag/v0.0.31) (2026/04/01)
    - This version updates the [user interface](https://github.com/zensical/ui) to [v0.0.12](https://github.com/zensical/ui/releases/tag/v0.0.12), which includes the [removal of 19 brand icons](https://lucide.dev/guide/version-1) due to the update of Lucide to v1, and the addition of 166 new icons, most of them in SimpleIcons and FontAwesome. Additionally, there are bug fixes related to the latest changes of the table of contents in the modern theme and instant navigation on anchor links.
- [0.0.30](https://github.com/zensical/zensical/releases/tag/v0.0.30) (2026/03/29)
    - This version adds support for [mike](https://github.com/jimporter/mike), a tool for managing multiple versions of MkDocs projects on GitHub Pages. We created [a tailored fork of mike](https://github.com/squidfunk/mike) for Zensical – all mike commands should work as expected. Please refer to [our documentation](https://zensical.org/docs/setup/versioning/) for setup instructions, and [mike's documentation](https://github.com/jimporter/mike#readme) for advanced usage patterns and options.
    - Note that this is a temporary solution. Zensical will ship [native support for versioning](https://zensical.org/about/roadmap/#versioning) in the near future, which will remove the GitHub Pages constraint and offer more flexibility in how versions are deployed and served.
    - The [user interface](https://github.com/zensical/ui) is updated to [v0.0.11](https://github.com/zensical/ui/releases/tag/v0.0.11), which adds a floating table of contents menu for mobile to the modern theme. The toggle sits at the bottom of the screen for easy thumb access, and the sidebar scrolls to accommodate arbitrarily long tables of contents. This release also includes several improvements: snappier sidebar animations, better tooltip readability, and improved inline code block sizing.
- [0.0.29](https://github.com/zensical/zensical/releases/tag/v0.0.29) (2026/03/24)
    - This version fixes an issue with absolute paths in links, as well as changed files not being picked up by Zensical on Windows 11.
- [0.0.28](https://github.com/zensical/zensical/releases/tag/v0.0.28) (2026/03/19)
    - This version updates the [user interface](https://github.com/zensical/ui) to [v0.0.10](https://github.com/zensical/ui/releases/tag/v0.0.10), which fixes a couple of bugs related to search and code annotation rendering. Additionally, it adds support for version selectors in the modern theme, paving the way for adding support for [mike](https://github.com/jimporter/mike) to manage multiple versions of documentation on GitHub Pages.In addition, this release adds new configuration options for the file watcher to improve compatibility in certain environments.
- [0.0.27](https://github.com/zensical/zensical/releases/tag/v0.0.27) (2026/03/14)
    - This version fixes a reload loop for when auto-appended snippets are located inside of the docs directory, and auto-reload for pages with Chinese path segments.
- [0.0.26](https://github.com/zensical/zensical/releases/tag/v0.0.26) (2026/03/11)
    - This version fixes a regression introduced in 0.0.25 where the wheels built for manylinux x86 would be based on Python 3.8 instead of Python 3.10, making Zensical unusable on those architectures. This is related to a [recent bug](https://github.com/PyO3/maturin/issues/3059) in our upstream dependency [maturin](https://github.com/PyO3/maturin), which was introduced in version 1.12.5. Additionally, it fixes a deprecation warning on Python 3.14 when using the emoji extension.
- [0.0.25](https://github.com/zensical/zensical/releases/tag/v0.0.25) (2026/03/11)
    - This version updates the [user interface](https://github.com/zensical/ui) to [v0.0.9](https://github.com/zensical/ui/releases/tag/v0.0.9), which improves on accessibility and fixes some minor rendering issues. Additionally, it fixes some bugs related to configuration parsing and plugin handling in zensical serve, ensuring a smoother development experience.
- [0.0.24](https://github.com/zensical/zensical/releases/tag/v0.0.24) (2026/02/26)
    - This version updates the [user interface](https://github.com/zensical/ui) to [v0.0.8](https://github.com/zensical/ui/releases/tag/v0.0.8), which fixes issues with instant previews for Chinese and other non-ASCII languages, and layout shifts when switching from short to long pages in the modern theme. Additionally, same-page links for when directory URLs are disabled where not resolved correctly, which is fixed as well.
- [0.0.23](https://github.com/zensical/zensical/releases/tag/v0.0.23) (2026/02/12)
    - This version fixes a regression introduced in 0.0.22, where builds would error with mkdocstrings being not found, although the plugin wasn't configured.
- [0.0.22](https://github.com/zensical/zensical/releases/tag/v0.0.22) (2026/02/12)
    - This version adds support for the [autorefs](https://github.com/mkdocstrings/autorefs) plugin, and further improves performance for large mkdocstrings projects. The [user interface](https://github.com/zensical/ui) is updated to [v0.0.7](https://github.com/zensical/ui/releases/tag/v0.0.7), which fixes some isses with the mobile browsering experience.
- [0.0.21](https://github.com/zensical/zensical/releases/tag/v0.0.21) (2026/02/05)
    - This version updates the [user interface](https://github.com/zensical/ui) to [v0.0.6](https://github.com/zensical/ui/releases/tag/v0.0.6), which fixes excessive memory usage for pages with hundreds of links that are marked with data-preview (for instant previews), among several other improvements and bug fixes.
        - Back-to-top button was moved to the bottom for modern theme
        - Several fixes for instant previews, improving memory usage and usability
- [0.0.20](https://github.com/zensical/zensical/releases/tag/v0.0.20) (2026/01/29)
    - This version fixes excessive memory usage when building large mkdocstrings-powered documentation sites. Additionally, it fixes an issue where the build sometimes terminates prematurely. We're working on further improvements to memory consumption and stability in upcoming releases, as we're currently refactoring a significant part of the runtime.
- [0.0.19](https://github.com/zensical/zensical/releases/tag/v0.0.19) (2026/01/25)
    - This version adds support for the generation of objects.inv for your [mkdocstrings](https://mkdocstrings.github.io/)-powered documentation site, allowing external tools to discover and link to your API documentation. No changes to your configuration are necessary.
- [0.0.18](https://github.com/zensical/zensical/releases/tag/v0.0.18) (2026/01/23)
    - This version fixes a reload loop when mkdocstrings paths setting is set to ., which was introduced in 0.0.17 as a regression, and a race condition related to caching is resolved. Additionally, Zensical was too retrictive, only allowing specific meta keys for the navigation templates. This has been relaxed to allow any meta keys to be used.
- [0.0.17](https://github.com/zensical/zensical/releases/tag/v0.0.17) (2026/01/19)
    - This version brings support for automatic and manual API cross-references. Symbol names on pages that include auto-generated API documentation now automatically link to the relevant section. Additionally, manual cross-references can be created both in Markdown pages and Python docstrings with the following syntax:
- [0.0.16](https://github.com/zensical/zensical/releases/tag/v0.0.16) (2026/01/16)
    - This version updates the [user interface](https://github.com/zensical/ui) to [v0.0.4](https://github.com/zensical/ui/releases/tag/v0.0.4), which fixes searching for & characters, as well as usage of Lucide icons in the footer, and adds support for custom admonition icons via theme configuration.
- [0.0.15](https://github.com/zensical/zensical/releases/tag/v0.0.15) (2025/12/24)
    - This release updates the [user interface](https://github.com/zensical/ui) to [v0.0.3](https://github.com/zensical/ui/releases/tag/v0.0.3), which includes support for fuzzy search, and improves tooltip behavior on touch devices.
- [0.0.14](https://github.com/zensical/zensical/releases/tag/v0.0.14) (2025/12/22)
    - This release includes the [official Docker image](https://hub.docker.com/r/zensical/zensical) for Zensical, and fixes problems with hanging builds on Linux and Windows, as well as the build cache not being invalidated when templates were changed in overrides.
- [0.0.13](https://github.com/zensical/zensical/releases/tag/v0.0.13) (2025/12/19)
    - This release updates the [user interface](https://github.com/zensical/ui) to [v0.0.2](https://github.com/zensical/ui/releases/tag/v0.0.2), which includes various improvements and bug fixes, and ships 132 new icons. It might be a breaking change, as Simple icons removed 44 icons in their latest release, so make sure you're not using them. See the [v0.0.2](https://github.com/zensical/ui/releases/tag/v0.0.2) release notes for details.
- [0.0.12](https://github.com/zensical/zensical/releases/tag/v0.0.12) (2025/12/18)
    - This release fixes several issue with mkdocs.yml parsing, problems with zensical new, and other bugs. It's also the first release that goes through our new release workflow powered by mono, our new [mono](https://github.com/zensical/mono) repository automation tool.
- [0.0.11](https://github.com/zensical/zensical/releases/tag/v0.0.11) (2025/12/03)
    - This release adds support for [mkdocstrings](https://zensical.org/docs/setup/extensions/mkdocstrings/), enabling generation of API reference documentation for Python projects. Note that cross-references and backlinks are not yet supported – we're working on it.
- [0.0.10](https://github.com/zensical/zensical/releases/tag/v0.0.10) (2025/11/26)
    - This release includes two massive performance improvements for Disco.
- [0.0.9](https://github.com/zensical/zensical/releases/tag/v0.0.9) (2025/11/20)
- [0.0.8](https://github.com/zensical/zensical/releases/tag/v0.0.8) (2025/11/15)
- [0.0.7](https://github.com/zensical/zensical/releases/tag/v0.0.7) (2025/11/13)
- [0.0.6](https://github.com/zensical/zensical/releases/tag/v0.0.6) (2025/11/12)
- [0.0.5](https://github.com/zensical/zensical/releases/tag/v0.0.5) (2025/11/08)
- [0.0.4](https://github.com/zensical/zensical/releases/tag/v0.0.4) (2025/11/06)
- [0.0.3](https://github.com/zensical/zensical/releases/tag/v0.0.3) (2025/11/05)
