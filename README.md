# My-Linux-Setup
 惯用linux的工具和其对应的github仓库

## [Oh-My-Zsh](https://github.com/ohmyzsh/ohmyzsh)

### Install

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Plugins

#### [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)

-   Clone this repository into `$ZSH_CUSTOM/plugins` (by default `~/.oh-my-zsh/custom/plugins`)

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

-   Add the plugin to the list of plugins for Oh My Zsh to load (inside `~/.zshrc`):

```
plugins=( 
# other plugins...
zsh-autosuggestions
)
```

#### [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

-   Simply clone this repository and source the script:

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/plugins/zsh-syntax-highlighting
```

-   Add the following line to automatically enable syntax highlighting in every session:

```bash
echo "source ~/.oh-my-zsh/plugins/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-~}/.zshrc
```

-   Then, enable syntax highlighting in the current interactive shell:

```bash
source ~/.oh-my-zsh/plugins/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```

## Vim 

### Theme

[monokai](https://github.com/ku1ik/vim-monokai)

-   Download the theme file

```bash
curl -fLo ~/.vim/colors/monokai.vim --create-dirs https://raw.githubusercontent.com/ku1ik/vim-monokai/refs/heads/master/colors/monokai.vim
```

-   Add the following line to automatically enable monokai:

```bash
echo -e "\nsyntax enable\ncolorscheme monokai" >> ~/.vimrc
```

