## Hands on Lab Sayfa #3

Eğlenceli bir komutla devam edelim: grep**command**

`cat /var/log/dmesg`{{execute}}

`grep cpu /var/log/dmesg`{{execute}}

Şimdi en sevdiğimiz, komut katarı yaoacağız. Bunun için | kullanıyoruz:

`find /var -type f -name *.log |grep apt`{{execute}}

Biraz Root kullanıcısından bahsedelim.

`sudo su -`{{execute}}

`whoami`{{execute}}

Disk büyüklüğü için: df

`df`{{execute}}

`df -h`{{execute}}

Dizin veya dosya büyüklüğü için: du

`du -h /var/log`{{execute}}