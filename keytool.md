
generate a key:
```
keytool -genkey -v -keystore keystore.jks -keyalg RSA -keysize 2048 -validity 10000 -alias sign
```

list keys in a keystore:
```
keytool -list -v -keystore keystore.jks
```
