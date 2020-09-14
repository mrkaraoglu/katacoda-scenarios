## Hands on Lab Sayfa #4

Dosyalarla oynamaya devam.
head komutu ile bir dosyanın ilk satırları (default:10) gösterilir.

`head /var/log/dmesg`{{execute}}
`head -n 5 /var/log/dmesg`{{execute}}

tail komutu ise son satırları gösterir:

`tail -n 6 /var/log/dmesg`{{execute}}

Hadi biraz oynayalım:

`ls -la /var/lib > folder_detail`{{execute}}
`ls -la /var/lib >> folder_detail`{{execute}}

Ne fark var? wc komutu ile satır sayısını öğrenebiliriz;

`wc -l folder_detail`{{execute}}

wc -c : Dosyadaki byte sayar
wc -l : Satır sayar
wc -w : kelime sayar

