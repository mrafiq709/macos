# macos
cmd command
```
brew upgrade
brew reinstall php
brew services restart php
brew services list
brew unlink php
brew link php@7.3

mysql.server stop
brew services start mysql
brew services restart mysql

brew services cleanup

To have launchd start mysql at login:
    ln -sfv /usr/local/opt/mysql/*.plist ~/Library/LaunchAgents
Then to load mysql now:
    launchctl load ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
Or, if you don't want/need launchctl, you can just run:
    mysql.server start
```
