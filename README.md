# Personal dotfiles

Optional personal configuration for [Dotfiles](https://github.com/oscariquelme01/Dotfiles).

## Contents

- `git/` — my default Git identity and per-organization settings. Organization includes are relative to `gitconfig.personal`, so the directory can be deployed as a unit.
- `mailspring/vesper-theme/` — the Vesper Theme, a fork of [Sparky Mailspring Theme](https://github.com/siniux/Sparky-Mailspring-Theme). The upstream MIT license is included. Its `screenshot/` directory contains the original Sparky previews, not screenshots of Vesper.
- `packages.txt` — optional personal application packages for installation through `yay`; currently Mailspring.
- `assets/screenshots/` — screenshots for the main Dotfiles README.

## Deployment

The planned bootstrap integration clones this repository only when personal setup is selected, then copies configuration to its application locations. That integration is not implemented yet.

The Git directory is intended to be copied to `~/.config/git/personal/`, with `~/.gitconfig.local` including `~/.config/git/personal/gitconfig.personal`. Customize the organization directory patterns for your machine. SSH keys referenced by Git configuration are supplied separately.

For manual theme installation, select `mailspring/vesper-theme/` through Mailspring's **Edit → Install Theme…** menu, then choose **Vesper** under **Preferences → Appearance**.

Firefox configuration will be added later. Account credentials, private keys, mail databases, and browser session data do not belong in this repository.
