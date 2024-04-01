# macos
cmd command
```
brew upgrade
brew reinstall php
brew services restart php
brew services list
brew unlink php
sudo launchctl unload /Library/LaunchDaemons/homebrew.mxcl.php.plist
brew link php@7.3
brew unlink php@8.3 && brew link php@7.3

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
# Multiple JAVA version
See installed JAVA versions
```
ls /Library/Java/JavaVirtualMachines/
```
Open bash profile
```
check which shell: echo $SHELL
new mac: sudo nano ~/.zshrc
old mac: sudo nano ~/.bash_profile

export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-1.8.jdk/Contents/Home
```
