[tmux](http://tmux.sourceforge.net/) is a terminal multiplexer.

- Prefix mapped to Ctrl-A for `screen` users.

New to tmux? [*The Tao of tmux*](https://leanpub.com/the-tao-of-tmux) is
now available on Leanpub and [Amazon Kindle](http://amzn.to/2gPfRhC). Read
and browse the book for [on the
web](https://leanpub.com/the-tao-of-tmux/read).

Want more tmux? Check out the [libtmux](https://github.com/tony/libtmux)
python library for controlling tmux, and load your code projects via
YAML/JSON with [tmuxp](https://github.com/tony/tmuxp).

Installation
------------

Download:

```bash
mkdir -p ~/works  # Or any other directory you like
cd ~/works
git clone https://github.com/ilya-bobyr/tmux-config.git
```

Install:

```bash
cd
ln -s ~/works/tmux-config/.tmux.conf
```

I use [Tmux Plugin Manager (TPM)](https://github.com/tmux-plugins/tpm), so
you'll need to install it as well:

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

Now you can start tmux:

```bash
tmux
```

or, if you want to name your session:

```bash
tmux new-session -s my-main-session
```

And finally, if this is the first time you are using this config, you need
to install TPM plugins, by pressing `<Control + a> <Shift + i>` and waiting
for a second, until you see a "Tmux environment reloaded" message.

Start tmux
----------

To start a session:

`tmux`

If you want to name your session:

`tmux new-session -s project1`

To reattach a previous session:

`tmux attach`

To reload the config file:

`<Control + a> r`

Commands
--------

Our prefix/leader key is `Control + a`. This sequence must be typed before
any tmux shortcut.

* `Control + a` before any command
* `Control + a` then `?` to bring up list of keyboard shortcuts
* `Control + a` then `"` to split window
* `Control + a` then `<Space>` to change pane arrangement
* `Control + a` then `o` to rotate panes
* `Control + a` then `h`, `j`, `k`, `l` to move left, down, up, right. Respectively. (vim hjkl)
* `Control + a` then `;` to go to last panel

Beyond your first window:

* `Control + a` then `c` to create a new window
* `Control + a` then `n` to next window
* `Control + a` then `p` to previous window
* `Control + a` then `[0-9]` move to window number
* `Control + a` then `&` to kill window

More configs / Tools
--------------------

* *Save / Load your tmux workspaces through JSON or YAML* with
  [tmuxp](https://github.com/tony/tmuxp).
* *Clone + Synchronize your git / hg / svn projects through JSON / YAML*
  with [vcspull](https://github.com/tony/vcspull).
* *Modular, Lazy-loading vim configuration* with support for C, C++,
  Python, Go and Javascript with
  [tony/vim-config](https://github.com/tony/vim-config)
* *Modular dot-config example*
  [tony/.dot-config](https://github.com/tony/.dot-config)

Other
-----

* LICENSE: MIT
