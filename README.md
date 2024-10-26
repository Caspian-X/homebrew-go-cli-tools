# homebrew-go-cli-tools

A collection of Go cli tools for homebrew.

## Install

```sh
brew install caspian-x/tools/go-cli-tools
```

## Upgrade

If you do not have the latest version you can just run
```sh
brew upgrade caspian-x/tools/go-cli-tools
```
> you can also run `brew upgrade` to upgrade all packages.

You can check if you have the latest version by checking the releases on the GitHub page and running
```sh
brew info caspian-x/tools/go-cli-tools
```

## Tools

### date-photos
```sh
date-photos <dir>
```
> Flags: --dry-run/-n

Checks files (`.jpg`, `.jpeg`, `.png`, `.webp`, case insensitive) for a valid exif metadata tag for a date. If there is not a valid date, a date is searched for in the file's last modified time and other metadata tags and added to the `DateTimeOriginal` metadata tag.

### remove-duplicate-photos
```sh
remove-duplicate-photos <dir>
```
> Flags: --dry-run/-n

Removes original photos/videos/files of ones that were edited on Apple devices. 
Example: if there are two photos, IMG_E1234.jpg and IMG_1234.jpg, this script will remove IMG_1234.jpg because IMG_E1234.jpg is the "newer", edited version.
