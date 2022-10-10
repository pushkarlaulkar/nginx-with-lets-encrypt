CentOS 8 nginx with LetsEncrypt

```
yum install nginx -y
```
```
systemctl enable --now nginx
```

```
yum install epel-release -y
```

```
yum install certbot python3-certbot-nginx -y
```

```
certbot --nginx -d your_domain -d www.your_domain
```

Verify the status of your SSL certificate by opening the following link in your preferred web browser (don’t forget to replace your_domain with your base domain):

https://www.ssllabs.com/ssltest/analyze.html?d=your_domain

Visit your site now

https://your_domain
