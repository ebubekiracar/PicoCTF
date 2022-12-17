Burada bize verilen adrese netcat ile bağlantı sağladığımızda bizden bir cümlenin veya kelimenin md5 karşılığını istiyor . Bunun için ikinci bir terminal ekranı açıp şu komutu kullanıyoruz .

```sh
echo -n "istenilen cümle veya kelime" | md5sum
```

Bizden birkaç kez farklı şekilde sorduğu soruları yine yukardaki komut ile md5'leri öğreniyor ve cevaplıyoruz . Ve sonunda flag karşımıza çıkıyor .

flag: ```picoCTF{4ppl1c4710n_r3c31v3d_674c1de2}```
