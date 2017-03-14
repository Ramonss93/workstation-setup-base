# Base Workstation Setup

This is my base Fedora 25 workstation setup with any sensitive information removed.
I've used these scripts since Fedora 18 came out to automatically provision my
workstation with a fresh install of Fedora. There are two scripts that need to be
ran:

- `sudo ./bin/install-packages` - This script installs all of the packages from the
  Fedora repositories.
- `./bin/setup-user-settings` - Sets up various user settings including gsettings,
  dconf, symlinks for some config files, background, user icon, etc.

In the past, I've tried to version all of the config files in my home directory and
that ended up becoming a mess. I've found that it is better to only version the
config files that I care about in a git repo, and symlink them into my home directory.
