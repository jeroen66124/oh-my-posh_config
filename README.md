***Installation***
1. in the **iTerm2** menu bar options, execute the ***Install Shell Integration***
2. `brew install jandedobbeleer/oh-my-posh/oh-my-posh`
3. `brew update && brew upgrade oh-my-posh`
4. `brew update && brew upgrade && exec zsh`
5. `oh-my-posh font install meslo`
6. Setup iTerm2 to use ***MesloLGL Nerd Font Mono*** by going to ***Settings > Profiles > Text***
7. Add the following snippet to `~/.zshrc`:

`
if [ "$TERM_PROGRAM" != "Apple_Terminal" ]; then
eval "$(oh-my-posh init zsh --config 'https://raw.githubusercontent.com/jeroen66124/oh-my-posh-config/refs/heads/main/config.json')"
fi
test -e "${HOME}/.iterm2_shell_integration.zsh" && source "${HOME}/.iterm2_shell_integration.zsh"
`
