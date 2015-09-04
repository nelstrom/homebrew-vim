Use this command to install a patched version of Vim:

    brew install nelstrom/vim/vim --with-cdo

This formula is based on [the standard Homebrew formula][formula] for Vim, but it has been modified to include a [patch][] that adds a few new commands: `:cdo`, `:cfdo`, `:ldo`, and `:lfdo`.

Check out the talk I gave at Vim London: [Meet the :cdo and :cfdo commands][video]

[patch]: https://groups.google.com/d/msg/vim_dev/dfyt-G6SMec/fYjv0Afq1l4J
[formula]: https://github.com/Homebrew/homebrew/blob/master/Library/Formula/vim.rb
[video]: https://vimeo.com/132367070

## What if I've already installed Vim using homebrew?

Uninstall the existing build of Vim:

    brew uninstall vim

Then install the patched version

    brew install nelstrom/vim/vim --with-cdo

When you're finished trying out the patched version of Vim, you can uninstall it and remove the tap by running:

    brew uninstall vim
    brew untap nelstrom/vim

Then install the standard homebrew issue of Vim again as follows:

    brew install vim

Now you're back to where you started.
