## Hands on Lab Sayfa #3

Branchlara çalışmaya başlayalım;

`git status`{{execute}}

Hangi branch üzerinde olduğunuzu görmek için;

`git branch`{{execute}}

Yeni bir branch oluşturalım;

`git branch backend`{{execute}}

Bir de frontend diye siz oluşturun ;-)

Tüm branch listesini görmek için

`git branch -a`{{execute}}

Gitmek istediğiniz branch'a geçmek için;

`git checkout backend`{{execute}}

Burada bir dosya oluşturalım, başka bir dosyada da değişiklik yapalım. Bu değişikliklerin master branchında olmadığını görelim;

`touch yeni_dosya`{{execute}}
`git add .`{{execute}}
`git commit -m Backend dalı oluştu ve içine yeni_dosya oluşturuldu`{{execute}}
`git log`{{execute}}
`git checkout master`{{execute}}
`ls`{{execute}}

Hızlı hareket etmeyi sevenler için;
Hem oluşturur, hem o branch'a geçer.

`git checkout -b quickbranch`{{execute}}

Silmek için ise;

`git checkout master`{{execute}}

`git branch -d quickbranch`{{execute}}

İki branch arasındaki farkları görmek için;

`git diff master backend`{{execute}}

Peki branchlarımızı birleştirmek için ne yapacağız?
Önce birleştirmek istediğimiz brancha gidiyoruz. Sonra;

`git checkout master`{{execute}}

`git merge`{{execute}}

Bakalım dosyamız gelmiş mi?

`ls`{{execute}}

Değişiklikler de log'a gelmiş olmalı;

`git log`{{execute}}

Sona yaklaşıyoruz. Sonraki sayfaya geçelim.
