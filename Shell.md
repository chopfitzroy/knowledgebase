### Emulators
There are numerous emulators to choose from, my preference is [WezTerm](https://wezfurlong.org/wezterm/) simply because it is cross platform and works well with [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).

### Setting up a shell prompt
I tend to use [Starship](https://starship.rs/) to quickly configure my shell prompt however manual shell prompts can be configured using the [`PS1`](https://www.warp.dev/blog/whats-so-special-about-ps1) value.

### Setting window and tab titles
This varies from system to system as well as from emulator to emulator. An example of this is macOS automatically setting the tab title to be either the shell name or process name.

You can usually set your tab title via your emulator, however if you want a solution that works cross shell you are better off setting up `preexec` and `precmd` functions for your shell using [escapes sequences](https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797). Starship has extensive [documentation](https://starship.rs/advanced-config) explaining how this works with various shell environments.

There are also other advantages to this approach including the fact that it [works with remote connections](https://github.com/wez/wezterm/discussions/1421).

