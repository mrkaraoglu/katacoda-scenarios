Kaldığımız yerden devam ediyoruz.

## Hands on Lab Sayfa #2

Commit öncesi değişiklikleri de görebiliriz: 

`git status`{{execute}}

`git diff`{{execute}}

`git add .`{{execute}}

`git commit -m "Değişiklikler yapıldı"`{{execute}}

`git log`{{execute}}

Şimdi dosyamızda değişiklik yapalım.

`nano newfile`{{execute}}

`git status`{{execute}}

Bir önceki versiyona geri dönmek için ise;

`git checkout -- newfile`{{execute}}

`nano newfile`{{execute}}

Eğer silinen dosya varsa;

`rm newfile`{{execute}}

`git status`{{execute}}

`git checkout -- newfile`{{execute}}

Stage Area'dan dönmek için ise; 
Önce newfile dosyasında değişiklik yapalım, sonra stage area'ya ekleyelim.

`git add newfile`{{execute}}

`git status`{{execute}}

`git reset HEAD newfile`{{execute}}

Daha önceki versiyonlara dönmek için ise;

`git log --oneline`{{execute}}

`git checkout 12345678 -- .` {{execute}}

Sonraki sayfadan Branch (dal) kavramından bahsedeceğiz. 

Önce slaytlara dönüp biraz konuyu anlayalım.