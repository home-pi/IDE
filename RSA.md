## https://bearssl.org/

## openssh

```
# generating the public-private keys pair in a single PEM file
$ openssl genrsa -des3 -out private.pem 2048
# export the RSA public key to a file
$ openssl rsa -in private.pem -outform PEM -pubout -out public.pem
# export the RSA private key to a file
$ openssl rsa -in private.pem -out private_unencrypted.pem -outform PEM
```
