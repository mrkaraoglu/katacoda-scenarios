Kaldığımız yerden devam ediyoruz.

## Hands on Lab Sayfa #2

Şimdi kendi paketlerimizi build edelim;

O halde bir ping de atabilen Ubuntu imajı hazırlayalım. Bunun için Dockerfile dosyamıza şunu yazmalıyız:

`mkdir UbuntuWPing`{{execute}}

`cd UbuntuWPing`{{execute}}

`touch Dockerfile`{{execute}}

`nano Dockerfile`{{execute}}

Ve aşağıdakileri Dockerfile dosyasına ekleyelim.

<pre class="file">

        FROM ubuntu
        MAINTAINER "Emre Karaoglu"
        RUN apt update
        RUN apt install -y iputils-ping

</pre>

Kaydedip çıkıyoruz ve hazırladığımız Dockerfile'ı build ediyoruz;

`docker build -t ubuntuwping .`{{execute}}

`docker run -it ubuntuwping /bin/bash`{{execute}}

Şimdi çalışıyor mu peki ping? 

`ping 8.8.8.8`{{execute}}

exit ile çıkabiliriz

`exit`{{execute}}

Son örneğimiz için bir sonraki sayfaya geç