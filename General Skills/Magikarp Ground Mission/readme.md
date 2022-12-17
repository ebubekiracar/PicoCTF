Makineyi başlatıyoruz ve ssh ile giriş yapacağız .
```
ssh ctf-player@venus.picoctf.net -p 52674
```
```a13b7f9d``` parolası ile giriş yapıyoruz .

Sisteme girip ```ls``` dediğimiz zaman iki dosya karşılıyor . Birincisi
flag'in ilk parçası . İkincisi ise ikinci parçasını bulmamız için bize verilen ipucu . Bize ```/``` dizinine gitmemizi istiyor . 
İlk parçayı ```cat``` ile okuyoruz ve köşeye kaydediyoruz .
```
picoCTF{xxsh_
```
```cd / ``` ile dizine geçtikten sonra yine aynı şekilde iki dosya . Birisi ikinci parça diğeri üçüncü parça için bize verilen ipucu . 
İkinci parçayı cat ile okuyoruz .
```
0ut_0f_\/\/4t3r_
```
```cd ~``` komutu ile kullanıcı dizinine geçiyoruz . Ve üçüncü parçayı okuyarak bir araya getiriyoruz .
```
71be5264}
```

Flag => ```picoCTF{xxsh_0ut_0f_\/\/4t3r_71be5264}```
