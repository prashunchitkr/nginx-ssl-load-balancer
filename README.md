# Nginx SSL Loadbalancer

This repository demonstrates an example on how you can setup Nginx loadbalancer
server with SSL to point to an application server sercured with SSL.

Generate self signed cerrtifiactes using the command
```
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ./certs/<service-name>/nginx-selfsigned.key -out ./certs/<service-name>/nginx-selfsigned.crt

openssl dhparam -out ./certs/<service-name>/dhparam.pem 4096
```
