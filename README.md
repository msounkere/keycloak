### Create .env file
```
cp env.example .env
```

### If creating a new certificate and key:
```
bash scripts/issue-certificate.sh -d <YOUR_MM_DOMAIN> -o ${PWD}/certs
```
### To include the certificate and key, uncomment the following lines in your .env file and ensure they point to the appropriate files.
```
#CERT_PATH=./certs/etc/letsencrypt/live/${DOMAIN}/fullchain.pem
#KEY_PATH=./certs/etc/letsencrypt/live/${DOMAIN}/privkey.pem
```