# Cyclone OS 

[<center><img src="https://i.imgur.com/3PvixWP.png" height="100%" width="100%;"/></center>](https://github.com/Cyclone-OS)

## Download the source code
#### Initialize local repository

```bash
repo init -u https://github.com/Cyclone-OS/manifest.git -b s
```
#### Sync
```
repo sync -c --force-sync --no-tags --no-clone-bundle -j$(nproc --all) --optimized-fetch --prune
```

**Build the rom**
```bash
. build/envsetup.sh
lunch cyclone_$(device)-userdebug
make bacon
```
