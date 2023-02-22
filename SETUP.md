# New computer dev setup
# first-light
New computer setup guide to get things just how I like them (generally for dev)

## Setup basic dev environment
### Setup iTerm2
Download [iTerm2](https://iterm2.com) and install.

Setup `option` key + arrows to travel word by word
* Go to iTerm2 Preferences -> Profiles -> Keys -> General
* Change `Left Option key` to `Normal`
* Switch to Profiles -> Keys -> Key Mappings
* Find Option + <- and change to:
	* Action: `Send Escape Sequence`
	* Esc+: `b`
* Find Option + -> and change to:
	* Action: `Send Escape Sequence`
	* Esc+: `f`

### Setup terminal in general
Install [Homebrew](https://brew.sh) and follow subsequent instructions.

Install [Oh My Zsh](https://ohmyz.sh)

Install `asdf`:
```
brew install asdf
brew plugin-install python
# other plugins too
```

#### Setup zsh aliases
```
touch ~/.git-aliases
```
Add the following
```
alias gs="git status"
alias gd="git diff"
alias gdc="git diff --cached"
alias go="git checkout"
alias gl="git log"
```

And run:
`echo “source ~/.git-aliases" >> ~/.zshrc`

### Setup VSCode
[Visual Studio Code](https://code.visualstudio.com)

Useful extensions
```
Pylance
Python
Live Share
GitHub Copilot
Jupyter
```

#### Setup fira code font
[OS Instructions · tonsky/FiraCode Wiki · GitHub](https://github.com/tonsky/FiraCode/wiki/Installing#macos)
[VS Code Instructions · tonsky/FiraCode Wiki · GitHub](https://github.com/tonsky/FiraCode/wiki/VS-Code-Instructions)

#### General
Search and update settings below in settings menu.

```
files.insertFinalNewline -> true
files.trimFinalNewlines -> true
files.trimTrailingWhitespace -> true
```

## SSH key + github.com
[Generating a new SSH key and adding it to the ssh-agent - GitHub Docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
[Adding a new SSH key to your GitHub account - GitHub Docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

## More Mac related setup
### OS related settings
Turn on touch to click
Turn on three finger drag (in Accessibility -> Pointer Control -> Trackpad Options)

#### Mouse settings
Plugin mouse
Turn sensitivity all the way up (Settings -> Mouse Sensitivity)
Turn off mouse acceleration (wtf is there not a way to do this? The shitty way on the internet doesn’t work). I guess give up and use:
```
brew install --cask linearmouse
```

#### Change Screenshot save location
Press `Shift + Command + 5`  to open Screenshot app. Buttons are below the selection area. Click on Options -> Other Location and set it to (preferably) `~/Documents/Screenshots`.

### Other applications
[Rectangle](https://rectangleapp.com) is great for basic shortcut-based windows management. Use `recommended` shortcuts and customize the following:
* remove `Top Left`, `Top Right`, `Bottom Left`, `Bottom Right`
* set `First Third` to `Ctrl + Option + H`
* set `Center Third` to `Ctrl + Option + T`
* set `Last Third` to `Ctrl + Option + N`

Install [SensibleSideButtons](https://sensible-side-buttons.archagon.net) for better mouse support.

## Useful software
### General / productivity
Rectangle
SensibleSideButtons
Bear
Zoom
Discord
Slack
Spotify
DaisyDisk (disk space analysis)
Google Chrome
GIMP

### Dev related
Docker for Mac
Beekeeper Studio (PostgreSQL)
Insomnia (REST API query-er)
LICEcap (easy screencap GIF)
