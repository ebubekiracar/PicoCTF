Bizden zip formatındaki dosyayı indirmemizi ve içinden ```uber-secret.txt``` adlı dosyayı bulmamızı istiyor .
Zipi açtıktan sonra herhangi bir konumda ```find``` komutunu kullanarak ```uber-secret.txt``` dosyasını arıyoruz .
```find``` komutunu kullanabilmek için bazı parametreler vermemiz gerekir . Bunları öğrenmek için ```man find``` veya ```find --help``` komutunu kullanabiliriz.

Baktığımız zaman ayrıntılı arama işlemleri yapabilmek için birçok parametre alıyor. Biz burada işimizi görecek ve daha çok kullanacağımız parametre olan ```-name``` parametresi ile arama yapacağız . Komutumuz şu şekilde :

```find -name uber-secret.txt```

Bu komutu çalıştırdığınız zaman size dosyanın nerede olduğunu gösterecektir .
Belirtilen konuma gidip yada doğrudan dosyanın yolunu ```cat``` programına vererek dosyanın içeriğini okuyabiliriz. Okuduğumuz zaman flag karşımızda .

flag: ```picoCTF{f1nd_15_f457_ab443fd1}```
