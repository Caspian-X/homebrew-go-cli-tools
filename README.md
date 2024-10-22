# homebrew-go-cli-tools

A collection of Go cli tools for homebrew.

## Install

```sh
brew install caspian-x/tools/go-cli-tools
```

## Tools

### date-screenshots

Checks screenshot files (`.jpg`, `.jpeg`, `.png`, case insensitive) for a valid exif metadata tag for a date. If there is not a valid date, a date is searched for in the file's last modified time and other metadata tags and added to the `DateTimeOriginal` metadata tag.

#### Usage
```sh
date-screenshots <directory>
```

> Dry run flag: `-n` or `--dry-run`
