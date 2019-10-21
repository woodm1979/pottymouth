# pottymouth

Prevent bad words in your commits

## Motivation

I recently had a friend "jokingly" ask for a web-scraper to help prevent her
from including words like "Poop" in open-source repos.
This is my attempt to help.

## Setup

Optionally create a word-list file:

```bash
${EDITOR-vi} ~/.pottymouth
```

## Usage

```
usage: $0 [-h] [-f] [-a] [-g]
    -h: Show this help message.

    -f <wordlist>: Specify a word-list file.  Defaults to ~/.pottymouth .
    -a: Check all files in the repo.  Defaults to only checking modified files.

    -g: Make a git pre-commit hook.  That hook will use the remainder of the options if specified (-f, -a, ...)
```
