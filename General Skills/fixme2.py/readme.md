fixme1 de olduğu gibi burdada istenilen python dosyasını indirip çalıştırdığımızda bir hata ile karşılaşıyoruz . 

```
  File "/home/analyst/Desktop/PicoCTF/General Skills/fixme2.py/fixme2.py", line 22
    if flag = "":
       ^^^^^^^^^
SyntaxError: invalid syntax. Maybe you meant '==' or ':=' instead of '='?

```

Burada hatanın olduğu satıra indiğimiz zaman if bloğunda flag değişkenini kontrol ederken yanlış parametre kullandığını görüyoruz .

```
flag=""
```

yerine 

```
flag==""
```

yaparak kodu düzeltiyoruz ve tekrar çalıştırdığımızda flag karışımızda.


flag: ```picoCTF{3qu4l1ty_n0t_4551gnm3nt_4863e11b}```
