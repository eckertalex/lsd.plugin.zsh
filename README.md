# lsd.plugin.zsh

> A lsd aliases plugin for zsh

## Installation

### Znap

I recommend using [Znap](https://github.com/marlonrichert/zsh-snap) or installing the plugin manually. You can also install it using any 3rd-party framework or plugin manager you like, but I won't document that here.

Just add this to your .zshrc file:

`znap source eckertalex/lsd.plugin.zsh`

To update, run `znap pull`.

### Oh My Zsh

1. Clone the repository:

   `git clone --depth=1 https://github.com/eckertalex/lsd.plugin.zsh.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/lsd`

2. Include it in your `~/.zshrc`

   `plugins=(... lsd)`

## Aliases

| Alias | Command                                                                     |
| ----- | --------------------------------------------------------------------------- |
| `ls`  | `lsd --classify`                                                            |
| `ll`  | `lsd --classify --header --long`                                            |
| `la`  | `lsd --classify --header --long --almost-all`                               |
| `lC`  | `lsd --classify --header --long --almost-all --sort time --group-dirs none` |
| `lS`  | `lsd --classify --header --long --almost-all --sort size --group-dirs none` |
| `lt`  | `lsd --tree --depth=2`                                                      |

## Changelog

### 2023-04-24

- Initial commit
