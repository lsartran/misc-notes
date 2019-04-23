More than having my laptop setup just the way I like, I want to /know/ what I changed for it to be the way I like. Attempt to list that below.

# macOS configuration

## System Preferences

### Keyboard

- Key Repeat: Fast
- Delay Until Repeat: Short

### Trackpad

#### Point & Click

- [X] Silent clicking
- [X] Force Click and haptic feedback

#### Scroll & Zoom

- [ ] Scroll direction: Natural

### User & Groups

- Shell: zsh

### Accessibility

#### Zoom

- [X] Use scroll gesture with modifier key to zoom: ^ Control

### From the CLI

```
# Enable key-repeat
defaults write -g ApplePressAndHoldEnabled -bool false
```

# Software to install

- Chrome
- Dash
- Dashlane
- Electrum
- Focus
- iTerm2
- Karabiner-Elements
- OmniFocus
- Slack
- Spectacle
- Spotify
- Sublime Text 3
- Transmission
- TrueCrypt 7.1a
- Tunnelblick
- VLC
- WhatsApp
- f.lux
- nvALT
- brew
    - git-annex
    - python3
    - stack
    - zsh
    - neovim

# Colour scheme

- Solarized (for Terminal)
    - Solarized Dark for Yosemite from https://github.com/jcberthon/solarized.git
    - Then, in Terminal > Preferences > Profiles > Solarized Dark for Yosemite > Cursor > Block (I cannot see Underline very well in vim)

# Config

- Install dotfiles

## Sublime Text

- `Preferences.sublime-settings` from `dotfiles` into `"~/Library/Application Support/Sublime Text 3/Packages/User/Preferences.sublime-settings"`

## Neovim

TBC

## iTerm2

Preferences > Profiles > Default > Text > Font > 16pt Monaco
