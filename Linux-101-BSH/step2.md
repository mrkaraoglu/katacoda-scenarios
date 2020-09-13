Kaldığımız yerden devam ediyoruz.

## Hands on Lab

Find komutu ile arama yapacağız**command**

`find / -name *.log`{{execute}}

`find / -name *.log` |more {{execute}}

Daha spesifik bir arama yapalım şimdi:
`find / -name *.log -size +10k`{{execute}}

Peki bu komutlar karışmaya mı başladı. O halde komutların parametlerini kolayca şöyle bulabilirsiniz: **man**

`man find`{{execute}}

Siz de deneyin farklı komutlarla. 

`cat /var/log/syslog` {{execute}}

Dosya kopyalamak için: **cp komutu**

`cp /var/log/syslog /tmp`
`ls /tmp`

Dosya taşımak için ise: **mv komutu**

`mv /tmp/syslog ./`
`ls`
`ls /tmp`

Dosyayı silmek için: **rm komutu**

`rm syslog`

