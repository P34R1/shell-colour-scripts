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

## Nixos Example
To move the dotfiles when you rebuild I personally use [config.lib.file.mkOutOfStoreSymlink](https://github.com/P34R1/nixos/blob/79fc56146c7c1399cd4fef32d84ce67465bd7536/main/home.nix#L85)

To make home-manager set your fish greeting I use [programs.fish.interactiveShellInit](https://github.com/P34R1/nixos/blob/79fc56146c7c1399cd4fef32d84ce67465bd7536/config/fish.nix#L32-L37)
