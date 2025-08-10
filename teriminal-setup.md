## 🖥️ Terminal Installation

### 1. Download iTerm2

Get the latest version from [iterm2.com/downloads.html](https://iterm2.com/downloads.html).

### 2. Set iTerm2 as Default Terminal

- Open **iTerm2**.
- Go to `iTerm2` > `Make iTerm2 Default Term`.

---

## 🍺 Brew Package Manager Installation

### 1. Install Homebrew

Paste the following command into **iTerm2** or any terminal:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### 2. Verify Installation

Check if Homebrew was installed successfully:

```sh
brew --version
```

---

> 💡 **Tip:** Restart your terminal after installation for best results.

---

### 3. Install a Nerd Font

- Download your preferred Nerd Font from the [Nerd Fonts website](https://www.nerdfonts.com/font-downloads).
- For example, I chose **JetBrains Mono**. After downloading, extract the ZIP file, open any regular font file, and click "Install".
- To use the new font in iTerm2: go to `iTerm2 Settings` > `Profiles` > `Text`, then change the font from Monaco (default) to your installed Nerd Font.

### 4. Configure VS Code Terminal to Use Nerd Font

- Press `CMD + Shift + P` and search for `Preferences: Open User Settings (JSON)` to open your settings file.
- Add the following line to your `settings.json` to set the terminal font:

```json
{
  "terminal.integrated.fontFamily": "<Your Nerd Font Name>"
}
```

---

> 💡 Tip: If you’re unsure of your Nerd Font’s name, check iTerm2 settings under `Profiles > Text` to find the exact font name you’re using.

---

### 5. Enhance Your Terminal with Oh My Zsh and Powerlevel10k

Oh My Zsh is a powerful framework for managing your Zsh configuration, making your terminal more efficient and customizable. Powerlevel10k is a fast, flexible theme for Zsh that lets you personalize your prompt with useful information and a beautiful appearance.

To install and configure Oh My Zsh and Powerlevel10k, follow this detailed guide: [Blog](https://dev.to/abdfnx/
oh-my-zsh-powerlevel10k-cool-terminal-1no0)

### 6. Supercharge your terminal with plugins and tools

Enhance your terminal experience by adding powerful plugins and tools. Here are some popular options:

- #### FZF (Command-line Fuzzy Finder)

FZF is a general-purpose command-line fuzzy finder that helps you quickly search and open files, command history, processes, and more. It’s not an Oh My Zsh plugin, but it integrates well with Zsh and other shells.

**Install FZF:**

```sh
brew install fzf
```

After installation, run the following to enable key bindings and auto-completion:

```sh
/opt/homebrew/opt/fzf/install
```

- #### Zsh Autosuggestions

This Oh My Zsh plugin suggests commands as you type, based on your history and completions.

**Install Zsh Autosuggestions:**

```sh
git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

Then add `zsh-autosuggestions` to the `plugins` array in your `.zshrc` file.

- #### Zsh Syntax Highlighting

This plugin provides syntax highlighting for your command line, making it easier to spot errors before running commands.

**Install Zsh Syntax Highlighting:**

```sh
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```

Add `zsh-syntax-highlighting` to the `plugins` array in your `.zshrc` file.

- #### Git Plugin (Oh My Zsh)

Oh My Zsh comes with a built-in Git plugin that provides many helpful aliases and functions for working with Git. You don’t need to install it separately—just add `git` to your plugins array in `.zshrc`.

> 💡 **Tip:** You can combine multiple plugins for a more productive workflow. After adding plugins, restart your terminal or run `source ~/.zshrc` to apply changes.

### 7. Change theme of iTerm2 terminal

You can easily change the appearance of your iTerm2 terminal by switching themes (color schemes). Here’s how:

#### Change Theme (Color Scheme) in iTerm2

1. Open **iTerm2**.
2. Go to `iTerm2` > `Preferences` > `Profiles` > `Colors`.
3. Click on the `Color Presets...` dropdown at the bottom right.
4. Select any built-in theme to instantly apply it.

#### Add a Theme from an Online Gallery

You can find many beautiful iTerm2 color schemes online. One popular gallery is [iTerm2 Color Schemes](https://iterm2colorschemes.com/).

To add a theme from the online gallery:

1. Visit [iTerm2 Color Schemes](https://iterm2colorschemes.com/).
2. Browse and click on a theme you like, then download the `.itermcolors` file.
3. In iTerm2, go to `Preferences` > `Profiles` > `Colors`.
4. Click `Color Presets...` > `Import...` and select the downloaded `.itermcolors` file.
5. After importing, select your new theme from the `Color Presets...` dropdown.

> 💡 **Tip:** Try different themes to find one that suits your style and improves readability.
