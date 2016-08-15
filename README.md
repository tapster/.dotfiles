first, install [janus](https://github.com/carlhuda/janus)

```
curl -Lo- https://bit.ly/janus-bootstrap | bash
```

and add vim-powerline and vimux

```
  mkdir -p ~/.janus
  cd ~/.janus
  git clone git@github.com:Lokaltog/vim-powerline.git
  git clone git@github.com:benmills/vimux.git
```

then install tmux:

    brew install tmux

then:

    cd ~
    git clone git@github.com:tapster/.dotfiles.git
    ln -s .dotfiles/.tmux.conf .tmux.conf
    ln -s .dotfiles/.vimrc.after .vimrc.after
    ln -s .dotfiles/.vimrc.before .vimrc.before
    ln -s .dotfiles/.gvimrc.local .gvimrc.local
    ln -s .dotfiles/.zshrc .zshrc
    ln -s .dotfiles/.gitconfig .gitconfig
    mkdir -p ~/.oh-my-zsh/custom/plugins/tapster
    ln -s .dotfiles/.oh-my-zsh/custom/plugins/tapster.plugin.zsh ~/.oh-my-zsh/custom/plugins/tapster/tapster.plugin.zsh
