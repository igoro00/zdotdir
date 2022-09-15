# zdotdir

My `$ZDOTDIR` [dotfiles] directory, which contains my zsh configuration.

## Installation

Install this dotfiles repo to your `$ZDOTDIR`:

```zsh
# set the amazing ZDOTDIR variable
export ZDOTDIR=~/.config/zsh

# clone this repo
git clone --recursive https://github.com/igoro00/zdotdir $ZDOTDIR

# change the root .zshenv file to use ZDOTDIR
cat << 'EOF' >| ~/.zshenv
export ZDOTDIR=~/.config/zsh
[[ -f $ZDOTDIR/.zshenv ]] && . $ZDOTDIR/.zshenv
EOF

# load zsh
zsh
```

## Configuration

Aliases:
- See [aliases.txt](https://github.com/igoro00/zdotdir/blob/main/conf.d/aliases.zsh)

Plugins:
- See [.zplugins.txt](https://github.com/igoro00/zdotdir/blob/main/.zplugins.txt)


## Look-and-feel

### Fonts

I use nerdfonts-patched Source Code Pro Medium Regular 18pt

Install nerdfonts

```zsh
yay -S nerd-fonts-hack nerd-fonts-complete
```

## Resources

- [antidote][antidote]
- [zephyr][zephyr]
- [zshzoo][zshzoo]
- [zsh_unplugged][zsh_unplugged]
- [prezto][prezto]
- [oh-my-zsh][oh-my-zsh]
- [supercharge your terminal with zsh][supercharge-zsh]
- [awesome zsh][awesome-zsh-plugins]

[antidote]:             https://github.com/mattmc3/antidote
[awesome-zsh-plugins]:  https://github.com/unixorn/awesome-zsh-plugins
[dotfiles]:             https://dotfiles.github.io/
[homebrew]:             https://brew.sh
[iterm2-colors]:        https://github.com/mbadolato/iTerm2-Color-Schemes
[nerd-fonts]:           https://github.com/ryanoasis/nerd-fonts
[oh-my-zsh]:            https://github.com/ohmyzsh/ohmyzsh
[prezto]:               https://github.com/sorin-ionescu/prezto
[starship-toml]:        https://github.com/mattmc3/zdotdir/blob/main/prompt/starship.toml
[starship]:             https://starship.rs
[supercharge-zsh]:      https://blog.callstack.io/supercharge-your-terminal-with-zsh-8b369d689770
[zdotdir_gif]:          https://raw.githubusercontent.com/mattmc3/zdotdir/resources/img/zdotdir.gif
[zephyr]:               https://github.com/zshzoo/zephyr
[zsh_unplugged]:        https://github.com/mattmc3/zsh_unplugged
[zshzoo]:               https://github.com/zshzoo/zshzoo
