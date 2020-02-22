# OH-My-FISH + FISH + iTerm2 INSTALLATION, CONFIGURATION AND THEME
Installation and template for Oh-My-Fish with iTerm on Mac OS
![alt text](https://github.com/nicolastrote/how-to-configurate-Oh-My-Fish/blob/master/oh-my-fish.png)

Installation and template for oh-my-fish:
 * iTerm2
 * fish
 * oh-my-fish
 * POWERLINE fonts
 * color preset
 
 ## PRELEMINARY: HOMEBREW INSTALLATION
Brew is a package manager for OSX

```/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```

```brew -v```

or if you have already brew installed

```$ brew update```

## INSTALLATION FONT POWERLINE-FONTS

```git clone https://github.com/powerline/fonts.git --depth=1```

```cd fonts```

```./install.sh```

## INSTALLATION ITERM2

```brew install iterm```

 * Go in preferences > Profiles > Text > font : Ubuntu for powerline font
 * Download: https://raw.githubusercontent.com/MartinSeeler/iterm2-material-design/master/material-design-colors.itermcolors
 * Save as file material-design-colors.itermcolors
 * Go in preferences > Profiles > Colors > Import in colors presets the file and select it by his name
  

## INSTALLATION FISH

```brew install fish```

## INSTALLATION OH-MY-FISH
You can get started right away with the default setup by running this in your terminal:

```curl -L https://get.oh-my.fish | fish```

This will download the installer script and start the installation.

Oh My Fish includes a small utility omf to fetch and install new packages and themes.

```omf install agnoster & omf reload```

In order to see all available themes, do:

```omf theme```

## LAUNCHING FISH AT EACH START OF ITERM
to make fish your default shell, add the line **/usr/local/bin/fish** at the very top of /etc/shells file :

```sudo nano /etc/shells```

and execute 

```chsh -s /usr/local/bin/fish```

## REINSTALLATION

```curl -L https://get.oh-my.fish > install```

```fish install --path=~/.local/share/omf --config=~/.config/omf```

Enjoy :)

