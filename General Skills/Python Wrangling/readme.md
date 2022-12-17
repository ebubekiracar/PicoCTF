3 Adet dosyayı indiriyoruz .

1- ende.py
2- flag.txt.en
3- pw.txt

Python dosyasını kullanarak flax.txt.en içindeki şifreli metnin çözülmesi isteniyor . Şifreyi çözebilmek için ise bize pw.txt içerisindeki parola verilmiş .

Öncelikle ende.py ' nin nasıl çalıştığını bilmemiz lazım . Bu yüzden her linux programında olduğu gibi ```-h``` veya ```--help``` komutları ile  bir açıklama belirtilmiş mi ona bakıyoruz . 
```
$ python ende.py -h
Usage: ende.py (-e/-d) [file]
Examples:
  To decrypt a file named 'pole.txt', do: '$ python ende.py -d pole.txt'
```
Şifreli dosyayı çözmek için ```-d``` parametresini kullanmamız gerekiyor .
```
$ python ende.py -d flag.txt.en
Please enter the password:
```
Şifreye ise pw.txt içerisindeki parolayı yazarak flag'a ulaşıyoruz .

Daha hızlı bir işlem için ```|``` operatorunu kullanabilirsiniz .

```
$ cat pw.txt | python ende.py -d flag.txt.en 
Please enter the password:picoCTF{4p0110_1n_7h3_h0us3_ac9bd0ff}
```
