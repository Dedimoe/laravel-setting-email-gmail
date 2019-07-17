# laravel-setting-email-gmail
laravel-setting-email-gmail

Login to gmail and under *My account* > *Sign In And Security* > *Sign In to google*, enable two step verification, then you can generate app password, and you can use that app password in .env file.

Your .env file will then look something like this
```
MAIL_DRIVER=smtp
MAIL_HOST=smtp.gmail.com
MAIL_PORT=587
MAIL_USERNAME=youremail@gmail.com
MAIL_PASSWORD=*yourpassword*
MAIL_ENCRYPTION=tls
```

And run below after you make changes in your .env file.
```
php artisan config:cache 
```
