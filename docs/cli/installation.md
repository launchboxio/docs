---
sidebar_position: 1
title: Installation
---

## From Github Releases 

Download the appropriate release from https://github.com/launchboxio/launchboxctl/releases 
```shell
tar -xvf launchboxctl_$version_$arch.tar.gz 
sudo chmod +x launchboxctl 
sudo mv launchboxctl /usr/local/bin/
```

## Using `asdf`
```shell
asdf plugin add launchbox 
asdf install launchboxctl latest
asdf global launchboxctl latest
```

## Using `homebrew`

```shell
brew install launchboxctl
```
