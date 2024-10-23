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

### date-screenshots

Checks screenshot files (`.jpg`, `.jpeg`, `.png`, case insensitive) for a valid exif metadata tag for a date. If there is not a valid date, a date is searched for in the file's last modified time and other metadata tags and added to the `DateTimeOriginal` metadata tag.

#### Usage
```sh
date-screenshots <directory>
```

> Dry run flag: `-n` or `--dry-run`
