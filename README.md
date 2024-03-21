# HTTPS
The original idea is from  
https://medium.com/@HereAndBeyond/spring-boot-3-websocket-oauth-2-0-tls-bf479327339f


Generate self-signed certificate with
```
keytool \
  -genkey \
  -alias mycertificate \
  -keyalg RSA \
  -keysize 2048 \
  -sigalg SHA256withRSA \
  -keystore keystore.p12 \
  -storepass mypassword \
  -ext san=dns:localhost
```
1. Answer only What is your first and last name? question. Enter Orcun Colak
2. For all other questions press Enter key
3. Copy the keystore.p12 to src/main/resources