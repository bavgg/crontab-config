# crontab-config
Crontab config to automatically delete files and folders with exceptions within a certain period of time.

`0 18 * * * find ~ -mindepth 1 -maxdepth 1 \\( ! -name .zsh_history -a ! -name .zcompdump -a ! -name '.zcompdump-plunaden’s MacBook Air-5.9' -a ! -name .Trash -a ! -name .DS_Store -a ! -name Music -a ! -name Pictures -a ! -name .config -a ! -name .local -a ! -name .CFUserTextEncoding -a ! -name .zsh_sessions -a ! -name Library -a ! -name Downloads -a ! -name .docker -a ! -name .zshrc -a ! -name Desktop -a ! -name .p10k.zsh -a ! -name .zprofile -a ! -name .zsh \) \ -exec rm -r {} \;`
