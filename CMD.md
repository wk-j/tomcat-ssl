##  Steps

```
docker-compose up
docker-compose down
```

## Create key

```
rm (pwd)/temp/keys/.keystore
keytool -genkey -alias wk-j -keyalg RSA -keystore (pwd)/temp/keys/.keystore -keysize 4096 -validity 720
keytool -genkey -alias wk-j -keyalg RSA -keystore (pwd)/temp/keys/.keystore 


123456
wk-j
y
```

## Create certificate signing request

```
keytool -certreq -keyalg RSA -alias wk-j -file (pwd)/temp/keys/wk-j.csr -keystore (pwd)/temp/keys/.keystore
123456
```

## Install certificate

- ...