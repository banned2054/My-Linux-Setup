[Source Link](https://github.com/zsh-users/zsh-syntax-highlighting)

-   Simply clone this repository and source the script:

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git /home/$USER/.oh-my-zsh/plugins/zsh-syntax-highlighting
echo "source /home/$USER/.oh-my-zsh/plugins/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
```

-   Then, enable syntax highlighting in the current interactive shell:

```bash
source /home/$USER/.oh-my-zsh/plugins/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```