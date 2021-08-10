# alacrittyconfig
alacritty config. I hope it helps someone.

![Screenshot 2021-08-10 at 22 41 02](https://user-images.githubusercontent.com/69175188/128877619-85ab9071-a24e-4401-ac0e-74d4424843b6.png)


## usage 

copy this config file into your alacritty config file.
```
git clone https://github.com/lil-shimon/alacrittyconfig.git
cp alacrittyconfig/alacritty.yml ~/.config/alacritty.yml
```

## warnings

I use alacritty with fish shell, tmux and neovim
so there is some configurations to use those .
In case you want to try this config file, you may have to fix some codes.

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
