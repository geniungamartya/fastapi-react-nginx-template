
# Setup Nginx
```
sudo apt install nginx
mv ./config/nginx/conf/geniungamartya.xyx.conf /etc/nginx/sites-available/
sudo ln -s /etc/nginx/sites/available/geniungamartya.xyz.conf /etc/nginx/sites-enabled/
sudo nginx -t
sudo systemctl restart nginx
```


# Generate SSL

```
sudo apt install certbot python3-certbot-nginx
sudo certbot --nginx -d "geniungamartya.xyz"
```