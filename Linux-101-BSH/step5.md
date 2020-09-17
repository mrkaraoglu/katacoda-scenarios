## Hands on Lab Sayfa #5

Sona yaklaşırken dosyalardan biraz daha sistem seviyesine inelim.

Yavaş gidelim. Şifre değiştirmek için: passwd

`passwd`{{execute}}

`useradd emre`{{execute}}

`passwd emre`{{execute}}

Gruplara bakalım:

`groupadd testgrup`{{execute}}

Grupları listeleme:

`cat /etc/group |more`{{execute}}

Kullanıcıyı gruba ekleme

`usermod -aG testgrup emre`{{execute}}

`grep emre /etc/group`{{execute}}

Biraz fantezi yapalım mı? Önce bir uygulama kuralım:

`apt install members`{{execute}}

`members testgrup`{{execute}}

Kullanıcı yetkileri için **chmod** komutu kullanılır. Bunu daha iyi anlamak için de;

4: Okuma
2: Yazma
1: Çalıştırma (dizin için içine girebilme)
sahibi-grubu-diğer kullanıcılar

Bir dosya oluşturalım:

`touch test_file`{{execute}}

Bu dosyanın yetkilerini herkese yetki verecek şekilde değiştirelim:

`chmod 777 test_file`{{execute}}
`ls -la`{{execute}}

Sadece kullanıcısına full yetki verelim;

`chmod 700 test_file`{{execute}}

`chmod +x test_file`{{execute}}

Deneyin bakalım ne oldu? :-)

