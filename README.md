# The Vim Configuration of Champions

Version 3! Now each plugin is included and managed in its
[own file](vundle_plugins)!

[![iTerm][ss]][ss]

[ss]: https://github.com/mutewinter/dot_vim/raw/master/screenshots/iTerm.png

## Installation

1. `git clone http://github.com/mutewinter/dot_vim.git ~/.vim`.
1. `cd ~/.vim`.

Now you have a choice. The automated script or the manual process.

1. Run `scripts/setup`.

**or**

1. `rake vim:link` to make the `.vimrc` and `.nvimrc` symbolic links.
2. Install [Vundle](https://github.com/gmarik/vundle) with `git clone
   http://github.com/gmarik/vundle.git bundle/vundle`
3. `vim +PluginInstall +qall`

Enjoy enhanced productivity, increased levitation, reduced watermelon-related
accidents, and startling sex appeal.

## Vim Requirements

* [NeoVim](https://github.com/neovim/neovim) or
  [MacVim](https://github.com/b4winckler/macvim) - I'm currently using NeoVim
  [via Homebrew](https://github.com/neovim/neovim/wiki/Installing) on OS X
  Yosemite.

## Plugin Requirements

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

## Mappings

* Typing `jk` insert mode is equivalent to `Escape`.
* Pressing `enter` in normal mode saves the current buffer.

And many more. See [`mappings.vim`](mappings.vim) and
[`vundle_plugins`](vundle_plugins) for more.

## Installing Custom Plugins

Create a new `.vim` file with the same name as the plugin you'd like to install
in [`vundle_plugins/custom`](vundle_plugins/custom). Then add the installation
block. For example:

`vundle_plugins/custom/vim-move.vim`

```viml
if exists('g:vundle_installing_plugins')
  Plugin 'matze/vim-move.vim'
  finish
endif

let g:move_key_modifier = 'C'
```

This example installs [`vim-move`](https://github.com/matze/vim-move).

## Plugin List

| Stars___ | **Plugin** | **Description** |
| -------: | :--------- | :-------------- |
| 5,535 ★ |[vim-fugitive](https://github.com/tpope/vim-fugitive) [:page_facing_up:](vundle_plugins/vim-fugitive.vim)|fugitive.vim: a Git wrapper so awesome, it should be illegal |
| 5,173 ★ |[vim-airline](https://github.com/bling/vim-airline) [:page_facing_up:](vundle_plugins/vim-airline.vim)|lean & mean status/tabline for vim that's light as air |
| 4,977 ★ |[syntastic](https://github.com/scrooloose/syntastic) [:page_facing_up:](vundle_plugins/syntastic.vim)|Syntax checking hacks for vim |
| 4,714 ★ |[nerdtree](https://github.com/scrooloose/nerdtree) [:page_facing_up:](vundle_plugins/nerdtree.vim)|A tree explorer plugin for vim. |
| 4,377 ★ |[ctrlp.vim](https://github.com/kien/ctrlp.vim) [:page_facing_up:](vundle_plugins/ctrlp.vim)|Fuzzy file, buffer, mru, tag, etc finder. |
| 2,882 ★ |[vim-rails](https://github.com/tpope/vim-rails) [:page_facing_up:](vundle_plugins/vim-rails.vim)|rails.vim: Ruby on Rails power tools |
| 2,750 ★ |[vim-surround](https://github.com/tpope/vim-surround) [:page_facing_up:](vundle_plugins/vim-surround.vim)|surround.vim: quoting/parenthesizing made simple |
| 2,512 ★ |[emmet-vim](https://github.com/mattn/emmet-vim)|emmet for vim: http://emmet.io/ |
| 1,604 ★ |[ultisnips](https://github.com/SirVer/ultisnips) [:page_facing_up:](vundle_plugins/ultisnips.vim)|UltiSnips - The ultimate snippet solution for Vim. Send pull requests to SirVer/ultisnips! |
| 1,579 ★ |[vim-coffee-script](https://github.com/kchmck/vim-coffee-script)|CoffeeScript support for vim |
| 1,433 ★ |[supertab](https://github.com/ervandew/supertab)|Perform all your vim insert mode completions with Tab |
| 1,261 ★ |[vim-ruby](https://github.com/vim-ruby/vim-ruby)|Vim/Ruby Configuration Files |
| 1,167 ★ |[vim-javascript](https://github.com/pangloss/vim-javascript)|Vastly improved Javascript indentation and syntax support in Vim. |
| 1,154 ★ |[vim-indent-guides](https://github.com/nathanaelkane/vim-indent-guides) [:page_facing_up:](vundle_plugins/vim-indent-guides.vim)|A Vim plugin for visually displaying indent levels in code |
| 1,056 ★ |[tabular](https://github.com/godlygeek/tabular) [:page_facing_up:](vundle_plugins/tabular.vim)|Vim script for text filtering and alignment |
| 1,048 ★ |[gist-vim](https://github.com/mattn/gist-vim) [:page_facing_up:](vundle_plugins/gist-vim.vim)|vimscript for gist |
| 943 ★ |[vimux](https://github.com/benmills/vimux) [:page_facing_up:](vundle_plugins/vimux.vim)|vim plugin to interact with tmux |
| 861 ★ |[vim-unimpaired](https://github.com/tpope/vim-unimpaired)|unimpaired.vim: pairs of handy bracket mappings |
| 812 ★ |[delimitMate](https://github.com/Raimondi/delimitMate)|Vim plugin, provides insert mode auto-completion for quotes, parens, brackets, etc. |
| 779 ★ |[vim-startify](https://github.com/mhinz/vim-startify) [:page_facing_up:](vundle_plugins/vim-startify.vim)|:rocket: A fancy start screen for Vim. |
| 750 ★ |[ag.vim](https://github.com/rking/ag.vim) [:page_facing_up:](vundle_plugins/ag.vim)|Vim plugin for the_silver_searcher, 'ag', a replacement for the Perl module / CLI script 'ack' |
| 742 ★ |[jellybeans.vim](https://github.com/nanotech/jellybeans.vim) [:page_facing_up:](vundle_plugins/jellybeans.vim)|A colorful, dark color scheme for Vim. |
| 662 ★ |[vim-signify](https://github.com/mhinz/vim-signify) [:page_facing_up:](vundle_plugins/vim-signify.vim)|:rotating_light: Show a diff via Vim sign column. |
| 660 ★ |[vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator) [:page_facing_up:](vundle_plugins/vim-tmux-navigator.vim)|Seamless navigation between tmux panes and vim splits |
| 627 ★ |[vim-repeat](https://github.com/tpope/vim-repeat)|repeat.vim: enable repeating supported plugin maps with "." |
| 566 ★ |[vim-abolish](https://github.com/tpope/vim-abolish)|abolish.vim: easily search for, substitute, and abbreviate multiple variants of a word |
| 552 ★ |[html5.vim](https://github.com/othree/html5.vim)|HTML5 omnicomplete and syntax |
| 527 ★ |[vim-less](https://github.com/groenewege/vim-less)|vim syntax for LESS (dynamic CSS) |
| 516 ★ |[vim-haml](https://github.com/tpope/vim-haml)|Vim runtime files for Haml, Sass, and SCSS |
| 481 ★ |[tcomment_vim](https://github.com/tomtom/tcomment_vim) [:page_facing_up:](vundle_plugins/tcomment_vim.vim)|An extensible & universal comment vim-plugin that also handles embedded filetypes |
| 450 ★ |[vim-jade](https://github.com/digitaltoad/vim-jade)|Vim Jade template engine syntax highlighting and indention |
| 429 ★ |[vim-session](https://github.com/xolox/vim-session) [:page_facing_up:](vundle_plugins/vim-session.vim)|Extended session management for Vim (:mksession on steroids) |
| 413 ★ |[vim-json](https://github.com/elzr/vim-json)|A better JSON for Vim: distinct highlighting of keywords vs values, JSON-specific (non-JS) warnings, quote concealing. Pathogen-friendly. |
| 401 ★ |[vim-ruby-refactoring](https://github.com/ecomba/vim-ruby-refactoring)|Refactoring tool for Ruby in vim! |
| 393 ★ |[vim-endwise](https://github.com/tpope/vim-endwise)|endwise.vim: wisely add "end" in ruby, endfunction/endif/more in vim script, etc |
| 360 ★ |[vim-eunuch](https://github.com/tpope/vim-eunuch)|eunuch.vim: helpers for UNIX |
| 343 ★ |[vim-textobj-user](https://github.com/kana/vim-textobj-user)|Vim plugin: Create your own text objects |
| 304 ★ |[undotree](https://github.com/mbbill/undotree)|The ultimate undo history visualizer for VIM |
| 296 ★ |[vim-css3-syntax](https://github.com/hail2u/vim-css3-syntax)|Add CSS3 syntax support to vim's built-in `syntax/css.vim`. |
| 277 ★ |[vim-cucumber](https://github.com/tpope/vim-cucumber)|Vim Cucumber runtime files |
| 270 ★ |[webapi-vim](https://github.com/mattn/webapi-vim)|vim interface to Web API |
| 233 ★ |[vim-bundler](https://github.com/tpope/vim-bundler)|bundler.vim: Lightweight support for Ruby's Bundler |
| 223 ★ |[vim-textobj-rubyblock](https://github.com/nelstrom/vim-textobj-rubyblock)|A custom text object for selecting ruby blocks. |
| 212 ★ |[vim-stylus](https://github.com/wavded/vim-stylus)|Syntax Highlighting for Stylus |
| 202 ★ |[MatchTagAlways](https://github.com/Valloric/MatchTagAlways) [:page_facing_up:](vundle_plugins/MatchTagAlways.vim)|A Vim plugin that always highlights the enclosing html/xml tags |
| 201 ★ |[cocoa.vim](https://github.com/msanders/cocoa.vim)|Vim plugin for Cocoa/Objective-C development. |
| 200 ★ |[csv.vim](https://github.com/chrisbra/csv.vim)|A Filetype plugin for csv files |
| 195 ★ |[switch.vim](https://github.com/AndrewRadev/switch.vim) [:page_facing_up:](vundle_plugins/switch.vim)|A simple Vim plugin to switch segments of text with predefined replacements |
| 161 ★ |[vim-rake](https://github.com/tpope/vim-rake)|rake.vim: it's like rails.vim without the rails |
| 158 ★ |[vim-turbux](https://github.com/jgdavey/vim-turbux) [:page_facing_up:](vundle_plugins/vim-turbux.vim)|Turbo Ruby testing with tmux |
| 144 ★ |[vim-markdown](https://github.com/gabrielelana/vim-markdown)|Markdown for Vim: a complete environment to create Markdown files with a syntax highlight that don't sucks! |
| 127 ★ |[vim-misc](https://github.com/xolox/vim-misc)|Miscellaneous auto-load Vim scripts |
| 94 ★ |[ZoomWin](https://github.com/vim-scripts/ZoomWin) [:page_facing_up:](vundle_plugins/ZoomWin.vim)|Zoom in/out  of windows (toggle between one window and multi-window) |
| 92 ★ |[ember.vim](https://github.com/dsawardekar/ember.vim) [:page_facing_up:](vundle_plugins/ember.vim)|Vim plugin for the Emberjs frontend framework |
| 89 ★ |[matchit.zip](https://github.com/vim-scripts/matchit.zip)|extended % matching for HTML, LaTeX, and many other languages |
| 87 ★ |[colorv.vim](https://github.com/Rykka/colorv.vim) [:page_facing_up:](vundle_plugins/colorv.vim)|A powerful color tool in vim |
| 85 ★ |[vim-visual-star-search](https://github.com/nelstrom/vim-visual-star-search)|Start a * or # search from a visual block |
| 78 ★ |[vim-handlebars](https://github.com/nono/vim-handlebars)|[deprecated] Vim plugin for Handlebars |
| 68 ★ |[nerdtree-git-plugin](https://github.com/Xuyuanp/nerdtree-git-plugin)|A plugin of NERDTree showing git status |
| 62 ★ |[vim-marked](https://github.com/itspriddle/vim-marked)|Open the current Markdown buffer in Marked.app |
| 57 ★ |[portkey](https://github.com/dsawardekar/portkey) [:page_facing_up:](vundle_plugins/portkey.vim)|Navigate files at the speed of Vim. |
| 55 ★ |[vim-anzu](https://github.com/osyo-manga/vim-anzu) [:page_facing_up:](vundle_plugins/vim-anzu.vim)|Vim search status. |
| 51 ★ |[L9](https://github.com/vim-scripts/L9)|Vim-script library |
| 44 ★ |[textile.vim](https://github.com/timcharper/textile.vim)|Textile for VIM |
| 35 ★ |[Join](https://github.com/sk1418/Join)|a better (hopefully) :Join command in vim |
| 29 ★ |[ListToggle](https://github.com/Valloric/ListToggle) [:page_facing_up:](vundle_plugins/ListToggle.vim)|A vim plugin for toggling the display of the quickfix list and the location-list. |
| 29 ★ |[vim-togglecursor](https://github.com/jszakmeister/vim-togglecursor) [:page_facing_up:](vundle_plugins/vim-togglecursor.vim)|Toggle the cursor shape in the terminal for Vim. |
| 26 ★ |[QFEnter](https://github.com/yssl/QFEnter) [:page_facing_up:](vundle_plugins/QFEnter.vim)|Open a Quickfix item in a window you choose. (Vim plugin) |
| 16 ★ |[scratch.vim](https://github.com/vim-scripts/scratch.vim)|Plugin to create and use a scratch Vim buffer |
| 10 ★ |[vim-voogle](https://github.com/papanikge/vim-voogle) [:page_facing_up:](vundle_plugins/vim-voogle.vim)|google for the word under the cursor to a browser because 2013 |
| 8 ★ |[vim-tomdoc](https://github.com/jc00ke/vim-tomdoc)|Simple vim plugin that adds TomDoc templates to your code. |
| 7 ★ |[indenthtml.vim](https://github.com/vim-scripts/indenthtml.vim) [:page_facing_up:](vundle_plugins/indenthtml.vim)|alternative html indent script |
| 7 ★ |[nginx.vim](https://github.com/mutewinter/nginx.vim)|Syntax highlighting for nginx.conf and related config files. |
| 3 ★ |[YouCompleteMe](https://github.com/blueyed/YouCompleteMe) [:page_facing_up:](vundle_plugins/YouCompleteMe.vim)|A slightly modified fork of YCM: A code-completion engine for Vim |
| 3 ★ |[GIFL](https://github.com/mutewinter/GIFL) [:page_facing_up:](vundle_plugins/GIFL.vim)|Add "wrap terms in google I'm feeling lucky url" à la Textmate |
| 3 ★ |[swap-parameters](https://github.com/mutewinter/swap-parameters)|Swap parameters of a function or a comma separated list with a single command. |
| 2 ★ |[taskpaper.vim](https://github.com/mutewinter/taskpaper.vim)|This package contains a syntax file and a file-type plugin for the simple format used by the TaskPaper application. |
| 1 ★ |[HelpClose](https://github.com/vim-scripts/HelpClose)|Close all help windows |
| 1 ★ |[tomdoc.vim](https://github.com/mutewinter/tomdoc.vim)|A simple syntax add-on for vim that highlights your TomDoc comments. |
| 0 ★ |[vim-tmux](https://github.com/mutewinter/vim-tmux)|http://tmux.svn.sourceforge.net/viewvc/tmux/trunk/examples/tmux.vim?view=log |
| 0 ★ |[vim-autoreadwatch](https://github.com/mutewinter/vim-autoreadwatch)|A forked script for vim auto reloading of buffers when changed on disk. |

_That's 82 plugins, holy crap._

_Generated by `rake update_readme` on 2015/05/29._

