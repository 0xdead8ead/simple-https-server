Simple HTTPS Server
===================

Code ganked from here:  https://gist.github.com/dergachev/7028596

Get HTTPS Cert for Server:

sudo certbot certonly --register-unsafely-without-email --standalone -d <domain_name>
sudo cat /etc/letsencrypt/live/<domain_name>/fullchain.pem > server.pem
sudo cat /etc/letsencrypt/live/<domain_name>/privkey.pem >> server.pem
