## Usage ##

```
git clone https://github.com/calid/configz.git --recurse-submodules
```

### Vim ###

```
ln -sv configz/vim ~/.vim
```

### Bash ###

```
ln -sv configz/skel/{.profile,.bash_profile,.bashrc} ~/
ln -sv configz/profile.d ~/.profile.d
ln -sv configz/bashrc.d ~/.bashrc.d
```

The prompt configuration expects a custom version of bash and/or readline. You can find details and instructions [here](https://github.com/calid/bash).

Alternatively, simply remove `\\m` from the PS1 in [bashrc.d/ps1.sh](https://github.com/calid/configz/blob/14d9ac3487a47cde2a4f0539d5e31b3e064eb1f4/bashrc.d/ps1.sh#L121)
