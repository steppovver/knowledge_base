`tmux` -- create new session
`tmux new -s <name>` -- create with naming
`tmux ls` -- list all sessions
`tmux attach` -- attach to most recent session
`tmux attach` -- shortcut for attach
`tmux attach -t <name>` -- attach session with name


## Default settings

**`ctrl + b` by default** **-- PREFIX**
+ `<prefix> s` -- list all sessions
+ `<prefix> w` -- list all sessions with preview

### Windows

+ `<prefix> c` -- create new window
+ `<prefix> 0` -- switch between windows (0, 1, 2)
+ `<prefix> n` -- cycle through windows (next)
+ `<prefix> p` -- cycle through windows (previous)
+ `<prefix> &` -- close current window
**Custom**
+ `shift+alt+l` -- cycle between windows
+ `shift+alt+h` -- cycle between windows
**Yanky**
`<prefix> [` -- enter copy mode
in those mode
+ `V` -- to insert selection mode
+ `Y` -- to yanky mde
### Panes

+ `<prefix> %` -- split horizontally
+ `<prefix> "` -- split vertically
+ `<prefix> ←↑→↓` -- navigate between panes
+ `<prefix> {}` -- switch panes between each other
+  `<prefix> q then 0` -- switch by number firstly from up to down then by every column
+ `<prefix> z` -- zoom into pane 
+ `<prefix> x` -- close pane

### Sessions

+ 

### Commands

**`<prefix> :` -- enter command mode**

+ `swap-window -s 2 -t 1` -- source and target
+ `new` -- create new session