# Patient-Survival-Prediction

# Hastane Veri Analizi Projesi

## Proje Özeti
Bu proje, hastaneye yatırılan hastaların yoğun bakım süreçleriyle ilgili verileri analiz ederek, hastane içi ölüm oranlarını etkileyen faktörleri anlamayı amaçlamaktadır. Projede kullanılan veri seti, hasta demografik bilgileri, yoğun bakım kabul kaynakları, yoğun bakım türleri ve belirli klinik ölçümleri içermektedir.

## Veri Seti
Kullanılan veri seti, hastaların hastane ve yoğun bakım ünitesi içindeki durumlarına ilişkin detaylı bilgiler içermektedir. Verilerde eksik değerler ve çeşitli veri türleri (sayısal ve kategorik) bulunmaktadır. Verilerin işlenmesi sırasında eksik veri analizi ve veri temizleme işlemleri uygulanmıştır.

### Veri Seti Özellikleri
- **Ethnicity (Etnik Köken):** 6 kategori, eksik değerler NaN.
- **Gender (Cinsiyet):** 2 kategori (M, F), eksik değerler NaN.
- **ICU Admit Source (Yoğun Bakım Kabul Kaynağı):** 5 kategori.
- **ICU Stay Type (Yoğun Bakım Kalış Türü):** İlk kabul, yeniden kabul veya transfer.
- **ICU Type (Yoğun Bakım Türü):** 8 farklı tür.
- **Apache 3J Body System:** 12 vücut sistemi kategorisi.
- **Apache 2 Body System:** 11 vücut sistemi kategorisi.

## Kullanılan Kütüphaneler
Projede aşağıdaki Python kütüphaneleri kullanılmıştır:
- **Pandas:** Veri işleme ve analiz.
- **Matplotlib ve Seaborn:** Veri görselleştirme.
- **Missingno:** Eksik veri analizi ve görselleştirme.
- **Scikit-learn:** Makine öğrenmesi ve tahminleme.

## Yapılan Analizler
### 1. Veri İncelemesi ve Temizleme
- **Veri Tipi Kontrolü:** Her sütunun veri tipi gözden geçirilerek, kategorik ve sayısal veri türleri ayrıldı.
- **Eksik Veri Analizi:**
  - Eksik değerlerin tespit edilmesi ve görselleştirilmesi için `missingno` kütüphanesi kullanıldı.
  - Eksik veriler:
    - Silindi (yüksek eksiklik oranı varsa).
    - Ortalama, medyan, mod gibi yöntemlerle dolduruldu.

### 2. Kategorik Değişkenlerin Analizi
- Frekans ve yüzdelik dağılımlar incelendi.
- Çapraz tablolar kullanılarak kategoriler arası ilişkiler analiz edildi.
- Çubuk grafikler ile görselleştirme yapıldı.

### 3. Sayısal Verilerin Analizi
- Dağılım ve temel istatistiksel metrikler incelendi.
- Kutu grafikleri ve histogramlar oluşturularak verilerdeki uç değerler tespit edildi.

### 4. Eksik Veri Stratejileri
- **Silme:** Eksik veriler rastgele dağılım gösteriyorsa veya eksiklik oranı düşükse, ilgili satırlar silindi.
- **Doldurma:** Ortalama, medyan veya mod kullanılarak eksik veriler dolduruldu. Zaman serisi verileri için ileri ve geri doldurma yöntemleri kullanıldı.

## Çıktılar ve Sonuçlar
Analiz sonucunda, hastane içi ölüm oranlarını etkileyen ana faktörler arasında şunlar tespit edilmiştir:
1. Hastanın demografik özellikleri (cinsiyet, etnik köken).
2. Yoğun bakım kabul kaynağı ve türü.
3. Apache skorlarına dayalı klinik ölçümler.

Bu bulgular, hastane yönetimine hasta bakım süreçlerini iyileştirme konusunda bilgi sağlayabilir.
