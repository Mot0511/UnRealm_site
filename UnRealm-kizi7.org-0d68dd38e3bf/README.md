/etc/nginx/sites-available
Create a file yoursitename.com

Put inside this text



server {
server_name yoursitename.com;
root /var/www/yoursitename.com/web;
index index.html index.htm;
location / {}

}


Create a folder and put files of site inside/
/var/www/yoursitename.com/


Create Sym Link

sudo ln -s /etc/nginx/sites-available/yoursitename.com /etc/nginx/sites-enabled/


sudo certbot --nginx

Choose yourwebsitename 

sudo systemctl restart nginx
