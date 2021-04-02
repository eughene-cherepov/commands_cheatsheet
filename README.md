# commands_cheatsheet
*Cheatsheet w/ command to mac/terminal/git and so on*

# Commands (mac config)

- Create mac's Dock splitter:
  - `defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}';killall Dock`

- Manage mac's Dock appearing speed:
  - `defaults write com.apple.dock autohide-time-modifier -float 0.15;killall Dock`

- Manage mac's Dock' appearing delay:
  - `defaults write com.apple.dock autohide-delay -float 0; killall Dock`

# Useful RN Libraries

- react-native-responsive-screen (hp/wp commands which returns number of pixels)