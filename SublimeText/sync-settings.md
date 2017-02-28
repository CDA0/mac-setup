# Sync Settings

On the first box:

```
cd ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/
mkdir ~/Dropbox/config/Sublime
mv User ~/Dropbox/config/Sublime/
ln -s ~/Dropbox/config/Sublime/User
```

To link other macs to the same settings:

```
cd ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/
rm -r User
ln -s ~/Dropbox/config/Sublime/User
```



