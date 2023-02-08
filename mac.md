- [Homebrew](https://brew.sh/)
  - /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
- [Rectangle](https://rectangleapp.com/)
  - `brew install --cask rectangle`
- [MacDown](https://macdown.uranusjr.com/)
  - `brew install --cask macdown`
- [iTerm2]()
  - `brew install --cask iterm2`
- [Docker]()
  - `brew install --cask docker`
- [Xcode](https://apps.apple.com/us/app/xcode/id497799835?mt=12)
- git
  - `brew install git`
  - git-lfs
    - `brew install git-lfs`
- [Sublime]
  - `brew install --cask sublime-text`
- [VS Code](https://code.visualstudio.com/docs/setup/mac)
  - `brew install --cask visual-studio-code`
- [PyCharm](https://www.jetbrains.com/help/pycharm/installation-guide.html#standalone)
  - Pro: `https://formulae.brew.sh/cask/pycharm`
  - Community: `https://formulae.brew.sh/cask/pycharm-ce`
- [Alfred](https://www.alfredapp.com/)
  - brew install --cask alfred
- [SnippetsLab](https://apps.apple.com/us/app/snippetslab/id1006087419?mt=12)
- tree
  - `brew install tree`
- Postman
  - `brew install --cask postman`
- 1Password
  - `brew install --cask 1password`
  - `brew install --cask 1password-cli`

# Python
- [pyenv](https://github.com/pyenv/pyenv)

```bash
brew update
brew install pyenv
```

- [post install](https://github.com/pyenv/pyenv#set-up-your-shell-environment-for-pyenv)

```
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
```

- pipx
  - `brew install pipx`
  - `pipx ensurepath`
  - post install
```bash
autoload -U bashcompinit
bashcompinit
eval "$(register-python-argcomplete pipx)"
```
- virtualenv
  - `pipx install virtualenv`
- [httpie](https://httpie.io/docs/cli/homebrew)
  - From website: `brew install httpie`
  - From Xcc: `pip install httpie`?


## Pip installs in virtualenv only
If you really want to make sure you never install packages outside of a virtualenv by accident there is an option to explicitly deny this in pip. You can do this by setting the `PIP_REQUIRE_VIRTUALENV` to `true`. I do this in my `~/.bashrc` OR `~/.zshrc` file so that it is automatically set every time I open a terminal. In order to make sure I can still install packages globally if I want, I also added the `gpip` function which will allow it

```
export PIP_REQUIRE_VIRTUALENV=true

gpip() {
    PIP_REQUIRE_VIRTUALENV="" pip "$@"
}

gpip3() {
    PIP_REQUIRE_VIRTUALENV="" pip3 "$@"
}
```


