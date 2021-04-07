# Commands cheatsheet
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

# Useful RN Commands

- Create Android bundle and create build: (to avoid old build data in APK)
  1. (in project directory) `mkdir android/app/src/main/assets`
  2. `react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res`
  3. `react-native run-android`
