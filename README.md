# ShellDoc Themes (work in progress)

<!-- Tagline -->
<p align="center">
    <b>Install extensible documentation generators for ShellDoc</b>
    <br />
</p>


<!-- Badges -->
<p align="center">
    <a href="https://github.com/markdumay/shelldoc-themes/commits/main" alt="Last commit">
        <img src="https://img.shields.io/github/last-commit/markdumay/shelldoc-themes.svg" />
    </a>
    <a href="https://github.com/markdumay/shelldoc-themes/issues" alt="Issues">
        <img src="https://img.shields.io/github/issues/markdumay/shelldoc-themes.svg" />
    </a>
    <a href="https://github.com/markdumay/shelldoc-themes/pulls" alt="Pulls">
        <img src="https://img.shields.io/github/issues-pr-raw/markdumay/shelldoc-themes.svg" />
    </a>
    <a href="https://github.com/markdumay/shelldoc-themes/blob/main/LICENSE" alt="License">
        <img src="https://img.shields.io/github/license/markdumay/shelldoc-themes" />
    </a>
</p>

<!-- Table of Contents -->
<p align="center">
  <a href="#about">About</a> •
  <a href="#built-with">Built With</a> •
  <a href="#prerequisites">Prerequisites</a> •
  <a href="#deployment">Deployment</a> •
  <a href="#usage">Usage</a> •
  <a href="#contributing">Contributing</a> •
  <a href="#donate">Donate</a> •
  <a href="#license">License</a>
</p>


## About
| :warning: This repository is a work in progress and references to ShellDoc, which has not been released to the public yet. |
| --- |

ShellDoc is a documentation generator for Shell scripts using extensible themes. This repository is a companion for the ShellDoc application and maintains the themes available for installation by ShellDoc. Visit the [main repository][shelldoc_repository] of ShellDoc for usage instructions.


<!-- TODO: add tutorial deep-link 
Detailed background information is available on the author's [personal blog][blog].
-->

## Built With
Each ShellDoc theme uses [Go templates][go_template] to generate text output.

## Prerequisites
ShellDoc needs to be installed on your local machine. Visit the [main repository][shelldoc_repository] for more details.

## Deployment
ShellDoc provides the following built-in commands to manage the installation of the generators.

### Browse
Run the `browse` command to show the generators available for installation.

```console
shelldoc browse
```

By default, themes that are installed already are not displayed. Use the `--all` flag to show all available themes instead. If the theme is already installed it will get `*` appended to it's name.

```console
shelldoc browse --all
```

Run the following command to display the names of the available themes only. This will exclude the theme descriptions.

```console
shelldoc browse --brief
```

### Install
The `install` command installs a remote theme on the local machine. For example, the following command installs the Docsify theme. The theme's name is not case sensitive.

```console
shelldoc install docsify
```

<!--
### Remove an Installed Theme
### Upgrade Installed Themes
-->

## Usage
Visit the [main repository][shelldoc_repository] of ShellDoc for further usage instructions.

## Contributing
shelldoc-themes welcomes contributions of any kind, including new theme configurations. Please consider the guidelines in this section when contributing a new theme.

### Guidelines
- Themes in this repository are accepted only if they come with an Open Source license, that allows for the theme to be freely used, modified, and shared. Visit the [Open Source Initiative][open_source_url] for more details.
- The root folder of the theme should include a valid configuration file called `generator.json`.
- Submissions should include an instructive README. Please provide at least an English translation of the README.
- When adapting an existing theme for a derivative work, be sure the requirements of the original theme's license are met.
- When submitting a theme you are expected to maintain it as well. Please ensure your theme is compatible with the latest release of ShellDoc.

### Submitting a Theme
1. Clone the repository and create a new branch 
    ```console
    $ git checkout https://github.com/markdumay/shelldoc-themes.git -b name_for_new_branch
    ```
2. Make and test the changes
3. Submit a Pull Request with a comprehensive description of the changes


## Donate
<a href="https://www.buymeacoffee.com/markdumay" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/lato-orange.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;"></a>

## License
The ShellDoc Themes codebase is released under the [MIT license][license]. The README.md file is licensed under the Creative Commons *Attribution-NonCommercial 4.0 International* ([CC BY-NC 4.0)][cc-by-nc-4.0] license.

<!-- MARKDOWN PUBLIC LINKS -->
[cc-by-nc-4.0]: https://creativecommons.org/licenses/by-nc/4.0/
[docsify_url]: https://docsify.js.org
[go_template]: https://golang.org/pkg/text/template/
[open_source_url]: https://opensource.org/licenses

<!-- MARKDOWN MAINTAINED LINKS -->
<!-- TODO: add blog link
[blog]: https://markdumay.com
-->
[blog]: https://github.com/markdumay
[license]: https://github.com/markdumay/shelldoc-themes/blob/main/LICENSE
[shelldoc_repository]: https://github.com/markdumay/shelldoc.git
[repository]: https://github.com/markdumay/shelldoc-themes.git
