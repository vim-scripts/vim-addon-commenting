vim-addon-commenting is a simple commenting plugin having enough feature for every day use
==========================================================================================

features:
- \\ for commenting and uncommenting using selection or movement
- pays attention col of cursor so that you can indent at col 0 or indentation
  level
- n\\\ comment n lines 
- prefer simple comemnts (// in C/C++ case) without configuration
- tries to detect commenting based on 'commentstring' and 'comments' options
  simple comment till end of line comment markers

all options see plugin/commentary.vim and commentary#CommentLineRange(..)

If you need a sophisticated full blown commenting plugin try tcomment
which magically even supports commenting JS within PHP code and such.

Installing [repeat.vim](https://github.com/tpope/vim-repeat) will enable 
you to use . to repeat a commenting action

configuration:
--------------

    " Force commenting styles:
    let g:vim_addon_commenting = {'force_filetype_comments': {'php': ['#',''], 'c' : ['/*','*/']}}

why fork?
---------
based on https://github.com/tpope/vim-commentary

Because tpope told me: "cursor indentation level I think is a no, at this point".
Whenever he changes his mind I'll be ready to merge.

related work
------------
See www.vim.org/search.php .. There are many existing plugins. But I feel that
they are hard to support because most of them have many hundreds of lines or
are lacking features I want

Eg a very complete commenting implementation also supporting nested file types is
[tcomment](https://github.com/tomtom/tcomment_vim)

License
-------
Distributable under the same terms as Vim itself.  See `:help license`.
