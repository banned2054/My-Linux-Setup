<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Oh-My-Zsh](#oh-my-zsh)
  - [安装](#%E5%AE%89%E8%A3%85)
  - [插件](#%E6%8F%92%E4%BB%B6)
    - [zsh-autosuggestions](#zsh-autosuggestions)
    - [zsh-syntax-highlighting](#zsh-syntax-highlighting)
- [Vim](#vim)
  - [monokai](#monokai)
  - [设置制表符宽度](#%E8%AE%BE%E7%BD%AE%E5%88%B6%E8%A1%A8%E7%AC%A6%E5%AE%BD%E5%BA%A6)
- [Linux Mirrors](#linux-mirrors)
  - [更新源](#%E6%9B%B4%E6%96%B0%E6%BA%90)
  - [安装Docker](#%E5%AE%89%E8%A3%85docker)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

惯用 linux 的工具和其对应的 github 仓库

## [Oh-My-Zsh](https://github.com/ohmyzsh/ohmyzsh)

### 安装

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### 插件

#### [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)

-   克隆此仓库到 `$ZSH_CUSTOM/plugins` 中（默认路径为 `~/.oh-my-zsh/custom/plugins`）：

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

-   将插件添加到 Oh My Zsh 的插件列表中以便加载（在 `~/.zshrc` 中）：

```
plugins=(
# other plugins...
zsh-autosuggestions
)
```

#### [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

-   克隆此仓库并引入脚本：

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/plugins/zsh-syntax-highlighting
```

-   添加以下行以自动启用语法高亮功能：

```bash
echo "source ~/.oh-my-zsh/plugins/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-~}/.zshrc
```

-   在当前的交互式 shell 中启用语法高亮：

```bash
source ~/.oh-my-zsh/plugins/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```

## Vim

### [monokai](https://github.com/ku1ik/vim-monokai)

-   下载主题文件

```bash
curl -fLo ~/.vim/colors/monokai.vim --create-dirs https://raw.githubusercontent.com/ku1ik/vim-monokai/refs/heads/master/colors/monokai.vim
```

-   添加以下行以自动启用 monokai 主题：

```bash
echo -e "\nsyntax enable\ncolorscheme monokai" >> ~/.vimrc
```

### 设置制表符宽度

```bash
echo -e "set tabstop=4\nset shiftwidth=4\nset expandtab" >> ~/.vimrc
```

## [Linux Mirrors](https://github.com/SuperManito/LinuxMirrors)

### 更新源

```bash
bash <(curl -sSL https://linuxmirrors.cn/main.sh)
```

### 安装Docker

```bash
bash <(curl -sSL https://linuxmirrors.cn/docker.sh)
```
