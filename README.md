# dotfiles
This repository contains my personal configuration files and scripts for optimizing my environment. Includes settings for Bash, ZSH, and more. Easily back up, synchronize, and customize your environment.

## Install Homebrew
Open up a terminal window and install homebrew with the following command:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Add Homebrew To Path
After installing, add it to the path (replace ”[username]” with your actual username):

```bash
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/[username]/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## Install Git
If you don’t have it installed, install git as well:

```bash
brew install git
```

## Install Oh My Zsh
Run this to install Oh My Zsh:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Install ZSH Plugins
Install zsh-autosuggestions:

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

Install zsh-syntax-highlighting:

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

Load these new plugins by running:

```bash
source ~/.zshrc
```

## Install Kiro
Run this to install Kiro:

```bash
brew install kiro-cli
```

## Install JetBrainsMono Nerd Font
Install the font using homebrew:

```bash
brew install --cask font-jetbrains-mono-nerd-font
```

## Configure Terminal
Configure Terminal to use Clear Dark Theme, font Jet Brains Nerd and size 18

## Install Stow
If you don’t have it installed, install stow as well:

```bash
brew install stow
```

## Usage of Stow and Dotfiles
To use this repository, simply clone it to your local machine. 

```bash
git clone https://github.com/ofabbarros/dotfiles.git
```

Once cloned, navigate to the desired directory.

```bash
cd dotfiles
```

Run stow to install the dotfiles.

```bash
stow .
```

You are now ready to use the dotfiles in your environment.

## References
[How To Easily Manage Your Dotfiles With GNU Stow](https://www.josean.com/posts/how-to-manage-dotfiles-with-gnu-stow)
[How To Setup Your Mac Terminal](https://www.josean.com/posts/terminal-setup)
