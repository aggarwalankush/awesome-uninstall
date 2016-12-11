# MAC

```bash
launchctl unload ~/Library/LaunchAgents/homebrew.mxcl.mongodb.plist
launchctl remove homebrew.mxcl.mongodb
pkill -f mongod
rm -f ~/Library/LaunchAgents/homebrew.mxcl.mongodb.plist
brew uninstall mongodb
sudo rm -rf /data/db
sudo rm -rf /usr/local/var/mongodb
```

# UBUNTU

```bash
sudo service mongod stop
sudo apt-get purge mongodb*
sudo apt-get autoremove
sudo rm -r /var/log/mongodb
sudo rm -r /var/lib/mongodb
sudo rm /etc/apt/sources.list.d/mongodb.list
```
