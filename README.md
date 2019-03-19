# meta-effective-spork

eslintrc, tsconfig, ... boilerplate tooling files

## hyperjs
### Plugins
#### hyperterm-visor
- Show/hid your Hyper terminal with a global hotkey.
- Configured to show/hide on Command+Tilde.
#### hyper-solarized-light
- light theme
#### hyperpower 
- Boom! with every keystroke :-)
#### hyper-statusline
- Status line showing current cwd and git branch status.

## oh-my-zsh
Make sure to add `shell: 'zsh'` to the `.hyper.js` config. 
### Theme
- `agnoster`
- Make sure to also install [Powerline
  Fonts](https://github.com/powerline/fonts)

First install the fonts:
```zsh
# clone
git clone https://github.com/powerline/fonts.git --depth=1
# install
cd fonts
./install.sh
# clean-up a bit
cd ..
rm -rf fonts
```

Then update the `fontFamily` in `.hyper.js`. The following are legible fonts:
- Cousine for Powerline
- Droid Sans Mono Slashed 

Run this command to test glyphs:
```
echo "\ue0b0 \u00b1 \ue0a0 \u27a6 \u2718 \u26a1 \u2699"
```
### Plugins
#### brew
- Completion for `brew`.
- Now comes automatically enabled with oh-my-zsh.
#### catimg
- Print pictures to `stdout`. Needs `brew install imagemagick`.
```zsh
catimg image.png
```
#### colorize
- Colorized `cat`. Use `ccat`.
- You'll need to `pip install pygments`.
#### dirhistory
- Navigate history via keyboard shortcuts.
- OPT-LEFT and OPT-RIGHT moves through directory history.
#### docker
- Completion for `docker`.
#### emacs
| Alias | Command	Description |
=========================================
|emacs	|$EMACS_LAUNCHER --no-wait	|Opens a temporary emacsclient frame|
|e	|emacs	|Same as emacs alias|
|te	|$EMACS_LAUNCHER -nw	|Open terminal emacsclient|
|eeval	|$EMACS_LAUNCHER --eval	|Same as M-x eval but from outside Emacs|
|eframe	|emacsclient --alternate-editor "" --create-frame	|Create new X frame|
|efile	|-	|Print the path to the file open in the current buffer|
|ecd	|-	|Print the directory of the file open in the the current buffer|
#### gitfast
- Completion for `git`. Much faster than official plugin from zsh.
#### osx
|Command	|Description|
===============================
|tab	|Open the current directory in a new tab|
|ofd	|Open the current directory in a Finder window|
|pfd	|Return the path of the frontmost Finder window|
|pfs	|Return the current Finder selection|
|cdf	|cd to the current Finder directory|
|pushdf	|pushd to the current Finder directory|
|quick-look	|Quick-Look a specified file|
|man-preview	|Open a specified man page in Preview app|
|showfiles	|Show hidden files|
|hidefiles	|Hide the hidden files|
#### per-directory-history
- Does what it's name says. Bound to CTRL-g.
#### web-search
```zsh
google foo bar # Google
ddg foo bar # DuckDuckGo
```
#### yarn
- Completion for `yarn`.
