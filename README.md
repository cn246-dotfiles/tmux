## Tmux Dotfiles
My tmux configuration is loosely based off of my `.screenrc` as I've used GNU Screen for many years prior.

I like to keep custom configuration minimal so I can still use tmux reliably when connecting to remote servers without my configuration files.

----

### Key Bindings
#### Prefix
I changed the prefix to `Ctrl a` and configured vim movement keys for navigating panes.

I like having the prefix set to `Ctrl a` on my workstations and `Ctrl b` on servers.
This makes it easier for me to issue tmux commands per session.

#### Other non-default bindings
- Exit tmux with `Ctrl+a \`.
- Close a window with `Ctrl+a K`.
- Use `Ctrl+a Ctrl+a` to toggle between last used windows.
- Split window vertically (side by side) with `Ctrl+a |`.
- Split window horizontally (top and bottom) with `Ctrl+a S`.
- Use `Ctrl+a [h,j,k,l]` to navigate panes (splits).
- Copy mode uses vi keys.
  - Start visual selection of characters with **v**.
  - Yank (copy) selections with **y**.

### Status Bar
The status bar is fairly basic which looks like this (but with color):
```
[ <hostname> | <ip_address> ][               (0:zsh-Z) (1*zsh*)  2:zsh-               ][ Sun Mar-17 |  9:22AM ]
```

The active window indicator is also bold.
