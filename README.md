# Docu-Node.js-Setup
Documentation how to setup Node.js with Debian 11 "bullseye"
https://nodejs.org/ https://www.npmjs.com/ https://deb.nodesource.com/

## Preparation
```
sudo apt update && sudo apt upgrade --show-upgraded
```
```
sudo apt install -y ca-certificates curl gnupg
curl -fsSL https://deb.nodesource.com/gpgkey/nodesource-repo.gpg.key | sudo gpg --dearmor -o /etc/apt/keyrings/nodesource.gpg
NODE_MAJOR=20
echo "deb [signed-by=/etc/apt/keyrings/nodesource.gpg] https://deb.nodesource.com/node_$NODE_MAJOR.x nodistro main" | sudo tee /etc/apt/sources.list.d/nodesource.list
```
## Installation
```
sudo apt update && sudo apt install nodejs -y
```
