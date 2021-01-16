## Hands on Lab Sayfa #3

Şimdi basit bir Web uygulaması yapalım.

Önce bir üst dizine çıkıp yeni bir dizin oluşturalım. Sonras bildiğimiz gibi;

`cd ..`{{execute}}

`mkdir WebApp`{{execute}}
**command**

`cd WebApp`{{execute}}

Önce basit PHP kodumuzu yazalım;

Bunu da src dizini oluşturup yapabiliriz;

`mkdir src ; cd src ; touch index.php`{{execute}}

`nano index.php`{{execute}}

Buraya bir PHP kodu yazmalıyız. Örneğin;

<?php

echo "Hello All... It's Docker :-)"

?>

Şimdi bir üst dizinde bir Dockerfile oluşturalım;

`cd ..`{{execute}}

`nano Dockerfile`{{execute}}

Dockerfile içine ise şunları ekleyelim;

FROM php:7.3-apache
COPY src/ /var/www/html/
EXPOSE 80

Artık Dockefile'ımızı build edebiliriz;

`docker build -t webapp .`{{execute}}

Şimdi çalıştırıyoruz;

`docker run -p 8080:80 webapp`{{execute}}
