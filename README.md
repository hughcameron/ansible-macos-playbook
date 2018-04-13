# MacOS


## Installation

### Automated

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/hughcameron/playbook/master/install.sh)"
```

### Manual

```bash
# Install Apple's Command Line Tools
xcode-select --install

# Install Homebrew (see http://brew.sh)
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# Install ansible
brew install ansible

# Clone this repository
https://github.com/hughcameron/playbook.git

# Run the playbook
ansible-playbook main.yml
```


### Variables

If you want to use this playbook for your own computer, fork the repository and
execute `cp vars/defaults.yml vars/${USER}.yml` - you can change any variable
in that file however you like.

### To Do
- [ ] Preferences > Dotfiles aren't working
- [ ] Remove macOS folder at end of init isn't working
- [ ] Fix pyenv dependencies
- [ ] Create `security` function to leverage Keychain
- [ ] Place `git config` commands
- [ ] Setup 1password using cli
- [ ] Install chrome profiles using cli
- [ ] Where did 'font-interface' come from, does it need to be replaced?
- [ ] Re-upload repository on GitHub
- [ ] Add in a software update command
- [ ] Change wallpaper method to AppleScript
- [ ] Create Projects Folder, Assign Icon and Add to Sidebar
- [ ] Don't use diskutil
+ [ ] Pimp up Spotlight and Quicklook (https://github.com/juanbrujo/Talus)
- [ ] Set Slack, Things etc. to Open at Login
- [ ] Sort Desktop by Date Modified
- [ ] Stop creating DS Store Files
- [ ] Symlink atom settings to current settings - /Users/hugh/.atom/
- [ ] View Bluetooth Menu in Toolbar
- [ ] Why does keyboard beep on move line down (Ctrl + Cmd + Down)?
- [ ] Create a 'How To Get Started'
- [X] Add command line developer tools to initilise
- [X] Improve Terminal view readability
- [X] Remove keyboard refresh rate
- [ ] Finder sidebar icons using https://developer.apple.com/library/content/documentation/General/Conceptual/ExtensibilityPG/Finder.html
- [ ] Sweep unused preloaded apps (Mail, Photobooth, Dashboard, Mission Control) into 'Other' Folder
- [ ] Disable Guest Profile
- [ ] Set login screen photo to black
- [ ] Set up Finder shortcut for Projects
- [ ] Remove .DS_Store files
- [ ] Atom dotfile preferences
- [ ] Keep Ansible script awake while running
- [ ] Switch to VS Code
- [ ] Modify VS Code Logo
- [ ] Modify Letterpress (/Applications/Visual Studio Code.app/Contents/Resources/app/resources/letterpress.svg)


## Acknowledgements, Attributions & Appreciations
* https://github.com/jeromegamez/ansible-macos-playbook
* https://github.com/mzdr/macOS
* https://github.com/pathikrit/mac-setup-script
* https://github.com/sb2nov/mac-setup
* https://github.com/JacobDB/git-icon
* https://github.com/geerlingguy/mac-dev-playbook
* https://mths.be/macos
* http://dotfiles.github.io
