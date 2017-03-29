## vim and tmux configuration

### vimrc
I haven't found a good .vimrc yet, but here are some candidates

- https://github.com/samlaudev/ConfigurationFiles
- https://github.com/GoYchen/VIM_TMUX

### tmux.conf

My tmux configuration is [here](.tmux.conf)  
Main features are
- Rebind `Ctrl+b` to `Ctrl+x`
- Enable mouse to select window and panel, resize panel
- Enlarge history to 10000 lines
- Horizontal split: `bind-key v`, Vertical split: `bind-key s`

### How to cooperate vim and tmux 
For unknow reason, vim colortheme may not work in tmux without the following configuration  
(1) In .vimrc
```
se t_Co=256
set term=screen-256color
```
(2) In .bashrc
```
 alias tmux="TERM=screen-256color tmux" 
```
