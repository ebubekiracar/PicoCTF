Bize verdiği dosya içerisinde flag bulunuyor ama bunu tek tek incelememizin yorucu olacağını söylüyor . Bu yüzden burada ```grep``` komutunu kullanmamız daha mantıklı . Grep komutu tek başına kullanılmıyoru bu yüzden dışarıdan bir girdi alması lazım . En başta ```cat``` ile dosya içeriğini okuyoruz ve çıktısını grep komutuna yönlendiriyiruz . Yönlendirmek içinde ```|``` Pipe denilen karakteri kullanıyoruz . 

Kullanacağımız komut örneği şu şekilde
```cat file | grep <aranacak_kelime>```

Şimdi pico kelimesini aratarak flag'i bulalım 

```cat file | grep pico```

ve flag 

```picoCTF{grep_is_good_to_find_things_5af9d829}```
