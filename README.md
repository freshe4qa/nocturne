<p align="center">
  <img height="100" height="auto" src="https://github.com/freshe4qa/nocturne/assets/85982863/02c5fd26-cea7-4381-93e6-31c7f28996ee">
</p>

# Nocturne — Trusted Setup

Official documentation:
>- [Guide](https://nocturnelabs.notion.site/nocturnelabs/Nocturne-Trusted-Setup-Contributor-Guide-411ac624abdb44d989f3f5be354c91ac)

Explorer:
>- [-](-)

### Minimum Hardware Requirements
 - 2x CPUs; the faster clock speed the better
 - 2GB RAM
 - 20GB of storage (SSD or NVME)

Заходим на сервер через Mobaxterm с такими настройками:

![image](https://github.com/freshe4qa/nocturne/assets/85982863/cd706858-cff1-4a37-b93e-da5a1f5c4932)

```
sudo apt update && sudo apt upgrade -y
```

```
wsl --install
```
```
sudo apt-get upgrade
```
```
sudo apt install curl
```
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
```
```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```
```
nvm install 18.0.0
```
```
npm install -g @nocturne-xyz/nocturne-setup
```
```
nocturne-setup auth
```
```
screen -S nocturne
```
```
nocturne-setup contribute
```
Выйти CTRL + A + D
