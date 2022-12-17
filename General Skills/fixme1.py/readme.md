Bize bir python dosyası veriyor . Çalıştırdığımız zaman hatalı olduğunu gösteriyor . Fixlemeye çalışacağız .
20.satırda bir hata olduğunu söylüyor .
```
  File "/home/analyst/Desktop/PicoCTF/General Skills/fixme1.py/fixme1.py", line 20
    print('That is correct! Here\'s your flag: ' + flag)
IndentationError: unexpected indent

```
Baktığımız zaman 20.satır fonksiyon bloğunun içinde olduğu için çalışmıyor . 
Başındaki boşlukları silerek bloktan çıkarıp tekrar çalıştırıyoruz ve 

flag: ```picoCTF{1nd3nt1ty_cr1515_6a476c8f}```
