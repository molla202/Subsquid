
### sıfırdan kurucaksanız
```
sudo apt-get update && sudo apt install jq git && sudo apt install apt-transport-https ca-certificates curl software-properties-common -y && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" && sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin && sudo apt-get install docker-compose-plugin 
```
```
sudo npm install -g npm@10.1.0
```
```
curl -sL https://deb.nodesource.com/setup_20.x | sudo -E bash -
```
```
sudo apt-get install -y nodejs
```

```
mkdir ~/global-node-packages
```
```
npm config set prefix ~/global-node-packages
```
```
export PATH="${HOME}/global-node-packages/bin:$PATH"
```
```
npm install --global @subsquid/cli@latest
```
```
sqd --version
```
Not: `@subsquid/cli/2.5.0 linux-x64 node-v20.5.1`  bu şekilde çıktı almamız gerekiyor.
```
sqd init my-snapshot-squid -t https://github.com/subsquid-quests/snapshot-squid
```
```
cd my-snapshot-squid
```
Not: `my-snapshot-squid/query-gateway/keys`  içine indirdiğiniz dosyayı atınız.
```
sqd up
```
```
npm ci
sqd build
sqd migration:apply
```
```
sqd run .
```
Not: bitince puanı claim edince `sqd down` diyoruz...
