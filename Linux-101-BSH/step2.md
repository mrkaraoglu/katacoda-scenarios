Kaldığımız yerden devam ediyoruz.

## Hands on Lab Sayfa #2

Dosyanın içini okumak: 

`cat /var/log/syslog`{{execute}}

Dosya kopyalamak için: **cp komutu**

`cp /var/log/syslog /tmp`{{execute}}

`ls /tmp`{{execute}}

Dosya taşımak için ise: **mv komutu**

`mv /tmp/syslog ./`{{execute}}

`ls`{{execute}}

`ls /tmp`{{execute}}

Dosyayı silmek için: **rm komutu**

`rm syslog`{{execute}}

Find komutu ile arama yapacağız**command**

`find / -name *.log`{{execute}}

`find / -name *.log |more` {{execute}}

Daha spesifik bir arama yapalım şimdi:

`find / -name *.log -size +10k`{{execute}}

Peki bu komutlar karışmaya mı başladı. O halde komutların parametlerini kolayca şöyle bulabilirsiniz: **man**

`man find`{{execute}}

Siz de deneyin farklı komutlarla. 

Bir sonraki sayfadan devam edelim ;-)