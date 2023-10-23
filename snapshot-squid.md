





mkdir ~/global-node-packages

npm config set prefix ~/global-node-packages

export PATH="${HOME}/global-node-packages/bin:$PATH"

npm install --global @subsquid/cli@latest

sqd --version

Not: `@subsquid/cli/2.5.0 linux-x64 node-v20.5.1`  bu şekilde çıktı almamız gerekiyor.

sqd init my-snapshot-squid -t https://github.com/subsquid-quests/snapshot-squid

cd my-snapshot-squid

Not: `my-snapshot-squid/query-gateway/keys`  içine indirdiğiniz dosyayı atınız.

sqd up

npm ci
sqd build
sqd migration:apply

sqd run .

Not: bitince puanı claim edince `sqd down` diyoruz...
