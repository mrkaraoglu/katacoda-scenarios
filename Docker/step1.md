Docker Eğitimine hoşgeldin.

## Hands on Lab Sayfa #1

Bu Lab çalışması "Docker" eğitimin uygulama aşamasını yapmak üzere hazırlandı.

Ve, oyun başlasın ;-)

Sistemimizde Docker çalışıyor mu? Hangi versiyon gibi bazı detay bilgileri almak için:

`docker info`{{execute}}
**command**

`docker version`{{execute}}

Sistemimizde docker çalışıyor gibi. O halde ilk containerimizi çalıştıralım. 
Yazılımın şanındandır "Hello World" ile başlamış olalım :-) **command**

`docker container run hello-world`{{execute}}

Çalışıp çalışmadığını kontrol etmek için;

`docker ps`{{execute}}

`docker ps -a`{{execute}}

Bu containeri silmek için ise;

`docker container rm`{{execute}}
:-) Buraya container-id veya Container name bilgisini yazmalısınız tabi ki.

Sistemimizde hangi image'lar var?

`docker images`{{execute}}

Ubuntu image'ını çalıştıralım

`docker run ubuntu`{{execute}}

**command**

`docker run ubuntu ls /lib/bin`{{execute}}

Daha ele avuca gelen bir Ubuntu daha hoş olur:

`docker run -it ubuntu /bin/bash`{{execute}}

Güzel bir Ubuntu imajı ama ping atabiliyor muyuz? :-)

Bir sonraki sayfadan devam edelim...