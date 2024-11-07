[Source Link](https://github.com/zsh-users/zsh-autosuggestions)

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

