# p10k Themes

Based on official [p10k repository](https://github.com/romkatv/powerlevel10k), these are some custom themes based on generic colors.

* Blue
* Orange
* Yellow

## How to use

First, copy one of this custom themes files to `$HOME` and rename to `.p10k.zsh`. That means, remove the color spread. Don't forget that this file must be hidden.

Follow these steps:
* Copy source file to your home directory.
  ```sh
  cp p10k.zsh.blue.dark $HOME/.p10k.zsh
  ```
* Reload session settings.
  ```sh
  . ./.zshrc
  ```

## Customizing theme

The only changes I have made are the following variables:

```sh
  ##################################[ dir: current directory ]##################################
  typeset -g POWERLEVEL9K_DIR_FOREGROUND=<<color_code>>
  typeset -g POWERLEVEL9K_DIR_SHORTENED_FOREGROUND=<<color_code>>
  typeset -g POWERLEVEL9K_DIR_ANCHOR_FOREGROUND=<<color_code>>
```
