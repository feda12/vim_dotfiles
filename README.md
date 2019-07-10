# Ben's Vim Config
### Copied from Braintree's and updated for personal preferences

After cloning this project, you can run the following to link these dotfiles
into your home directory:

    rake

Be warned: this will overwrite any existing .vimrc, .gvimrc or .vim/ files you
have in your home directory.

Uses `vim-plug` to manage bundles. Downloading and setting up the described
plugins requires an extra step:

    vim +:PlugInstall

If you plan on using command-t, you'll need to build the C extension. Make sure
to use the ruby you built vim against:

    rvm use system

To build it, go to the `~/.vim/plugged/command-t/ruby/command-t/ext/command-t` folder and run the following:

- `ruby extconf.rb`
- `make`

Open Vim and check command-t is working using the `\fr` command
