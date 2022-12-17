Bu soruda da aynı PW Crack 1 de olduğu gibi iki dosya verdi . 
Yine python dosyasını ```cat``` ile kontrol ettiğimiz zaman şifre doğrulamasının yapıldığı yerde hex kodları karakterlere dönüştürüp doğrulama yaptığını görüyoruz . 
```chr()``` şeklinde ilerleyen hex satırını kopyalayıp terminal üzerinden şu komut satırını çalıştırdığımız zaman bize aslını gösteriyor .
```sh
$ python -c "print(chr(0x64) + chr(0x65) + chr(0x37) + chr(0x36))" 
de76
```
Programı tekrar çalıştırıp gerekli şifreyi girdiğimizde 
```sh
python level2.py level2.flag.txt.enc
```
flag karşımıza çıkıyor .

flag : ```picoCTF{tr45h_51ng1ng_489dea9a}```
