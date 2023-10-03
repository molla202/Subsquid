
![image](https://github.com/molla202/Subsquid/assets/91562185/65ba10fe-34d7-48d9-9d90-36515344edbe)


![image](https://github.com/molla202/Subsquid/assets/91562185/e9011ddf-92a3-46e0-8b0c-2c074ef095e6)

👉 👉 👉 Not: sqd run .       = bu kodu screen açarak çalıştırın sona çok sıkıntı oluyor bağlantı kopunca 👉 👉 👉
- öncelikle siteden get key deyip indiriyoruz keyimizi
- daha sonra how to diyoruz
- dökuman zaten hazır ancak sıfır sunucuya kuracaksanız bazı şeyleri kurmamız gerekıyor
- /root/my-quad-proc-squid/query-gateway/ keyler olusturduğumuz my single trible quad dosyalarının içindeki yerlere atıyoruz

# güncelleme ve docker kurulumu
```
sudo apt update -y && sudo apt upgrade -y
for pkg in docker.io docker-doc docker-compose podman-docker containerd runc; do sudo apt-get remove $pkg; done
```
```
sudo apt-get update
sudo apt-get install ca-certificates curl gnupg
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg
```
```
echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
```
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
```
sudo apt update -y && sudo apt upgrade -y
```
- bu kısımda hata alırsanız bir düzenleme lazım

![image](https://github.com/molla202/Subsquid/assets/91562185/e4c8ccf8-f959-4052-ab67-b494ef42999e)

- zaten bunun içinde oluyoruz single duble quad 4 dündede kurunca böle oluyor

cd my-single-proc-squid

- düzenlıyoruz açılan yerde olması gereken resimi bırakıyorum

nano ./commands.json

![image](https://github.com/molla202/Subsquid/assets/91562185/43ce8504-bc4b-490c-8de0-9f05da0f5ded)

- zaten en son başlayınca siteden yüzde artmaya baslar bitince siteden claim edin puanınızı
- eğer eski aquad çalışıyorsa dokcer ps den bakınız durdurunuz ilkini yaptınız puanı aldınız aynı sunucuda 2cisine baslamak için yine docker ps deyip çalışan squadla ilgili dockerları stoplayınızı docker stop docker-id
- sitede yüzde ilerlemesinde sıkıntı var ilerleme hemen gözkmeyebilir takılı kalabilir
- birden fazla sunucuda işlemelri başlatıp loglar akamya baslayınca bırakın kendi haline yyok tek sunucunuz varsa mecbur puanı alıp daha sonrakine geçmeniz gerekıyor.
- sorunuz varsa sorunuz dokumandaki kodlara uyarsanız sıkıntı cıkmıyor. ben sadece bazı sıkıntılardan bahsetmek istedim.


















