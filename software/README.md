# ALL
### Oh My Zsh https://github.com/robbyrussell/oh-my-zsh

**installation**
zsh  
https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH  
ubuntu issue with `chsh -s $(which zsh)`    
http://unix.stackexchange.com/questions/111365/how-to-change-default-shell-to-zsh-chsh-says-invalid-shell
`sudo chsh -s "$(command -v zsh)" "${USER}"`

via curl  
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
via wget   
`sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"`

numpad issue   
http://vim.wikia.com/wiki/PuTTY_numeric_keypad_mappings  
Run PuTTY Configuration.  
In the left pane, select Terminal, Features.  
Put a check mark next to "Disable application keypad mode".  
In the left pane, select Session.  
Save the settings.  

http://superuser.com/questions/742171/zsh-z-shell-numpad-numlock-doesnt-work

ohmyzsh plugins
**dirhistory**  
CTRL+ALT-LEFT/RIGHT works instead of ALT-LEFT/RIGHT in putty on windows

**per-directory-history**   
CTRL+G switching between using local/global history


# Windows
## cmder
prompt format in `cmder\vendor\init.bat`

    @prompt $d$s$t $E[1;32;40m$P$S{git}{hg}$S$_$E[1;30;40m{lamb}$S$E[0m

# Mac OS

# Linux

# FreeBSD
