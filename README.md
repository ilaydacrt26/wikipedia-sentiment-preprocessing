# Wikipedia Duygu Analizi -- Veri Temizleme ve Görselleştirme

Bu proje, Wikipedia'dan elde edilen duygu analizi verileri üzerinde
**veri temizleme**, **ön işleme** ve **görselleştirme** işlemlerini
gerçekleştirmek amacıyla hazırlanmıştır.\
Model eğitimi yapılmamış olup, tamamen **data preprocessing + EDA
(Exploratory Data Analysis)** odaklıdır.

------------------------------------------------------------------------

## Proje İçeriği

Notebook'ta gerçekleştirilen işlemler:

### 1. Veri Yükleme

`wiki_data.csv` dosyası okunarak temel tablo yapısı incelendi.

### 2. Metin Temizleme (Text Cleaning)

Aşağıdaki işlemleri yapan bir temizleme fonksiyonu uygulandı:

-   Küçük harfe dönüştürme\
-   Noktalama işaretlerini kaldırma\
-   Rakamları kaldırma\
-   Gereksiz boşlukları silme

### 3. Stopwords Temizleme

NLTK ile İngilizce durak kelimeler indirildi ve metinlerden çıkarıldı:

-   "the", "and", "is", "to" gibi bağlaçlar temizlendi\
-   Her satır kelime listesine dönüştürülerek stopwords filtrelendi

### 4. Temizlenmiş Verinin İncelenmesi

-   İlk satırlar kontrol edildi\
-   Kelime sayısı değişimleri gözlemlendi

### 5. Veri Görselleştirme

Keşifsel veri analizi için temel grafikler oluşturuldu:

-   Kelime dağılımı\
-   Duygu sınıflarının dağılım grafiği (varsa)\
-   Temizlenmiş metinlerden word cloud üretimi

------------------------------------------------------------------------

## Kullanılan Teknolojiler

-   **Python**
-   **Pandas**
-   **NLTK**
-   **Matplotlib**
-   **WordCloud** (varsa)

------------------------------------------------------------------------

## Amaç

Verileri duygu sınıflandırması için hazır hale getirmek,\
temizlemek ve analiz etmek isteyen geliştiricilere örnek bir ön işleme
akışı sunmak.

------------------------------------------------------------------------

## Dosyalar

  -----------------------------------------------------------------------
  Dosya                         Açıklama
  ----------------------------- -----------------------------------------
  `main.ipynb`                  Veri temizleme ve görselleştirme
                                adımlarını içeren notebook
                                
  `wiki_data.csv`               Wikipedia metin veri seti
  
  -----------------------------------------------------------------------

