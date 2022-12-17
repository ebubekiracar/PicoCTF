Netcat ile bize verilen adrese bağlandığımız zaman karşımıza 

```
'picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}'

```

Şöyle bir yarı flag yarı hex sayılardan char karşılığı alınan bir satır karşılıyor . 

Burada uzun uzadıya tek tek ```chr``` içindekilerin karşılığını bulabilirsiniz . Veya sırası ile python'da ```print(chr(<hex>)``` şeklinde de çalıştırabilirsiniz . Ama daha kısa yolu ise şu şekilde .

```python
print('picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}')
```
Bu kodu terminal üzerinden dosya ile uğraşmadan çalıştırmak için şu komutu kullanıyorum.

```sh

python -c "print('picoCTF{gl17ch_m3_n07_' + chr(0x39) + chr(0x63) + chr(0x34) + chr(0x32) + chr(0x61) + chr(0x34) + chr(0x35) + chr(0x64) + '}')"

```
Ve flag : ```picoCTF{gl17ch_m3_n07_9c42a45d}```
