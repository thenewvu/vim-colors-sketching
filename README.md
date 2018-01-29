What's this?
============

A minimal light colorscheme for Vim/Neovim.

![neovim-nvim-vim-colors-sketching-screenshot](./demo.png?raw=true)

In the screenshot:

* The iterm2 color preset: PencilLight
* The font: [Script 12 Pitch PT](http://www.myfonts.com/fonts/bitstream/script-12-pitch/)
* The buffer line: [ap/vim-buftabline](https://github.com/ap/vim-buftabline)
* The tmux theme: [edkolev/tmuxline.vim](https://github.com/edkolev/tmuxline.vim) with below configs:
  ```
  let g:tmuxline_powerline_separators = 0
  let g:tmuxline_theme = 'vim_statusline_1'
  let g:tmuxline_preset = {
    \ 'win': '#W',
    \ 'cwin': '#W#F',
    \ 'options': {
    \   'status-justify': 'left'}
    \}
  ```

Requirements
============

* `set termguicolors` in your `.vimrc`: Read
  [this](https://gist.github.com/XVilka/8346728) to check if your terminal
  emulator supports it or not

Installation
============

If you use `vim-plug`, do something like this in your `.vimrc`.

``` 
Plug 'thenewvu/vim-colors-sketching' 
set rtp+=~/.vim/plugged/vim-colors-sketching
colorscheme sketching
```

For other plugin managers, please follow their guide.

Suggestions
===========

This colorscheme works very well with [vim-gigutter](https://github.com/airblade/vim-gitgutter). You can see the above screenshot. For other VCS (version control system), you can use [vim-signify](https://github.com/mhinz/vim-signify). Below is my configurtion for `vim-gitgutter`, just for example:

```
Plug 'airblade/vim-gitgutter'
let g:gitgutter_highlight_lines = 1
hi link GitGutterAdd DiffAdd
hi link GitGutterChange DiffChange
hi link GitGutterDelete DiffDelete
hi link GitGutterAddLine DiffAdd
hi link GitGutterChangeLine DiffChange
hi link GitGutterDeleteLine Normal
hi link GitGutterChangeDeleteLine DiffChange
```

Credits
=======

* https://github.com/noahfrederick/vim-hemisu/
* https://github.com/reedes/vim-colors-pencil
* https://github.com/pbrisbin/vim-colors-off

License
=======

MIT.
