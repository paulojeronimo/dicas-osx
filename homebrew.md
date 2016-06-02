# Homebrew, Cask e softwares instalados através deles

## Homebrew

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

* Ref(s):
  * http://brew.sh

### Docker

```
brew install docker
```

### Docker Machine

```
brew install docker-machine
```

## Cask

```
brew tap caskroom/cask
```

* Ref(s):
  * http://caskroom.io/
  * https://github.com/caskroom/homebrew-cask/blob/master/USAGE.md
  * http://www.rocu.de/manage-your-mac-apps-with-homebrew-cask/

### Spectacle

```
brew cask install spectacle
```

### Virtualbox

```
brew cask install virtualbox virtualbox-extension-pack
```

### Vagrant

```
brew cask install vagrant
```

### Java

```
brew cask install java
```

## Obtendo uma lista do que está instalado

```
list=brew-list.txt
> $list
cat > cmds <<'EOF'
brew list
brew cask list
for f in $(brew cask list); do brew cask list $f; done
EOF
cat cmds | while read CMD
do
    echo -e "\n$ $CMD" >> $list
    eval $CMD >> $list
done
rm cmds
```

Minha lista: [brew-list.txt](brew-list.txt)
