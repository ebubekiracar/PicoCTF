Öncelikle bu soru bölümün en güzel sorularından biridir diyebilirim .

Soruda bize bir tane c dili ile yazılmış bir kaynak kod verilmiş . Bu kaynak kod verdiği sunucuya bağlandığımızda bizi karşılayan shop alanıdır .

Sunucuya bağlandığımızda bizi market karşılamakta . Burada bakiyemizi görebiliyoruz ve flag satın alıyoruz . Flag satın alma kısmında ise 2 seçenek bulunmakta . Burada önemli olan ikinciseçenek çünkü flag burada oluşturulup bize veriliyor .Ama birinci seçenek ise bize flagi almada yardım edecek . Peki nasıl ?

Flag almak için birinci seçeneği seçtiğimizde bizden kaç tane almak istemediğimizi soruyor . Ve girdiğimiz değer 900 ile çarpıp bize satın alım için gerekli
miktarı söylüyor . Eğer miktar bakiyemizden düşük ise direk çekim yapıyor . Değil ise toplam ödeme miktarını bize gösteriyor .

Kodları incelediğimiz zaman bizden adet sayısını isterken int bir değer belirlemiş . Buda demek oluyorki ```int``` bir değer en fazla ```2147483647``` değerini alabilir . Bunu geçtiği anda ```-2147483648``` değerini alır . İşte bu olay ```integer overflow``` olarak bilinir .

Kaynak kodu incelediğimiz zaman
```c
...
...
int total_cost = 0;
total_cost = 900*number_flags;
printf("\nThe final cost is: %d\n", total_cost);
if(total_cost <= account_balance){
account_balance = account_balance - total_cost;
...
...
```
Burada almak istediğimiz flag sayısı 900 ile çarpılıp total_cost denilen toplam ödeme miktarına atanıyor . Sonrasında eğer miktar bizim hesabımızdaki paradan küçük ise hesabımızdan çekiliyor . 
Peki biz ```number_flags```'e int boyutunu (2147483647) geçecek şekilde değer verirsek ne olur ? Tabikide boyut negatife dönüşür . Sonrasında şu işlemi gerçekleştirmesini sağlamış oluruz :
```c
account_balance = account_balance -  total_cost;
    1100	=        1100     -  (-2147483648) ; // 1100 + 2147483648
```
Ve bu sayede hesabımızdaki para yükselmiş olur . Sonrasında flag alma seçeneğinden ikinci seçeneği seçerek flag'i almış oluruz .

flag:```picoCTF{m0n3y_bag5_65d67a74}```
