Node.vim
========
Tools to make Vim superb for developing with Node.js.  
It's the Node equivalent of [Rails.vim (vimscript #1567)](https://github.com/tpope/vim-rails) and [Rake.vim (vimscript #3669)](https://github.com/tpope/vim-rake).

This is just the first release to get the nodes rolling. If you've collected great helpers and shortcuts that help you work with Node, please share them via [email](mailto:andri@dot.ee), [Twitter](https://twitter.com/theml) or [GitHub issues](https://github.com/moll/vim-node/issues) so we could incorporate them here, too! Thanks!

### Tour

- Use `gf` on paths or requires to open the same file Node.js would.
- Use `gf` on `require(".")` to open `./index.js`
- Use `gf` on `require("./dir")` to open `./dir/index.js`
- Use `gf` on `require("./foo")` to open `foo.js`.
- Use `gf` on `require("./package")` and have it open package.json.
- Use `gf` on `require("module")` to open the module's main file (parsed for you from `package.json`).
- Use `gf` on `require("module/lib/utils")` and open files inside the module.
- Automatically sets the filetype to JavaScript for files with Node's shebang (`#!`).
- Use `[I` etc. to look for a keyword in required files (Sets Vim's `&include`).
- Node.vim itself is tested with a thorough automated integration test suite! No cowboy coding here!

Expect more to come soon and feel free to let me know what you're after!


Installing
----------
The easiest and most modular way is to download this to `~/.vim/bundle`:
```
mkdir -p ~/.vim/bundle/node
```

Using Git:
```
git clone https://github.com/moll/vim-node.git ~/.vim/bundle/node
```

Using Wget:
```
wget https://github.com/moll/vim-node/archive/master.tar.gz -O- | tar -xf- --strip-components 1 -C ~/.vim/bundle/node
```

Then prepend that directory to Vim's `&runtimepath` (or use [Pathogen](https://github.com/tpope/vim-pathogen)):
```
set runtimepath^=~/.vim/bundle/node
```


Using
-----
Open any JavaScript file inside a Node project and you're all set.

- Use `gf` on `require()` to jump to source files.
- Use `[I` on any keyword to look for it in the current and required files.


License
-------
Node.vim is released under a *Lesser GNU Affero General Public License*, which in summary means:

- You **can** use this program for **no cost**.
- You **can** use this program for **both personal and commercial reasons**.
- You **do not have to share your own program's code** which uses this program.
- You **have to share modifications** (e.g bug-fixes) you've made to this program.

For more convoluted language, see the `LICENSE` file.


About
-----
**[Andri Möll](http://themoll.com)** authored this in SublemacslipseMate++.  
[Monday Calendar](https://mondayapp.com) supported the engineering work.  

If you find Node.vim needs improving or you've got a question, please don't hesitate to email me anytime at [andri@dot.ee](mailto:andri@dot.ee), tweet at [@theml](https://twitter.com/theml) or [create an issue online](https://github.com/moll/vim-node/issues).
