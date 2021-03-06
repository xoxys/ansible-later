---
title: Configuration
---

ansible-later comes with some default settings which should be sufficient for most users to start, but you can adjust most settings to your needs.

Changes can be made in a YAML configuration file or through CLI options which will be processed in the following order (last wins):

- default configuration (build-in)
- global configuration file (this will depend on your operating system)
- folder-based configuration file (.later.yml|.later.yaml|.later) in current working directory
- CLI options

Be careful! YAML Attributes will be overwritten while lists in any configuration file will be merged.

To make it easier to review a single file e.g. for debugging purpose, ansible-later will ignore `exclude_files` and `ignore_dotfiles` options.
