## Usage ##

```
git clone https://github.com/calid/dotfiles.git --recurse-submodules
```

### Caveat Emptor ###

These configurations are provided as-is, without warranty or guarantees. They work for me, but they may not work for you. You should review these files before using them and modify them based on your needs. You have been warned.

### Vim ###

```
ln -sv dotfiles/vim ~/.vim
```

### Bash ###

```
ln -sv dotfiles/skel/{.profile,.bash_profile,.bashrc} ~/
ln -sv dotfiles/profile.d ~/.profile.d
ln -sv dotfiles/bashrc.d ~/.bashrc.d
ln -sv dotfiles/etc/inputrc ~/.inputrc
```
one-time/login configurations are under `profile.d` (e.g. environment variables). per-shell/interactive configurations are under `bashrc.d` (e.g. prompt & aliases).

The prompt configuration expects a custom version of bash and/or readline. You can find details and instructions [here](https://github.com/calid/bash).

Alternatively, if you don't care about the custom behavior remove `\\m` from the PS1 in [bashrc.d/ps1.sh](https://github.com/calid/dotfiles/blob/14d9ac3487a47cde2a4f0539d5e31b3e064eb1f4/bashrc.d/ps1.sh#L121) and set `show-mode-in-prompt` to `off` in [etc/inputrc](https://github.com/calid/dotfiles/blob/caa9797df1e1bdc12b41f311ab7edc064400d730/etc/inputrc#L6).

### etc ###

symlink the files under `etc` as appropriate
