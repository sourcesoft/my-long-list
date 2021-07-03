## Installation

![Vim](https://user-images.githubusercontent.com/608906/124341365-bc3c4100-db89-11eb-8919-3ed3c7a6074a.png "vim")

![ZSH](https://user-images.githubusercontent.com/608906/124360522-6357c180-dbf8-11eb-9ce2-c9e9a54bcf5c.png "zsh")

#### 1. Install required binaries
1. Have [Alacritty](https://github.com/alacritty/alacritty) (Neo)Vim and Git installed ofcourse
2. Install `tmux` and the [plugins manager](https://github.com/tmux-plugins/tpm)
3. Install `zsh`: [Oh My ZSH](https://github.com/robbyrussell/oh-my-zsh), [pwerlevel10k theme](https://github.com/romkatv/powerlevel10k#oh-my-zsh), [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md) and [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md)
4. Install `Inconsolata font`  and [Knack Nerd Font](https://github.com/enricobacis/.dotfiles/blob/master/osx-fonts/Library/Fonts/Knack%20Regular%20Nerd%20Font%20Complete.ttf).
5. Install some cool binaries like [`universal-ctags`](https://github.com/universal-ctags/ctags), [The Silver Searcher](https://github.com/ggreer/the_silver_searcher), [bat](https://github.com/sharkdp/bat), [fd](https://github.com/sharkdp/fd), [exa](https://github.com/ogham/exa) and [delta](https://github.com/dandavison/delta)
6. If you're on OSX install [reattach-to-user-namespace](https://github.com/ChrisJohnsen/tmux-MacOSX-pasteboard)

#### 2. Backup your old configuration and get new ones
1. Backup the old one first: `mv ~/.vimrc ~/.vimrc.bak`
2. Replace it: `wget -O ~/.vimrc https://raw.githubusercontent.com/sourcesoft/my-long-list/master/.vimrc`
3. NeoVim uses XDG configuration: `ln -s ~/.vimrc ~/.config/nvim/init.vim`
4. Vim uses old `.vimrc` location so there's no need to create symlink.
5. Copy other config files in the repository like `.bash_profile`, `.alacritty.yml`, `.gitconfig`, `.tern-config`, `.tmux.conf`, `.zshrc`, `.eslintrc.js`, `prettierrc`, `.gitignore`, `.prettierignore`, `.ctags` and configure more if feel comfortable.

#### 3. Setup (Neo)Vim (in order)
1. Before opening (Neo)Vim:
- Install some required compilers for our plugins with `npm install -g typescript neovim`, `pip install pynvim`, `pip3 install pynvim`, `curl -L http://xrl.us/installperlosx | bash` and [GO](https://golang.org/doc/install)
- Open tmux running `tmux` and install tmux plugins with `Prefix + I`
- Setup plugins by first installing [vim-plug](https://github.com/junegunn/vim-plug) and then running `vim +PlugInstall +qall` or `nvim +PlugInstall +qall` in the terminal
2. Open (Neo)Vim and:
- run `:UpdateRemotePlugins` and `:GoInstallBinaries` 
- Learn key bindings by reading this file

## Mappings and Environment

It's much easier to use right CMD or Alt instead of reaching out to escape.
I also use Caps Lock for Control, since it's closer and easier to hit.
- Escape -> Right CMD or Right Alt
- Control -> Caps Lock

Tools to setup the key bindings:
- OSX: Use Karabiner to map
  - Visit: https://github.com/tekezo/Karabiner-Elements
- Ubuntu: Install xcape (https://github.com/alols/xcape)
  - Use the following command: `xcape -e 'Alt_R=Escape;ISO_Level3_Shift=Escape'`

### Tools included
- [NeoVim](https://neovim.io)
- [vimrc](https://github.com/sourcesoft/my-long-list/blob/master/.vimrc)
- [ag](https://github.com/ggreer/the_silver_searcher)
- [Alacritty](https://github.com/alacritty/alacritty)
- [zsh](https://github.com/robbyrussell/oh-my-zsh)
- [tmux](https://tmux.github.io/)
- [The Silver Searcher](https://github.com/ggreer/the_silver_searcher)
- [bat](https://github.com/sharkdp/bat)
- [fd](https://github.com/sharkdp/fd)
- [exa](https://github.com/ogham/exa)
- [delta](https://github.com/dandavison/delta)
