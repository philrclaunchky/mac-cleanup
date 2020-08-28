# mac-cleanup

A cleanup script for macOS that runs the following tasks:

* Empty the Trash on All Mounted Volumes and the Main HDD
* Clear System Log Files
* Clear Adobe Cache Files
* Cleanup iOS Applications
* Remove iOS Device Backups
* Cleanup Xcode Derived Data and Archives
* Reset iOS simulators
* Cleanup Homebrew Cache
* Cleanup Any Old Versions of Gems
* Cleanup Dangling Docker Images
* Purge Inactive Memory
* Cleanup pip cache
* Cleanup Pyenv-VirtualEnv Cache
* Cleanup npm Cache
* Cleanup Yarn Cache
* Cleanup Docker Images and Stopped Containers
* Cleanup CocoaPods Cache Files
* Cleanup Google Chrome Cache Files
* Cleanup composer cache
* Cleanup Dropbox cache

## Install Automatically

### Using curl

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/philrclaunchky/mac-cleanup/master/installer.sh)"
```

### Using wget

```bash
sh -c "$(wget https://raw.githubusercontent.com/philrclaunchky/mac-cleanup/master/installer.sh -O -)"
```

## Step by Step Install

1. Download: `curl -o cleanup https://raw.githubusercontent.com/philrclaunchky/mac-cleanup/master/cleanup.sh`
2. Make it executable: `chmod +x cleanup`
3. Move to make it globally usable: `sudo mv cleanup /usr/local/bin/cleanup`

## Update

```bash
curl -fsSL "https://raw.githubusercontent.com/philrclaunchky/mac-cleanup/master/installer.sh" | bash -s update
```

## Uninstall

```bash
curl -fsSL "https://raw.githubusercontent.com/philrclaunchky/mac-cleanup/master/installer.sh" | bash -s uninstall
```

## Usage Options

Help menu:

```
$ cleanup -h

A Mac Cleanup Utility by philrclaunchky
https://github.com/philrclaunchky/mac-cleanup

USAGE:
 cleanup [FLAGS]

FLAGS:
-h,   prints help menu
-n    no brew updates
```

Clean up without homebrew updates:

```
$ cleanup -n
```
