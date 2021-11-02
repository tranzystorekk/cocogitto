+++
title = "Quickstart"

weight = 20
sort_by = "weight"
template = "docs/page.html"
+++

## Installation

### Cargo

Cocogitto is available on [crates.io](https://crates.io/crates/cocogitto):

```sh
cargo install cocogitto
```

### Arch linux

```sh
yay -S cocogitto-bin
```

## Shell completion

### Bash

```sh
cog generate-completions bash > ~/.local/share/bash-completion/completions/cog
coco generate completions bash > ~/.local/share/bash-completion/completions/coco
```

### Bash (macOS/Homebrew)

```sh
cog generate-completions bash > $(brew --prefix)/etc/bash_completion.d/cog.bash-completion
coco generate-completions bash > $(brew --prefix)/etc/bash_completion.d/coco.bash-completion
```

### Fish

```sh
mkdir -p ~/.config/fish/completions
cog generate-completions fish > ~/.config/fish/completions/cog.fish
coco generate-completions fish > ~/.config/fish/completions/coco.fish
```

### Zsh

```sh
cog generate-completions zsh > ~/.zfunc/_cog
coco generate-completions zsh > ~/.zfunc/_coco
```
