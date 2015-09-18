# hub-ci-zsh-plugin
A simple plugin for adding `hub ci-status` to your zsh theme.

# Setup
1. git clone into your `.oh-my-zsh/plugins/hub-ci-status` folder
2. add `hub-ci-status` to your `~/.zshrc` plugins
3. in your `.oh-my-zsh/themes/<yourtheme>` you can have something like this (notice `hub_ci_status` and hub specific vars)
```
PROMPT='$(battery_pct_prompt)%{$fg[blue]%}%~%{$reset_color%}%{$fg[blue]%}$(git_prompt_info) '
RPROMPT='$(hub_ci_status)%{$reset_color%}'

ZSH_THEME_GIT_PROMPT_PREFIX="("
ZSH_THEME_GIT_PROMPT_SUFFIX=")"
ZSH_THEME_GIT_PROMPT_DIRTY="%{$fg[red]%}✗%{$fg[blue]%}"
ZSH_THEME_GIT_PROMPT_CLEAN="%{$fg[green]%}✔%{$fg[blue]%}"
ZSH_THEME_HUB_CI_PROMPT_SUCCESS="%{$fg[green]%}Success ●%{$fg[blue]%}"
ZSH_THEME_HUB_CI_PROMPT_PENDING="%{$fg[yellow]%}Pending ●%{$fg[blue]%}"
ZSH_THEME_HUB_CI_PROMPT_FAIL="%{$fg[red]%}Fail ●%{$fg[blue]%}"
ZSH_THEME_HUB_CI_PROMPT_NO_STATUS=""```
