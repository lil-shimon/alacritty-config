# alacrittyconfig
alacritty config. It also serves as a backup, but I hope it helps someone.

## usage 

copy this config file into your alacritty config file.
```
git clone https://github.com/lil-shimon/alacrittyconfig.git
cp alacrittyconfig/alacritty.yml ~/.config/alacritty.yml
```

## warnings

I use alacritty with fish shell, tmux and neovim
so there is some configurations to use those .
in case you try this config in your environment, you should fix some codes.

### line 11
program : shell what you use
```
  program: /usr/local/bin/fish
```
### line 12 to 15
if you are not tmux user, delete that
```
  args: 
    - --login
    - --command 
    - "tmux attach || tmux"
```
### line 220
you are not tmux or neovim user, delete it
```
env:
  TERM: alacritty
```
