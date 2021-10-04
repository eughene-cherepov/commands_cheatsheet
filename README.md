# commands_cheatsheet
*Cheatsheet w/ command to mac/terminal/git and so on*

# Commands (mac config)

- Create mac's Dock splitter:
  - `defaults write com.apple.dock persistent-apps -array-add '{tile-data={}; tile-type="spacer-tile";}';killall Dock`
----
- Manage mac's Dock appearing speed:
  - `defaults write com.apple.dock autohide-time-modifier -float 0.15;killall Dock`
----
- Manage mac's Dock' appearing delay:
  - `defaults write com.apple.dock autohide-delay -float 0; killall Dock`
----
- Matrix:
  - `echo -e "\e[1;40m" ; clear ; while :; do echo $LINES $COLUMNS $(( $RANDOM % $COLUMNS)) $(( $RANDOM % 72 )) ;sleep 0.05; done|awk '{ letters="abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789@#$%^&*()"; c=$4; letter=substr(letters,c,1);a[$3]=0;for (x in a) {o=a[x];a[x]=a[x]+1; printf "\033[%s;%sH\033[2;32m%s",o,x,letter; printf "\033[%s;%sH\033[1;37m%s\033[0;0H",a[x],x,letter;if (a[x] >= $1) { a[x]=0; } }}'`

# Useful RN Libraries

- react-native-responsive-screen (hp/wp commands which returns number of pixels)

# Useful RN Commands

- Create Android bundle and create build: (to avoid old build data in APK)
  1. (in project directory) `mkdir android/app/src/main/assets`
  2. `react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res`
  3. `react-native run-android`
----
- List of commands to fix pods issue:

  1) `gem cleanup`
  2) `brew uninstall cocoapods`
  3) `sudo gem uninstall cocoapods`
  4) `sudo gem install cocoapods -v 1.11.2 -n /usr/local/bin`
  5) `sudo gem install cocoapods-user-defined-build-types`
  6) `rm -rf node_modules`
  7) `npm install`
  8) `npm run clean:pod`
ß