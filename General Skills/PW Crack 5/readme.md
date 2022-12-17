Bize 4 adet dosya vermiş . Hepsini indiriyoruz . Öncekilerine ek olarak ```dictionary.txt``` adında parolaların tutulduğu bir dosyamız daha var . Burada bu parolaları python içinde değişken olarak tutmamışta ayrı bir dosya halinde vermiş . Şimdi biz bunu python ile okuyup satır satır parola kontrolü yapmamız lazım .

Bunun için python kodundaki ```level_5_pw_check()``` fonksiyonunu yeniden düzenliyoruz .
```py

def level_5_pw_check():
    f = open('dictionary.txt','r')
    for i in f :
     user_pw = i.strip()
     user_pw_hash = hash_pw(user_pw)
    
     if( user_pw_hash == correct_pw_hash ):
         print("Welcome back... your flag, user:")
         decryption = str_xor(flag_enc.decode(), user_pw)
         print(decryption)
         return
     print("That password is incorrect")
```
Burada ```strip()``` kullanmamızın nedeni . Python satır satır okuma yaptığı zaman her satırın sonundaki bizde görünmeye ```\n``` ifadesini de alır . Bu yüzden bunu kullanarak doğrulamaya gidecek parolanın sade biçimde gitmesini sağlıyoruz . ```\n``` den kurtarıyoruz.

Programı tekrar çalıştırdığımızda flag'i yakalamış oluyoruz .

flag: ```picoCTF{h45h_sl1ng1ng_fffcda23}```
