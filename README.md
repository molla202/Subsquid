


![image](https://github.com/molla202/Subsquid/assets/91562185/dfabafe5-da0a-4ea5-85b9-c695b67626a3)



## Sistem Gereksinimleri
| Bileşenler | Minimum Gereksinimler | 
| ------------ | ------------ |
| CPU |	4|
| RAM	| 8+ GB |
| Storage	| 200 GB SSD |

👉 [Squids Platform](https://app.subsquid.io/squids/)

👉 [Başvuru Formu](https://subsquid.deform.cc/testnetnodeapplication/)

👉 [CoreNode Telegram](https://t.me/corenode)

👉 [CoreNode Twitter](https://twitter.com/corenodehq)


### ⚡ Update ve gereklilikleri kuralum
```
sudo apt update && sudo apt upgrade -y
sudo apt install curl git wget htop tmux build-essential jq make lz4 gcc unzip -y
```

### ⚡ Kurulum

```
apt install npm
```

```
sudo npm install -g npm@10.1.0
```

```
curl -sL https://deb.nodesource.com/setup_20.x | sudo -E bash -
```

```shell
sudo apt-get install -y nodejs
```


👉 https://app.subsquid.io/squids Adresine gidelim

```
npm install -g @subsquid/cli
```
Not: altta cıkan kodu çalıştırınız npm fund

![image](https://github.com/molla202/Subsquid/assets/91562185/ec532781-bb9b-4bc3-a916-b93deb1fc1a5)


👉 Not: sitedeki kodları sırayla giriyoruz. bittikten sonra dashborda geri dönelim.

![image](https://github.com/molla202/Subsquid/assets/91562185/b5307cc0-0e90-44e4-911d-7e9e69755c1d)

![image](https://github.com/molla202/Subsquid/assets/91562185/a051171b-2f6f-4adc-8afa-951d7dd16619)

### ⚡ Hata alanlar yada sitede synced den düşenler için.(bence kendi rpcnizi herhalukarda ekleyin)

![image](https://github.com/molla202/Subsquid/assets/91562185/967020e1-a474-40fb-9db6-f4bc33054711)

![image](https://github.com/molla202/Subsquid/assets/91562185/c6f736f5-1670-41ef-825d-1f6bfd305c40)

👉 Değişiklik yapılacak yer `adınız` yazan yer alta yazıyor. üstede gösterıor

👉 `nano /root/adınız/src/processor.ts`

![image](https://github.com/molla202/Subsquid/assets/91562185/106fcc60-b5cc-445b-aa9c-972baee1a330)


![image](https://github.com/molla202/Subsquid/assets/91562185/576a437e-c260-4453-a3c4-77e351c7543b)

👉 daha sonra rpcmizi eklemeliyiz https://dashboard.alchemy.com/ adresinden ve infra dan eth mainnet rpc açıyoruz https olanı eklıyoruz

![image](https://github.com/molla202/Subsquid/assets/91562185/b4e64181-ccdf-4856-ada2-5f15df1b9140)

👉 daha sonra depoloy işlemini tekrarlamamız gerekiyor. yukarıdaki yerde adınız ve organizasyon adınız nerde yazıyor goruluyor

```
sqd deploy --org isminiz ./isminiz
```

👉 Loglara bakmak için
```
npx sqd squid:logs isminiz@v1 -f
```







