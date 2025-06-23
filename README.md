# Kiz-basina-bitirme-1
Kız başına veri analizi bootcamp sertifikası için gerekli olan bitirme projesi

# ✈️ Airline Passenger Satisfaction Data Analysis

Merhaba!  
Bu projede, havayolu yolcularının memnuniyet durumunu etkileyen faktörleri analiz etmeyi hedefledim. Gerçek bir veri seti üzerinde çalışarak istatistiksel özetler, eksik veri analizi, aykırı değer tespiti ve veri görselleştirmesi adımlarını gerçekleştirdim. Projenin her aşamasını Python dilini kullanarak Google Colab ortamında yürüttüm.

## 📁 Veri Seti

Bu projede kullanılan veri seti: **Airline Passenger Satisfaction Dataset**

Veri seti, yolcuların cinsiyeti, yaşı, seyahat tipi, uçuş sınıfı, hizmet değerlendirmeleri ve uçuş sürelerine dair çeşitli bilgiler içermektedir. Özellikle **satisfaction** sütunu hedef değişken olarak kullanılmıştır. (satisfied / neutral or dissatisfied)

## 🔍 Proje Amaçları

- Sayısal ve kategorik veriler üzerinde istatistiksel analizler yapmak
- Eksik değerlerin tespit edilip uygun yöntemle işlenmesi
- Aykırı değerleri tespit edip yorumlamak
- Verileri uygun grafiklerle görselleştirerek içgörüler elde etmek

## 🛠️ Kullanılan Kütüphaneler

- `pandas`
- `matplotlib`
- `seaborn`

## 📊 Yapılan Analizler

### ✅ 1. İstatistiksel Özet
Veri setinde yer alan sayısal sütunlar için ortalama, medyan, standart sapma, min ve max değerleri hesapladım. Genel olarak hizmet kalitesi ortalamalarının 3 civarında olduğunu ve uçuş mesafelerinde büyük bir dağılım olduğunu gözlemledim.

### 🧩 2. Eksik Değer Analizi
Veride sadece `Arrival Delay in Minutes` sütununda eksik değer vardı (310 adet). Bu eksik veriler çok az sayıda olduğu için medyan değerle doldurmayı tercih ettim.

### ⚠️ 3. Aykırı Değer Analizi
Bazı sütunlarda özellikle uçuş mesafesi ve gecikme sürelerinde aykırı değerler bulunduğunu tespit ettim. Gecikme sürelerinde 1500 dakikayı aşan değerler gözlemlendi. Bu değerler çok nadir olsa da analiz dışı bırakılmadı, çünkü uçuş gecikmeleri gerçek dünyada da ekstrem olabilir.

### 📈 4. Görselleştirme
Veriyi daha anlaşılır hale getirmek için seaborn kütüphanesiyle çeşitli grafikler oluşturdum:
- Yolcu memnuniyet durumu dağılımı
  ![indir](https://github.com/user-attachments/assets/de70aef8-9684-43e3-b218-55beddb49efd)

- Seyahat türüne göre memnuniyet
- Boxplot'larla yaş, uçuş mesafesi ve gecikme sürelerinin aykırı değer analizi

## 📌 Genel Değerlendirme

Bu proje boyunca veriyi temizlemeyi, anlamayı ve görselleştirerek içgörüler elde etmeyi hedefledim. Elde ettiğim bazı sonuçlar şunlar oldu:

- **Business Travel** yapan yolcuların memnuniyet düzeyi genel olarak daha yüksek.
- Hizmet kalitesi (özellikle inflight entertainment ve cleanliness) arttıkça memnuniyet de artıyor.
- Bazı hizmet puanlarında 0 değerleri bulundu, bu durum veri giriş hatası veya bilinçli 0 puanlama olabilir.

## 💡 Kendi Notum

Bu proje sayesinde veri analizi sürecine dair temel ama etkili adımları uygulamalı olarak deneyimlemiş oldum. Özellikle eksik ve aykırı veri ile başa çıkma yöntemlerini pekiştirme fırsatım oldu.

---

Teşekkür ederim! 🙌  
Her türlü öneriye veya geri bildirime açığım.
