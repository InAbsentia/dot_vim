# The Vim Configuration of Champions

[See dot_vim's Stats on GitEgo](http://gitego.com/mutewinter/dot_vim)

## Installation

1. `git clone http://github.com/mutewinter/dot_vim.git ~/.vim`
2. `cd ~/.vim`
3. `rake vim:link` to make the .vimrc symbolic link.
4. Install [Vundle](https://github.com/gmarik/vundle) with `git clone
   http://github.com/gmarik/vundle.git bundle/vundle`
5. `vim "+mkspell ~/.vim/spell/custom.en.utf-8.add" +BundleInstall +qall`
_installs all of the plugins and compiles custom spellings._
6. Enjoy enhanced productivity, increased levitation, reduced
watermelon-related accidents, and startling sex appeal.

## Screenshots

**MacVim** / **Windows gVim**

[![MacVim](https://github.com/mutewinter/dot_vim/raw/master/screenshots/MacVim1_small.png)](https://github.com/mutewinter/dot_vim/raw/master/screenshots/MacVim1.png) [![Windows gVim](https://github.com/mutewinter/dot_vim/raw/master/screenshots/Windows1_small.png)](https://github.com/mutewinter/dot_vim/raw/master/screenshots/Windows1.png)

## Requirements

**Mac**

* [MacVim](https://github.com/b4winckler/macvim) - I'm currently using
[snapshot 65](https://github.com/b4winckler/macvim/downloads) on Mountain Lion.

**Windows**

* [gVim](http://www.vim.org/download.php#pc) - I'm using [Wu
Yongwei's](http://wyw.dcweb.cn) pre-compiled [gVim
7.3.333](http://wyw.dcweb.cn/download.asp?path=vim&file=gvim73.zip) because it
has Ruby support and the latest patches.

## Mappings

* Typing `jk` insert mode is equivalent to `Escape`.
* Pressing `enter` in normal mode saves the current buffer.

And many more. See [`mappings.vim`](mappings.vim) and
[`plugin_config.vim`](plugin_config.vim) for more.

## Notes

Be sure to always edit the vimrc using `,v`, which opens the vimrc in the
`.vim` folder. Vim has a nasty habit of overriding symlinks.

## Plugin Installation / Requirements

Here's a list of plugins that require further installation or have
dependencies.

* [Fugitive](https://github.com/tpope/vim-fugitive) Requires Git to be
  installed.
* [syntastic](https://github.com/scrooloose/syntastic) Requires many different
  binaries installed depending on what filetypes you want it to check. See the
  [FAQ](https://github.com/scrooloose/syntastic#faq) for more information.
* [Ag.vim](https://github.com/rking/ag.vim) Requires
  [The Silver Searcher](https://github.com/ggreer/the_silver_searcher) to be
  installed.
* [Source Code for Powerline](http://git.io/H3fYBg) The custom font I'm using
  for vim-airline.
* [CtrlP C Matching Extension](https://github.com/JazzCore/ctrlp-cmatcher)
  requires compilation. See the steps [in its
  readme](https://github.com/JazzCore/ctrlp-cmatcher).
* [underscore-cli](https://github.com/ddopson/underscore-cli) for sweet JSON
  formatting.

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/mutewinter/dot_vim/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

## Plugin List

_Note: Auto generated by `rake plugins:update_readme`_


 * [vundle](https://github.com/gmarik/vundle) - Vundle, the plug-in manager for Vim
 * [ZoomWin](https://github.com/vim-scripts/ZoomWin) - Zoom in/out  of windows (toggle between one window and multi-window)
 * [vim-space](https://github.com/christoomey/vim-space) - space.vim - Smart Space key for Vim
 * [ctrlp.vim](https://github.com/kien/ctrlp.vim) - Fuzzy file, buffer, mru, tag, etc finder.
 * [ctrlp-cmatcher](https://github.com/JazzCore/ctrlp-cmatcher) - CtrlP C matching extension
 * [vim-indent-guides](https://github.com/nathanaelkane/vim-indent-guides) - A Vim plugin for visually displaying indent levels in code
 * [vim-airline](https://github.com/bling/vim-airline) - lean & mean statusline for vim that's light as air
 * [nerdtree](https://github.com/scrooloose/nerdtree) - A tree explorer plugin for vim.
 * [colorv.vim](https://github.com/Rykka/colorv.vim) - A powerful color tool.
 * [jellybeans.vim](https://github.com/nanotech/jellybeans.vim) - A colorful, dark color scheme for Vim.
 * [vim-signify](https://github.com/mhinz/vim-signify) - A plugin that shows a diff via Vim's sign column.
 * [vim-startify](https://github.com/mhinz/vim-startify) - A fancy start screen for Vim.
 * [undotree](https://github.com/mbbill/undotree) - Display your undo history in a graph.
 * [vim-togglecursor](https://github.com/jszakmeister/vim-togglecursor) - Toggle the cursor shape in the terminal for Vim.
 * [tcomment_vim](https://github.com/tomtom/tcomment_vim) - An extensible & universal comment vim-plugin that also handles embedded filetypes
 * [vim-surround](https://github.com/tpope/vim-surround) - surround.vim: quoting/parenthesizing made simple
 * [vim-fugitive](https://github.com/tpope/vim-fugitive) - fugitive.vim: a Git wrapper so awesome, it should be illegal
 * [tabular](https://github.com/godlygeek/tabular) - Vim script for text filtering and alignment
 * [ag.vim](https://github.com/rking/ag.vim) - Vim plugin for the_silver_searcher, 'ag', a replacement for the Perl module / CLI script 'ack'
 * [vim-togglelist](https://github.com/milkypostman/vim-togglelist) - Functions to toggle the [Location List] and the [Quickfix List] windows.
 * [swap-parameters](https://github.com/mutewinter/swap-parameters) - Swap parameters of a function or a comma separated list with a single command.
 * [vim-abolish](https://github.com/tpope/vim-abolish) - abolish.vim: easily search for, substitute, and abbreviate multiple variants of a word
 * [scratch.vim](https://github.com/vim-scripts/scratch.vim) - Plugin to create and use a scratch Vim buffer
 * [emmet-vim](https://github.com/mattn/emmet-vim) - emmet for vim: http://emmet.io/
 * [GIFL](https://github.com/mutewinter/GIFL) - Add "wrap terms in google I'm feeling lucky url" à la Textmate
 * [switch.vim](https://github.com/AndrewRadev/switch.vim) - A simple Vim plugin to switch segments of text with predefined replacements
 * [vim-eunuch](https://github.com/tpope/vim-eunuch) - eunuch.vim: helpers for UNIX
 * [vim-marked](https://github.com/itspriddle/vim-marked) - Open the current Markdown buffer in Marked.app
 * [UnconditionalPaste](https://github.com/mutewinter/UnconditionalPaste) - A clone of UnconditionalPaste from http://www.vim.org/scripts/script.php?script_id=3355 since it's not updated on GitHub yet.
 * [HelpClose](https://github.com/vim-scripts/HelpClose) - Close all help windows
 * [gist-vim](https://github.com/mattn/gist-vim) - vimscript for gist
 * [vim-visual-star-search](https://github.com/nelstrom/vim-visual-star-search) - Start a * or # search from a visual block
 * [Join](https://github.com/sk1418/Join) - a better (hopefully) :Join command in vim
 * [ultisnips](https://github.com/SirVer/ultisnips) - Official Mirror of UltiSnips trunk on LaunchPad. Send pull requests to SirVer/ultisnips!
 * [vim-voogle](https://github.com/g3orge/vim-voogle) - google word under the cursor to a browser because 2013
 * [vimux](https://github.com/benmills/vimux) - vim plugin to interact with tmux
 * [vim-turbux](https://github.com/jgdavey/vim-turbux) - Turbo Ruby testing with tmux
 * [vim-ruby-refactoring](https://github.com/ecomba/vim-ruby-refactoring) - Refactoring tool for Ruby in vim!
 * [IndexedSearch](https://github.com/vim-scripts/IndexedSearch) - shows  'Nth match out of M'  at every search (index of match+total # matches)
 * [vim-session](https://github.com/xolox/vim-session) - Extended session management for Vim (:mksession on steroids)
 * [delimitMate](https://github.com/Raimondi/delimitMate) - Vim plugin, provides insert mode auto-completion for quotes, parens, brackets, etc.
 * [syntastic](https://github.com/scrooloose/syntastic) - Syntax checking hacks for vim
 * [supertab](https://github.com/ervandew/supertab) - Perform all your vim insert mode completions with Tab
 * [MatchTagAlways](https://github.com/Valloric/MatchTagAlways) - A Vim plugin that always highlights the enclosing html/xml tags
 * [YouCompleteMe](https://github.com/Valloric/YouCompleteMe) - A code-completion engine for Vim
 * [vim-autoreadwatch](https://github.com/kballenegger/vim-autoreadwatch) - A forked script for vim auto reloading of buffers when changed on disk.
 * [vim-ruby](https://github.com/vim-ruby/vim-ruby) - Vim/Ruby Configuration Files
 * [vim-haml](https://github.com/tpope/vim-haml) - Vim runtime files for Haml, Sass, and SCSS
 * [vim-rails](https://github.com/tpope/vim-rails) - rails.vim: Ruby on Rails power tools
 * [vim-rake](https://github.com/tpope/vim-rake) - rake.vim: it's like rails.vim without the rails
 * [vim-bundler](https://github.com/tpope/vim-bundler) - bundler.vim: Lightweight support for Ruby's Bundler
 * [vim-javascript](https://github.com/pangloss/vim-javascript) - Vastly improved Javascript indentation and syntax support in Vim.
 * [vim-coffee-script](https://github.com/kchmck/vim-coffee-script) - CoffeeScript support for vim
 * [vim-json](https://github.com/leshill/vim-json) - Syntax highlighting for JSON in Vim
 * [vim-handlebars](https://github.com/nono/vim-handlebars) - Vim plugin for Handlebars
 * [html5.vim](https://github.com/othree/html5.vim) - HTML5 omnicomplete and syntax
 * [indenthtml.vim](https://github.com/vim-scripts/indenthtml.vim) - alternative html indent script
 * [tomdoc.vim](https://github.com/mutewinter/tomdoc.vim) - A simple syntax add-on for vim that highlights your TomDoc comments.
 * [vim-tomdoc](https://github.com/jc00ke/vim-tomdoc) - Simple vim plugin that adds TomDoc templates to your code.
 * [cocoa.vim](https://github.com/msanders/cocoa.vim) - Vim plugin for Cocoa/Objective-C development.
 * [taskpaper.vim](https://github.com/mutewinter/taskpaper.vim) - This package contains a syntax file and a file-type plugin for the simple format used by the TaskPaper application.
 * [nginx.vim](https://github.com/mutewinter/nginx.vim) - Syntax highlighting for nginx.conf and related config files.
 * [textile.vim](https://github.com/timcharper/textile.vim) - Textile for VIM
 * [vim-css3-syntax](https://github.com/mutewinter/vim-css3-syntax) - Add CSS3 syntax support to vim's built-in `syntax/css.vim`.
 * [vim-tmux](https://github.com/mutewinter/vim-tmux) - http://tmux.svn.sourceforge.net/viewvc/tmux/trunk/examples/tmux.vim?view=log
 * [vim-markdown](https://github.com/plasticboy/vim-markdown) - Markdown Vim Mode
 * [vim-less](https://github.com/groenewege/vim-less) - vim syntax for LESS (dynamic CSS)
 * [vim-stylus](https://github.com/wavded/vim-stylus) - Syntax Highlighting for Stylus
 * [vim-cucumber](https://github.com/tpope/vim-cucumber) - Vim Cucumber runtime files
 * [csv.vim](https://github.com/chrisbra/csv.vim) - A Filetype plugin for csv files
 * [matchit.zip](https://github.com/vim-scripts/matchit.zip) - extended % matching for HTML, LaTeX, and many other languages
 * [vim-textobj-user](https://github.com/kana/vim-textobj-user) - Vim plugin: Create your own text objects
 * [vim-textobj-rubyblock](https://github.com/nelstrom/vim-textobj-rubyblock) - A custom text object for selecting ruby blocks.
 * [L9](https://github.com/vim-scripts/L9) - Vim-script library
 * [vim-repeat](https://github.com/tpope/vim-repeat) - repeat.vim: enable repeating supported plugin maps with "."
 * [webapi-vim](https://github.com/mattn/webapi-vim) - vim interface to Web API
 * [vim-misc](https://github.com/xolox/vim-misc) - Miscellaneous auto-load Vim scripts

_That's 77 plugins, holy crap._