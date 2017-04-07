# agkozak Git Prompt
![agkozak supports five shells: zsh, bash, ksh, mksh, and dash](https://github.com/agkozak/agkozak-git-prompt/raw/master/img/agkozak-git-prompt.jpg)
*agkozak supports five shells: `zsh`, `bash`, `ksh`, `mksh`, and `dash`*

![In zsh, the exit status is displayed in the right prompt. The left prompt alters in appearance when the line editor is in vi command mode.](https://github.com/agkozak/agkozak-git-prompt/raw/master/img/exit-status-and-vi-mode.jpg)
*In `zsh`, the exit status is displayed in the right prompt. The left prompt alters in appearance when the line editor is in `vi` command mode.*

**agkozak Git Prompt** is a dynamic color prompt for `zsh`, `bash`, `ksh`, `mksh`, and `dash` that displays the current Git branch and status of the working directory. It uses basic ASCII symbols to do so, not Unicode glyphs, so it works with more fonts. In `zsh` it has the added features of altering the appearance of the prompt when in vi command mode and of displaying exit codes in the right prompt.

The symbols that agkozak Git Prompt uses to represent Git status are as follows:

Git Status | Symbol
--- | ---
Modified | !
Deleted | x
Untracked | ?
New file(s) | +
Ahead | \*
Renamed | >

agkozak Git Prompt can be used without any shell framework and can be loaded thus:

     . /path/to/agkozak-git-prompt/agkozak-git-prompt.sh

If you do use a framework, consult its documentation to see how you can load agkozak Git Prompt. For `zsh`, I use [zplugin](https://github.com/zdharma/zplugin), so my `.zshrc` has the line

    zplugin load agkozak/agkozak-git-prompt

