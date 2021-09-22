# ShellDoc Generators (work in progress)

<!-- Tagline -->
<p align="center">
    <b>Install extensible documentation generators for ShellDoc</b>
    <br />
</p>


<!-- Badges -->
<p align="center">
    <a href="https://github.com/markdumay/shelldoc-generators/commits/main" alt="Last commit">
        <img src="https://img.shields.io/github/last-commit/markdumay/shelldoc-generators.svg" />
    </a>
    <a href="https://github.com/markdumay/shelldoc-generators/issues" alt="Issues">
        <img src="https://img.shields.io/github/issues/markdumay/shelldoc-generators.svg" />
    </a>
    <a href="https://github.com/markdumay/shelldoc-generators/pulls" alt="Pulls">
        <img src="https://img.shields.io/github/issues-pr-raw/markdumay/shelldoc-generators.svg" />
    </a>
    <a href="https://github.com/markdumay/shelldoc-generators/blob/main/LICENSE" alt="License">
        <img src="https://img.shields.io/github/license/markdumay/shelldoc-generators" />
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

ShellDoc is a documentation generator for Shell scripts using extensible generators. This repository is a companion for the ShellDoc application and maintains the generic generators available for installation by ShellDoc. Visit the [main repository][shelldoc_repository] of ShellDoc for usage instructions.


<!-- TODO: add tutorial deep-link 
Detailed background information is available on the author's [personal blog][blog].
-->

## Built With
Each ShellDoc generator uses [Go templates][go_template] to generate text output.

## Prerequisites
ShellDoc needs to be installed on your local machine. Visit the [main repository][shelldoc_repository] for more details.

## Deployment
ShellDoc provides the following built-in commands to manage the installation of the generators.

### Browse
Run the `browse` command to show the generators available for installation.

```console
shelldoc browse
```

By default, generators that are installed already are not displayed. Use the `--all` flag to show all available generators instead. If the generator is already installed it will get `*` appended to it's name.

```console
shelldoc browse --all
```

Run the following command to display the names of the available generators only. This will exclude the generator descriptions.

```console
shelldoc browse --brief
```

### Install
The `install` command installs a remote generator on the local machine. For example, the following command installs the Docsify generator. The generator's name is not case sensitive.

```console
shelldoc install docsify
```

<!--
### Remove an Installed Generator
### Upgrade Installed Generators
-->

## Usage
Visit the [main repository][shelldoc_repository] of ShellDoc for further usage instructions.

## Contributing
shelldoc-generators welcomes contributions of any kind, including new generator configurations. Please consider the guidelines in this section when contributing a new generator.

### Guidelines
- Generators in this repository are accepted only if they come with an Open Source license, that allows for the generator to be freely used, modified, and shared. Visit the [Open Source Initiative][open_source_url] for more details.
- The root folder of the generator should include a valid configuration file called `generator.json`.
- Submissions should include an instructive README. Please provide at least an English translation of the README.
- When adapting an existing generator for a derivative work, be sure the requirements of the original generator's license are met.
- When submitting a generator you are expected to maintain it as well and to ensure it is compatible with the latest release of ShellDoc.

### Submitting a Generator
1. Clone the repository and create a new branch 
    ```console
    $ git checkout https://github.com/markdumay/shelldoc-generators.git -b name_for_new_branch
    ```
2. Make and test the changes
3. Submit a Pull Request with a comprehensive description of the changes


## Donate
<a href="https://www.buymeacoffee.com/markdumay" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/lato-orange.png" alt="Buy Me A Coffee" style="height: 51px !important;width: 217px !important;"></a>

## License
The ShellDoc Generators codebase is released under the [MIT license][license]. The README.md file <!-- and files in the "[wiki][wiki]" repository are --> is licensed under the Creative Commons *Attribution-NonCommercial 4.0 International* ([CC BY-NC 4.0)][cc-by-nc-4.0] license.

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
[license]: https://github.com/markdumay/shelldoc-generators/blob/main/LICENSE
[shelldoc_repository]: https://github.com/markdumay/shelldoc.git
[repository]: https://github.com/markdumay/shelldoc-generators.git
<!-- [wiki]: https://github.com/markdumay/shelldoc-generators/wiki/
[wiki_commands]: https://github.com/markdumay/shelldoc-generators/wiki/Available-Commands
[wiki_dependencies]: https://github.com/markdumay/shelldoc-generators/wiki/Defining-Dependencies
[wiki_tags]: https://github.com/markdumay/shelldoc-generators/wiki/Using-Comments-Tags -->
