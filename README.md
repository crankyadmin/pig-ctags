
### Pig Ctags

First install ctags if you don\'t have it already.

        brew install ctags

Copy the ctags file in the repo to $HOME/.ctags

        cp ctags $HOME/.ctags

Install tagbar (for vim) from https://github.com/majutsushi/tagbar

Then add the below to your vimrc file

        nmap <F8> :TagbarToggle<CR>
        let g:tagbar_type_pig = {
            \ 'ctagstype' : 'pig',
            \ 'kinds' : [
         \ 'a:Alias',
                \ 's:Set',
                \ 'r:REGISTER',
                \ 'd:DEFINE'
         \]
        \}