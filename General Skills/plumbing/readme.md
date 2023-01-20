Burada bizden istenilen sunucuya bağlandığımızda çok fazla satıra sahip bir çıktı ile karşılaşıyoruz . CTF sorusunun açıklamasında da bunu az çok belirtmiş aslında . Bu yüzden bizim bu çıktıyı bir dosyaya aktarıp oradan flag'i bulmamız gerekiyor. Bunun için büyüktür ```>``` sembolünü kullanıyoruz. Evet bu bir yerlerden tanıdık gelmiş olmalı . Bir çıktıyı bir dosyanın içine yazmak için kullanıyoruz . Bu sembol üstüne yazarken alt satıra yazması içinde iki tane büyüktür sembolü kullanıyorduk .Aynı işlemi burada da yapacağız. 

```shell
nc jupiter.challenges.picoctf.org 4427 > output.txt
```
Dosyayı açtığımızda ```CTRL+F``` yardımı ile ```picoCTF``` yazdığımız zaman flag karşımıza çıkıyor .

flag: ```picoCTF{digital_plumb3r_5ea1fbd7}```
