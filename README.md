# pottymouth

Prevent bad words in your commits

## Motivation

I recently had a friend "jokingly" ask for a web-scraper to help prevent her
from including words like `Poop` in open-source repos.
I think a git pre-commit hook would be easier to write.
This is my attempt to help.

In retrospect, this should likely be a gist, but I just don't like them very much.

## Setup

Optionally create a word-list file:

```bash
${EDITOR-vi} ~/.pottymouth
```

Consider filling your word-list file with words from [this list](http://www.bannedwordlist.com/lists/swearWords.txt).

## Usage

```
usage: $0 [-h] [-f] [-a] [-g]
    -h: Show this help message.

    -f <wordlist>: Specify a word-list file.  Defaults to ~/.pottymouth .
    -a: Check all files in the repo.  Defaults to only checking modified files.

    -g: Make a git pre-commit hook.  That hook will use the remainder of the options if specified (-f, -a, ...)
```
