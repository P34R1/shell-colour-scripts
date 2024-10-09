# Shell Color Scripts
This is a fork of [DT's color scripts](https://gitlab.com/dwt1/shell-color-scripts/-/tree/master) made for my personal use.

![Screenshot of shell-color-scripts](https://gitlab.com/dwt1/dotfiles/raw/master/.screenshots/dotfiles12.png)

A collection of terminal color scripts I've accumulated over the years.
Included 52 beautiful terminal color scripts.

# Usage
If you manually run any of the scripts with bash it just works. If you want to get a random script use DT's script or to have your [Fish Shell](https://fishshell.com/) automatically run a random prompt put this function in your fish configuration file.

```fish
function fish_greeting
  set DIR_COLORSCRIPTS "myfullpath/colorscripts"
  bash "$DIR_COLORSCRIPTS/$(basename (random choice $(ls $DIR_COLORSCRIPTS)))"
end
```
