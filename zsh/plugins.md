| Plugin            | Description                                                  | Commands                                                     |
| ----------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| autopair          | close brackets                                               |                                                              |
| cargo             | completions for `cargo`                                      |                                                              |
| colored-man-pages |                                                              |                                                              |
| colorize          | Adds syntax highlighting based on file ext.<br>dependency: [Pygments](https://pygments.org/download/) | add `ZSH_COLORIZE_STYLE="colorful"` to .zshrc                |
| command-not-found | suggests packages to install if a called cmd is not found    |                                                              |
| copybuffer        | binds `CTRL+O` shortcut to copy text currently in the cli `$BUFFER`. Useful for when you want to copy a command you just entered so you can `*ahem*` execute another, then paste and execute the first | `CTRL+O`                                                     |
| dnote             | completes [Dnote](https://www.getdnote.com/) commands, also dynamically suggest matching book names | `dnote a(press <TAB> here)`                                  |
| gpg-agent         | starts gpg-agent if not already running                      | ==highly rec for keychain plugin==                           |
| keychain          | sets up and loads credentials for both ssh and gpg connections | Requires some [additional config](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/keychain) |
| npm               | provides npm command completion                              |                                                              |
| pip               | adds completion for pip                                      |                                                              |
| python            | adds aliases for python commands                             | ipython, pyfind, pyclean [dirs], pygrep <text>, pyuserpaths  |
| rust              | completions for `rustc`                                      |                                                              |
| safe-paste        | paste code in CLI without running it                         |                                                              |
| virtualenvwrapper | loads python's [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/) shell tools | [see notes on use](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/virtualenvwrapper) |
| zsh-autocomplete  |                                                              |                                                              |




## Runners up

- [git-extras](https://github.com/tj/git-extras)
- [magic-enter](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/magic-enter)
- [otp](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/otp) - create 1 time pws with oath; key saved in gpg-encrypted file

