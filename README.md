char101/Outliner
================

Project status: alpha | Usable: yes | Bugs: most likely

## Overview

* Data is stored in a sqlite database
* Portable, can be built statically as a single executable
* Theoretically cross-platform
* Can zoom/unzoom specific item (set a specific item as the root of the outline) - with breadcrumb navigation
* Optional checkbox for each item
* Highlight a specific item (e.g. for marking currently executed task)
* Each item is rendered using markdown (with [hoedown](https://github.com/hoedown/hoedown))

![Screnshot](http://char101.github.io/outliner/images/screenshot.png)

## [Downloads](https://github.com/char101/outliner/releases/)

## Keyboard Bindings

* `Z` zoom
* `z` unzoom
* `c` show/hide checkbox
* `space` toggle checked state
* `h` toggle highlight
* `del` delete item
* `insert` append sibling
* `ctrl+insert` append child
* `ctrl+up/ctrl+down` move item up/down
* `ctrl+left/ctrl-right` move item left/right
* `F2/enter` Edit item

## Mouse Bindings

* Double click  
  On leaf node it will open the editor, otherwise zoom to the item

## Standard QTreeView Key Bindings

* `Up`  
  Moves the cursor to the item in the same column on the previous row. If the parent of the current item has no more rows to navigate to, the cursor moves to the relevant item in the last row of the sibling that precedes the parent.
* `Down`  
  Moves the cursor to the item in the same column on the next row. If the parent of the current item has no more rows to navigate to, the cursor moves to the relevant item in the first row of the sibling that follows the parent.
* `Left`  
  Hides the children of the current item (if present) by collapsing a branch.
* `Minus`  
  Same as LeftArrow.
* `Right`  
  Reveals the children of the current item (if present) by expanding a branch.
* `Plus`  
  Same as RightArrow.
* `Asterisk`  
  Expands all children of the current item (if present).
* `PageUp`  
  Moves the cursor up one page.
* `PageDown`  
  Moves the cursor down one page.
* `Home`  
  Moves the cursor to an item in the same column of the first row of the first top-level item in the model.
* `End`  
  Moves the cursor to an item in the same column of the last row of the last top-level item in the model.
* `F2`  
  In editable models, this opens the current item for editing. The Escape key can be used to cancel the editing process and revert any changes to the data displayed.

## Future Plan

* Schedule view - shows the list of task for each day based on the date set in the outline
* Timer view - similar to a pomodoro timer for currently executed task
