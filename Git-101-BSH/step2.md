Kaldığımız yerden devam ediyoruz.

## Hands on Lab Sayfa #2

Commit öncesi değişiklikleri de görebiliriz: 

`git status`{{execute}}

`git diff`{{execute}}

`git add .`{{execute}}

`git commit -m "Değişiklikler yapıldı`{{execute}}

Bir önceki versiyona geri dönmek için ise;

`git checkout -- newfile`{{execute}}

Eğer silinen dosya varsa;

`git rm newfile`{{execute}}

`git status`{{execute}}

`git checkout -- newfile`{{execute}}

Stage Area'dan dönmek için ise; 
Önce newfile dosyasında değişiklik yapalım, sonra stage area'ya ekleyelim.

`git add newfile`{{execute}}

`git status`{{execute}}

`git reset HEAD newfile`{{execute}}

Daha önceki versiyonlara dönmek için ise;

`git log`{{execute}}

`git checkout 12345678 -- .` {{execute}}

Sonraki sayfadan Branch (dal) kavramından bahsedeceğiz. 

Önce slaytlara dönüp biraz konuyu anlayalım.