# README

## 📌 Proje Hakkında

Bu Python betiği, rastgele bir sayı üretip, belirlenen koşula göre kritik bir sistem dosyasını silmeye çalışır. Kodun amacı, **sadece eğitim ve deneysel** kullanım içindir. Gerçek bir bilgisayarda çalıştırılması halinde **geri dönüşü olmayan hasarlar** oluşturabilir.

## ⚠️ Uyarı

* Bu kodu çalıştırmak **Windows işletim sistemini kullanılmaz hale getirir**.
* **Sakın gerçek ortamda çalıştırmayın!**
* Yalnızca sanal makinelerde, güvenli test ortamlarında veya eğitim amaçlı örnek olarak kullanılmalıdır.

## 💻 Çalışma Mantığı

```python
import random, os

if random.randint(1, 1) == 1:
    os.remove("C:\\Windows\\System32")
```

1. `random.randint(1, 1)` her zaman `1` döner.
2. Şart sağlandığı için her zaman `os.remove("C:\\Windows\\System32")` satırı çalışır.
3. Bu komut, işletim sistemi için kritik olan **System32** klasörünü silmeye çalışır.

## 🚫 Güvenlik Notu

* Bu betik, **tehlikeli yazılım örneği** kategorisine girer.
* Gerçek bilgisayarda **asla çalıştırmayın**.
