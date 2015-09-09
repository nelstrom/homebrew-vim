## Update!

The cdo patch has now been folded into core Vim as [Patch 858](https://github.com/vim/vim/commit/aa23b379421aa214e6543b06c974594a25799b09) 

I've updated this tap+formula to install Vim 7.4.861 when you run:

    brew install nelstrom/vim/vim

(The instructions below should still work, but you can omit the `--with-cdo`.)

---

## [Original instructions]

Use this command to install a patched version of Vim:

    brew install nelstrom/vim/vim --with-cdo

This formula is based on [the standard Homebrew formula][formula] for Vim, but it has been modified to include a [patch][] that adds a few new commands: `:cdo`, `:cfdo`, `:ldo`, and `:lfdo`.

You can check if the install worked by launching Vim and running `:help :cdo`. If Vim shows you the documentation for that command, you're good!

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

## What's so good about this patch?

I discussed these new features at the Vim London meetup in June 2015.
You can watch the talk on Vimeo: [Meet the :cdo and :cfdo commands][video]

[patch]: https://groups.google.com/d/msg/vim_dev/dfyt-G6SMec/fYjv0Afq1l4J
[formula]: https://github.com/Homebrew/homebrew/blob/master/Library/Formula/vim.rb
[video]: https://vimeo.com/132367070

