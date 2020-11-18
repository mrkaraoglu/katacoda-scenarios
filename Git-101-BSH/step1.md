Git-101 Eğitimine hoşgeldin.

## Hands on Lab Sayfa #1

Bu Lab çalışması hem eğitimde öğreneceğimiz komutları takip etmek için hem de yanda kullanabileceğiniz bir Ubuntu Linux sunmak için hazırlanmıştır. 
Lütfen sadece yazılı komutlarla yetinmeden, aklınıza gelenleri deneyin. Hiç bir şey kaybetmeyeceksiniz, bir "refresh" her şeyi çözer :-)

Ve, oyun başlasın ;-)

Önce git ayarlarımızı yaparak başlıyoruz **command**

`git config --global user.name "Emre Karaoglu"`{{execute}}
 **command**

`git config --global user.email emrekaraoglu@gmail.com.tr`{{execute}}

Olmuş mu bakalım ;) **command**

`git config --global user.name`{{execute}}

Bir dizin oluşturup o dizini git tarafından takip edilmesini sağlayalım; **command**

`mkdir proje`{{execute}}

`ls`{{execute}}

`cd proje`{{execute}}

`git init`{{execute}}

Şimdi bir dosya oluşturalım içine;

`touch newfile`{{execute}}

`nano newfile`{{execute}}

Bu dosyamızı git içine aktaralım; 

`git add .`{{execute}}

`git commit -m "First File added"`{{execute}}

`git log`{{execute}}

`git status`{{execute}}

Şimdi 2. sayfadan devam etmeden önce yeni bir dosya daha ekleyin, ardından o dosyayı da git'e commit edin. 