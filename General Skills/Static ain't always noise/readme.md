Her iki dosyayıda indiriyoruz
ltdis.sh 'a çalıştırma yetkisi veriyoruz
çalıştırdığımız zaman bize nası kullanmamız gerektiği hakkında ipucu veriyor .

```./ltdis.sh <program-file>```
şeklinde çalıştırmamız gerekiyor . program dosyası olarak static dosyasını vereceğiz .
```
./ltdis.sh static 
```
sonuc olarak bize iki dosya çıkarıyor . Birisi strings.txt ile bitiyor diğeri x86_64.txt ile bitiyor . 

strings.txt ile biteni ```cat``` ile okuduğumuzda bize 1020 numara ile başlayan satırda flag'i gösteriyor .
```
1020 picoCTF{d15a5m_t34s3r_6f8c8200}
```
