# zsh_minimal
A perscrptive introduction to ZSH, FZF, Starship, and more...

---

# Install

```shell
brew install zsh fzf starship kitty font-sauce-code-pro-nerd-font
```

- [fzf](https://github.com/junegunn/fzf)
- [starship](https://starship.rs/guide/#step-1-install-starship)
- [kitty](https://github.com/kovidgoyal/kitty)
- [font-sauce-code-pro-nerd-font](https://github.com/ryanoasis/nerd-fonts)

---

# Drop in Config

```shell
cp ~/.zshrc ~/.zshrc.bak
wget https://raw.githubusercontent.com/gehrigkeane/zsh_minimal/main/.zshrc ~/.zshrc

mkdir -p ~/.config

cp ~/.config/starship.toml ~/.config/starship.toml.bak
wget https://raw.githubusercontent.com/gehrigkeane/zsh_minimal/main/starship.toml ~/.config/starship.toml

cp ~/.config/kitty/kitty.conf ~/.config/kitty/kitty.conf.bak
wget https://raw.githubusercontent.com/gehrigkeane/zsh_minimal/main/starship.toml ~/.config/kitty/kitty.conf
```

---

# Let's Play

TODO

---

# fzf

[fzf](https://github.com/junegunn/fzf)

```bash
# select git branches in horizontal split below (15 lines)
git branch | fzf-tmux -d 15
```

[fzf-tab](https://github.com/Aloxaf/fzf-tab)

```
# behold...
cd ~/...
gco ...
```

---

# ls

```bash
ls -lG
```

Environment variables can only get you soo far... let's leave the 1980's

My favorite: [lsd](https://github.com/Peltoche/lsd)

```bash
lsd -Al ~/
```

More popular, a bit slower: [exa](https://github.com/ogham/exa)

```bash
exa -al ~/
```

---

# Lightening round!

ncdu

[ripgrep](https://github.com/BurntSushi/ripgrep)

> ripgrep recursively searches directories for a regex pattern while respecting your gitignore 

```bash
rg "Repository" ./
```

[tldr](https://tldr.sh/) or [tealdeer](https://github.com/dbrgn/tealdeer)

> Simplified and community-driven man pages

```bash
tldr tar
```

[xh](https://github.com/ducaale/xh)

> Friendly and fast tool for sending HTTP requests 

```bash
xh :3000/users                 # resolves to http://localhost:3000/users
```

(macOCR) [ocr](https://github.com/schappim/macOCR)

> Get any text on your screen into your clipboard.

---

# Questions?

---

# References

[Shell Introduction](https://github.com/gehrigkeane/quick_pretty_demo)

Configuration Software

1. [starship](https://starship.rs/guide/#step-1-install-starship)
2. [zinit](https://github.com/zdharma-continuum/zinit)

ZSH Plugins

1. [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
2. [fast-syntax-highlighting](https://github.com/zdharma-continuum/fast-syntax-highlighting)

Command Line Tools

1. [slides](https://github.com/maaslalani/slides)
2. [lsd](https://github.com/Peltoche/lsd)
3. [exa](https://github.com/ogham/exa)
4. [fzf](https://github.com/junegunn/fzf)
5. [fzf-tab](https://github.com/Aloxaf/fzf-tab)
6. [tig](https://github.com/jonas/tig)
7. [forgit](https://github.com/wfxr/forgit)
8. [gti](http://r-wos.org/hacks/gti)
9. [rg](https://github.com/BurntSushi/ripgrep)
10. [tldr](https://github.com/dbrgn/tealdeer)
11. [xh](https://github.com/ducaale/xh)
12. [macOCR](https://github.com/schappim/macOCR)
