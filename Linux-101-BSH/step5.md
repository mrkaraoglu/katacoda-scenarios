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
