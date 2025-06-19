# dotfiles
collection of dotfiles

## Setup

```bash
export DOT=$HOME/${repo_path}/dotfiles
```

```bash
mkdir -p __setup git kitty/.config zsh
touch setup.sh
```

```bash
mv ~/.gitconfig $DOT/git
```

```bash
stow -v -R -t ~ git
```

`-v` verbose stow execution (see what its doing)
`-R` purge old links
`-t ~` target where stow should install
`git` the directory we are installing to `~` target

```bash
ls -la | grep .git
```
