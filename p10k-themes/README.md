# P10K Themes

Based on official [p10k official repository](https://github.com/romkatv/powerlevel10k), these are some custom themes based on generic colors.

* Blue
* Orange
* Yellow
* Cyan

## Requirements

You must have installed `zsh shell` and `powerlevel10k` before applying these themes.

## How to use

First, copy one of this custom themes files to `$HOME` and rename to `.p10k.zsh`. That means, remove the color spread. Don't forget that this file must be hidden.

### 1. Automatic configuration
* Use the following command to download and apply the changes remembering change de color theme **blue** | **orange** | **yellow** | **cyan** and the mode **dark** | **light**):
  ```sh
  wget -O $HOME/.p10k.zsh https://aramirol.github.io/custom-resources/p10k-themes/p10k.zsh.white.dark -o /dev/null | source $HOME/.zshrc
  ```

### 2. Manual configuration
* Download the file you want to use:
  ```sh
  wget https://aramirol.github.io/custom-resources/p10k-themes/p10k.zsh.blue.dark
  ```
* Copy source file to your home directory.
  ```sh
  cp p10k.zsh.blue.dark $HOME/.p10k.zsh
  ```
* Reload session settings.
  ```sh
  source $HOME/.zshrc
  ```

## Customizing theme

The only changes I have made are the following variables:

|VARIABLE| VALUE | EXAMPLE
| -- | -- | -- |
| **POWERLEVEL9K_BACKGROUND** | *<<numeric_color_code>>*  | 238 (Grey27)
| **POWERLEVEL9K_OS_ICON_FOREGROUND** | *<<numeric_color_code>>*  | 255 (Grey93)
| **POWERLEVEL9K_DIR_FOREGROUND** | *<<numeric_color_code>>* | 31 (DeepSkyBlue3)
| **POWERLEVEL9K_DIR_SHORTENED_FOREGROUND** | *<<numeric_color_code>>* | 103 (LightSlateGrey)
| **POWERLEVEL9K_DIR_ANCHOR_FOREGROUND** | *<<numeric_color_code>>* | 39 (DeepSkyBlue1)

