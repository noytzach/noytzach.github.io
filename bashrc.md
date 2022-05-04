# .bashrc Cheat sheet
## Prompt
```
PS1='\e[0;34m\w\e[0m\n$ '
```

## History search with arrows
```
bind '"\e[A": history-search-backward'
bind '"\e[B": history-search-forward'
bind '"\eOA": history-search-backward'
bind '"\eOB": history-search-forward'
```

## Let double-click select colon
```
puuid=$(gsettings get org.gnome.Terminal.ProfilesList default | tr -d "'")
gsettings set \
  org.gnome.Terminal.Legacy.Profile:/org/gnome/terminal/legacy/profiles:/:$puuid/ \
  word-char-exceptions '@ms "-=&#:/.?@+~_%;"'
```
