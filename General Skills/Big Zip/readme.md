Bu bölümde de firs find sorusunda olduğu gibi bir zip indirip içerisinde flag bulmamız isteniyor . Ama diğerinden farkı olarak bu sefer flag random bir txt içerisine bulunmakta . Bunun için find komutunun daha ayrıntılı olarak kullanmamız gerekecek veya farklı bir yöntem olan grep komutu ile daha basit bir şekilde arayabilriz . 
Bu aşağıdaki komut ile bize içinde pico geçen dosyayı bulması istenebilir .
```sh
find . -iname '*' | xargs grep 'pico' -sl
```
Çıktı:
```
./folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt
```
Diğer bir yöntem ise ```grep``` komutunu recursive olarak kullanmak . 
```
grep -r picoCTF .
``` 
Şeklinde kullandığımız zaman bize konumu ile beraber içeriğinide göstermiş olacak .
```
./folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt:information on the record will last a billion years. Genes and brains and books encode picoCTF{gr3p_15_m4g1c_ef8790dc}

```
flag:```picoCTF{gr3p_15_m4g1c_ef8790dc}```
