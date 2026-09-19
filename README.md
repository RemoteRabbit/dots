# dots

Portable machine configuration managed by [mise](https://mise.jdx.dev/).

## Bootstrap a machine

Install `mise`, Git, and Zsh, then run:

```sh
mise bootstrap --from https://github.com/remoterabbit/dots --yes
```

This clones the Neovim and Zsh configuration repositories and links:

- `~/.config/mise/config.toml`
- `~/.config/nvim`
- `~/.config/zsh`
- `~/.zshenv`

Start a new Zsh session after bootstrap. The Zsh configuration installs Zinit
and its plugins on first launch.

To preview or repair only the managed links:

```sh
mise bootstrap dotfiles apply --dry-run
mise bootstrap dotfiles apply --yes
```
