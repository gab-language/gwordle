# GWORDLE
This repository is mean to serve as an example of how to build and publish a Gab application.

## Repository Structure
The module containing our project is `gwordle@<version>`. There is only the one source file.

By changing the message `gui:` to `tui:` on line 7, you can play wordle in the terminal without launching a new os window.

## Building
To build the standalone executable, use the gab cli:
```bash
gab build -m github.com/gab-language/cgab@gab_version gwordle@version
```
This produces an executable for your platform. You may build cross-platform using the `-t` flag.

## Workflow
There is an example Github workflow file in this repository which creates a release, builds an executable for each platform, and attaches them to the release.
