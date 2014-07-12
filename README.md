# 2048-game.el #

This is an implementation of [2048](http://gabrielecirulli.github.io/2048/) in Emacs.

### Installing 2048-game.el ###

There are two ways to install 2048-game.el:

1. **[MELPA](http://melpa.milkbox.net/)** -- a package manager for emacs. This is the recommended way to install 2048-game.el
    1. Follow the instructions under "installing" on MELPA's [getting started](http://melpa.milkbox.net/#/getting-started) page.
    2. Restart Emacs, to make it reload your init file.
    3. Run `M-x package-list-packages`.
    4. Find this package in the package list, and move point (the cursor) there. It should one of the first few in the list.
    5. Press `i` to mark the package for installation.
    6. Press `x` to execute the commands and install the marked package.

2. You can install the game from source. This is not recommended unless you're changing the code.
    1. Clone this repository.
    2. Run `M-x load-file`, then navigate to the repository, and load `2048-game.el`

### Playing ###

* The goal is to create a tile with value 2048.
* Start the game by typing `M-x 2048-game`, and pressing enter.
* You can move the tiles around with the arrow keys, p/n/b/f, or C-p/C-n/C-b/C-f.
* Whenever the board moves, all tiles slide as far to that direction as they can go. If a tile collides with another tile of the same value, the tiles combine into a  tile with double the initial value, and you gain the new tile's value as your score.
