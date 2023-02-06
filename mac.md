- [Homebrew](https://brew.sh/)
  - /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
- [Rectangle]([https://www.spectacleapp.com/](https://rectangleapp.com/)
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
- VS Code
  - `brew install --cask visual-studio-code`
- 

# Python
- pyenv
- pipx
- virtualenv
  - `pipx install virtualenv`
- httpie
- pip install httpie


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


