## Hands on Lab Sayfa #4

Github'tan bahsedeceğiz, önce slayta dönelim, sonra bir kaç uygulama için geri dönün ama ;-)

github101 adında bir repo oluşturduğunuzu düşünüyorum.

**Bu komutu kendi adresinize göre düzenleyin**

Github'a remote bağlantı kurmak için;
`git remote add github_remote https://github.com/mrkaraoglu/github101`{{execute}}

Bağlantımız oldu mu? 

`git remote`{{execute}}

Local'deki git repomuzu github'ın master branch'ına yollayalım;

`git push -u github_remote master`{{execute}}

Github'tan bir repo'yu local'e çekmek için ise;

`git pull https://github.com/mrkaraoglu/katacoda-scenarios`{{execute}}