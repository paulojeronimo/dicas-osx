# Instalação do Homebrew, do Cask e de outros softwares (através deles)

## Instalação do Homebrew

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

* Ref(s):
  * http://brew.sh

## Instalação do Cask

```
brew tap caskroom/cask
```

* Ref(s):
  * http://caskroom.io/
  * https://github.com/caskroom/homebrew-cask/blob/master/USAGE.md

## Instalação de softwares via brew e cask (exemplos)

### Docker

```
brew install docker
```

### Docker Machine

```
brew install docker-machine
```

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

## Listagem do que está instalado

Para gerar uma lista ([brew-list.txt](brew-list.txt)) dos softwares instalados via brew (e cask) execute:

```
curl -sSL https://raw.githubusercontent.com/paulojeronimo/dicas-osx/master/brew-list | bash
```
