Use this command to install a patched version of Vim:

    brew install nelstrom/homebrew-vim/vim

This formula is based on [the standard Homebrew formula][formula] for Vim, but it has been modified to include a [patch][] that adds a few new commands: `:cdo`, `:cfdo`, `:ldo`, and `:lfdo`.

Check out the talk I gave at Vim London: [Meet the :cdo and :cfdo commands][video]

[patch]: https://groups.google.com/d/msg/vim_dev/dfyt-G6SMec/fYjv0Afq1l4J
[formula]: https://github.com/Homebrew/homebrew/blob/master/Library/Formula/vim.rb
[video]: https://vimeo.com/132367070
