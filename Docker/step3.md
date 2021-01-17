## Hands on Lab Sayfa #3

Şimdi basit bir Web uygulaması yapalım.

Önce bir üst dizine çıkıp yeni bir dizin oluşturalım. Sonras bildiğimiz gibi;

`cd ..`{{execute}}

`mkdir WebApp`{{execute}}

`cd WebApp`{{execute}}

Önce basit PHP kodumuzu yazalım;

Bunu da src dizini oluşturup yapabiliriz;

`mkdir src ; cd src ; touch index.php`{{execute}}


Bu dosyaya bir PHP kodu yazmalıyız. Örneğin;

`nano index.php`{{execute}}

<pre class="highlight">

       < ? php
        echo "Hello All... It's Docker :-)";
       ?>
    
</pre>

** Kopyala yapıştır yapıyorsanız ilk satırdaki boşlukları silmeyi unutmayın :-) **

Şimdi bir üst dizinde bir Dockerfile oluşturalım;

`cd ..`{{execute}}

`touch Dockerfile`{{execute}}

Dockerfile içine ise şunları ekleyelim;

<pre class="file">

        FROM php:7.3-apache
        COPY src/ /var/www/html/
        EXPOSE 80
    
</pre>

Artık Dockefile'ımızı build edebiliriz;

`docker build -t webapp .`{{execute}}

Şimdi çalıştırıyoruz;

`docker run -p 8080:80 webapp`{{execute}}
