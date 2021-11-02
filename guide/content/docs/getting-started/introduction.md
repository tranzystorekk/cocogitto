+++
title = "Introduction"

weight = 10
sort_by = "weight"
template = "docs/page.html"

[extra]
toc = true
+++

Cocogitto comes with two standalone binaries: `coco` and `cog`.

Both of them, as well as their subcommands, have a `--help` to display options and usage:

```sh
$ cog --help
# Some help

$ cog changelog --help
# Other help

# And so on...
```

## Conventional commits with `coco`

`coco` is primarily meant to be used as a replacement for the `git commit` command.
It will produce commits with messages respecting the conventional commit specification, with little effort.

Example:

```sh
# With raw git
git commit -m "feat: implement parser specification"

# With coco
coco feat "implement parser specification"
```

## Repository management with `cog`

Whereas local commits are made with `coco`, `cog` is meant to manage you repo both locally and in a CI context.

|Subcommand    |Description                                                                            |
|--------------|---------------------------------------------------------------------------------------|
|`check`       |Verify all commit messages against the conventional commit specification               |
|`init`        |Initialize `cog` config files                                                          |
|`edit`        |Rename all invalid commit messages in the repo (interactive rebase)                    |
|`log`         |Like `git log` but for conventional commits                                            |
|`verify`      |Verify a single commit message                                                         |
|`changelog`   |Display changelog for a given commit OID range                                         |
|`bump`        |Commit changelog from latest tag to HEAD and create a new tag                          |
|`install-hook`|      Add conventional git hooks to the repository                                     |
