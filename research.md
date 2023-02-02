# Academic Research tools

## Surfdrive - Owncloud
https://owncloud.com/desktop-app/#linux
https://download.owncloud.com/desktop/ownCloud/stable/latest/linux/download/

Server Address: https://surfdrive.surf.nl/files


## Zotero
```
wget -qO- https://github.com/retorquere/zotero-deb/releases/download/apt-get/install.sh | sudo bash
sudo apt-get update
sudo apt-get install zotero
```

### better bibtex plugin
Manage citation keys and quick copy latex citation, such that you don't have to wait for the overleaf sync. 

- Zotero > Preferences > Better BibteX
    - Citation keys
        - [auth:lower]_[shorttitle1_0]_[year]
    - QuickCopy format
        - Latex citation
    - LaTeX command cite


### Zotfile plugin
Configure to save pdf's to surfdrive folder, renaming of pdf's.

- Tools > Zotfile preferences
    - General Settings
        - Custom Location: cloud folder `/Users/jetze/surfdrive/phd_jetze/literature`
        - Use subfolder defined by `/%c`
    - Renaming Rules
        - Format for all Item Types: `{%a} ({%y}) {%t}`
        - Max nr of authors: 1

### Zutilo plugin
Relocate attachments (e.g. after (re)installation).

- Tools > Zutilo preferences
    - Modify attachments

Usage: select all > right click > zutilo > modify attachment paths


### Webplugin
https://www.zotero.org/download/

## Zsh
https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH

### Oh My Zsh
https://github.com/ohmyzsh/ohmyzsh

# Mac
## LaTeX
Install MacTex: https://tug.org/mactex/

Install TexStudio: https://www.texstudio.org/

### BibLaTeX
When using BibLaTeX, change default compiler from `PdfLaTeX` to `latexmk`

### TODO
- Check git integration of TexStudio: https://christianliebel.com/2015/11/setting-up-texstudio-on-mac-os-x-10-11-el-capitan/
