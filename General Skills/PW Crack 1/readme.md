Burada bize iki dosya verilmiş .Bir tanesi şifreli dosya diğeri ise şifreyi çözecek olan python programı .

İlk baştan normal olarak programa dosyayı veriyoruz ve bizden nasıl birşey istediğine bakıyoruz .
Çalıştırdığımız zaman bizden şifre istiyor . Şifreyi bilmediğimiz için ilk olarak python kodunu inceliyoruz . Acaba şifre açık bir şekilde verilmiş mi verilmemiş mi diye .
Baktığımız zaman ```user_pw``` adında bir değişken ile bizim girdiğimiz veriyi tutup şart bloğunda karşılaştırma yapıyor . Şifreyi görmüş olduk . Şimdi tekrardan kodu çalıştırığ şifreyi girdiğimiz zaman flag karşımıza çıkıyor .

```sh
└─$ python level1.py level1.flag.txt.enc
Please enter correct password for flag: 8713
Welcome back... your flag, user:
picoCTF{545h_r1ng1ng_1b2fd683}
```
Flag : ```picoCTF{545h_r1ng1ng_1b2fd683}```
