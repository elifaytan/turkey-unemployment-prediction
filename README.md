# Turkey Unemployment Prediction with Random Forest

Türkiye'nin işsizlik oranını ekonomik göstergeler üzerinden analiz etmek ve makine öğrenmesi kullanarak tahmin etmek amacıyla geliştirilmiş bir veri analizi ve regresyon projesidir.

Projede Türkiye'ye ait geçmiş yıllardaki işsizlik, GSYİH büyüme oranı ve enflasyon verileri incelenmiş; Random Forest Regression algoritması kullanılarak işsizlik oranı için tahmin modeli oluşturulmuştur.

## Projenin Amacı

Bu projenin temel amacı Türkiye'deki işsizlik oranının ekonomik göstergelerle ilişkisini incelemek ve geçmiş verilerden yararlanarak makine öğrenmesi tabanlı bir tahmin modeli geliştirmektir.

Model oluşturulurken temel olarak aşağıdaki değişkenlerden yararlanılmıştır:

- İşsizlik oranı
- GSYİH büyüme oranı
- Enflasyon oranı
- Yıllara göre ekonomik değişimler

## Veri Seti

Projede Türkiye'ye ait yaklaşık 30 yıllık ekonomik veriler kullanılmıştır.

Veri setinde temel olarak aşağıdaki bilgiler bulunmaktadır:

- Yıl
- İşsizlik oranı
- GSYİH büyüme oranı
- Enflasyon oranı

Veriler analiz ve modelleme işlemleri öncesinde Pandas kullanılarak düzenlenmiştir.

Projede kullanılan veri dosyası:

`issizlik_30yil_veri.xlsx`

## Veri Ön İşleme

Makine öğrenmesi modelinden önce veri seti üzerinde çeşitli hazırlık işlemleri gerçekleştirilmiştir.

Bu işlemler arasında:

- Veri setinin yüklenmesi
- Gerekli sütunların seçilmesi
- Eksik değerlerin kontrol edilmesi
- Veri tiplerinin incelenmesi
- Model giriş değişkenlerinin belirlenmesi
- Hedef değişkenin belirlenmesi
- Eğitim ve test verilerinin hazırlanması

bulunmaktadır.

Modelin hedef değişkeni:

`İşsizlik Oranı`

olarak belirlenmiştir.

Ekonomik büyüme ve enflasyon göstergeleri ise tahmin modelinin giriş değişkenleri olarak kullanılmıştır.

## Kullanılan Makine Öğrenmesi Modeli

Projede `RandomForestRegressor` kullanılmıştır.

Random Forest, çok sayıda karar ağacının sonuçlarını birleştiren topluluk öğrenmesi yöntemlerinden biridir.

Tek bir karar ağacına kıyasla farklı ağaçlardan elde edilen tahminlerin birleştirilmesi sayesinde daha dengeli regresyon sonuçları üretmeyi amaçlar.

Bu projede hedef değişken sürekli sayısal bir değer olduğu için Random Forest Regression tercih edilmiştir.

## Eğitim ve Test Süreci

Model geçmiş ekonomik veriler kullanılarak eğitilmiştir.

Veri setinin daha sonraki yıllarına ait bir bölüm modelin tahmin performansını incelemek amacıyla test verisi olarak kullanılmıştır.

Bu yaklaşım sayesinde model geçmiş yıllardaki ekonomik göstergelerden öğrenerek daha sonraki dönemlerdeki işsizlik oranlarını tahmin etmektedir.

## Model Değerlendirme

Random Forest modelinin performansını değerlendirmek amacıyla regresyon metriklerinden yararlanılmıştır.

### R² Score

R² değeri, modelin hedef değişkendeki değişimin ne kadarını açıklayabildiğini değerlendirmek için kullanılmaktadır.

Değerin 1'e yaklaşması modelin veriyi daha iyi açıklayabildiğini gösterir.

### RMSE

RMSE (Root Mean Squared Error), model tarafından tahmin edilen değerler ile gerçek değerler arasındaki hatayı ölçmek için kullanılmaktadır.

Daha düşük RMSE değeri daha düşük tahmin hatasını ifade eder.

## Random Forest Tahmini

Model eğitildikten sonra test dönemindeki ekonomik göstergeler kullanılarak işsizlik oranları tahmin edilmiştir.

Gerçek işsizlik oranları ile modelin tahmin ettiği değerler karşılaştırılarak model performansı incelenmiştir.

## Gelecek Yıllar İçin Senaryo Analizi

Projede geçmiş verilerin analiz edilmesinin yanında gelecek yıllara yönelik örnek ekonomik senaryolar da oluşturulmuştur.

Belirli:

- GSYİH büyüme oranı
- Enflasyon oranı

değerleri modele verilerek bu ekonomik koşullar altında oluşabilecek işsizlik oranları incelenmiştir.

Bu bölüm kesin ekonomik tahmin üretmek amacıyla değil, modelin farklı ekonomik senaryolara nasıl tepki verdiğini incelemek amacıyla hazırlanmıştır.

## Veri Görselleştirme

Projede ekonomik göstergelerin yıllar içerisindeki değişimini ve Random Forest modelinin tahmin sonuçlarını incelemek amacıyla çeşitli grafikler oluşturulmuştur.

### Türkiye'de İşsizlik Oranı

Türkiye'deki işsizlik oranının yıllara göre değişimi:

![Türkiye'de İşsizlik Oranı](Türkiye’de%20işsizlik%20oranı.jpeg)

### İşsizlik ve GSYİH Büyüme Oranı

İşsizlik oranı ile GSYİH büyüme oranının birlikte incelenmesi:

![İşsizlik ve GSYİH Büyüme Oranı](Türkiye’de%20işsizlik%20ve%20GSYİH%20büyüme%20oranı.jpeg)

### İşsizlik, Büyüme ve Enflasyon Göstergeleri

İşsizlik, ekonomik büyüme ve enflasyon göstergelerinin birlikte gösterimi:

![İşsizlik Büyüme ve Enflasyon](İşsizlik,%20büyüme%20ve%20enflasyon%20göstergeleri.jpeg)

### Random Forest Tahmin Sonuçları

Gerçek işsizlik oranları ile Random Forest modeli tarafından üretilen tahminlerin karşılaştırılması:

![Random Forest Tahmin Sonuçları](Random%20Forest%20modelinde%20işsizlik%20oranı.jpeg)

## Kullanılan Teknolojiler

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Random Forest Regression
- Machine Learning
- Data Analysis
- Data Visualization

## Proje Dosyaları

- `Yapay_Ogrenme_Kodu.ipynb` — Veri analizi, model eğitimi ve tahmin işlemlerinin bulunduğu Jupyter Notebook
- `issizlik_30yil_veri.xlsx` — Projede kullanılan ekonomik veri seti
- `Random Forest modelinde işsizlik oranı.jpeg` — Model tahmin sonuçları
- `Türkiye’de işsizlik oranı.jpeg` — İşsizlik oranının yıllara göre değişimi
- `Türkiye’de işsizlik ve GSYİH büyüme oranı.jpeg` — İşsizlik ve büyüme karşılaştırması
- `İşsizlik, büyüme ve enflasyon göstergeleri.jpeg` — Ekonomik göstergelerin birlikte gösterimi
- `README.md` — Proje açıklamaları

## Kurulum

Projeyi çalıştırmak için gerekli Python kütüphanelerini yükleyin:

    pip install pandas numpy matplotlib scikit-learn openpyxl

## Çalıştırma

Jupyter Notebook ortamında:

`Yapay_Ogrenme_Kodu.ipynb`

dosyasını açın ve hücreleri sırasıyla çalıştırın.

Notebook içerisinde:

1. Veri seti yüklenir.
2. Veriler incelenir ve hazırlanır.
3. Ekonomik göstergeler görselleştirilir.
4. Eğitim ve test verileri oluşturulur.
5. Random Forest modeli eğitilir.
6. Test verileri üzerinde tahmin gerçekleştirilir.
7. Model performansı değerlendirilir.
8. Gerçek ve tahmin edilen değerler karşılaştırılır.
9. Farklı ekonomik senaryolar için örnek tahminler oluşturulur.

## Öğrenilen Kavramlar

Bu proje kapsamında aşağıdaki konular uygulamalı olarak kullanılmıştır:

- Makine Öğrenmesi
- Regresyon
- Random Forest
- Veri Ön İşleme
- Veri Analizi
- Veri Görselleştirme
- Eğitim ve Test Ayrımı
- Model Eğitimi
- Model Tahmini
- R² Score
- RMSE
- Ekonomik Veri Analizi
- Senaryo Analizi

## Projenin Genel Akışı

Veri Seti  
↓  
Veri Ön İşleme  
↓  
Keşifsel Veri Analizi  
↓  
Veri Görselleştirme  
↓  
Eğitim / Test Ayrımı  
↓  
Random Forest Regression  
↓  
Model Değerlendirme  
↓  
İşsizlik Tahmini  
↓  
Ekonomik Senaryo Analizi

## Proje Notu

Bu proje Yapay Öğrenme dersi kapsamında geliştirilmiş akademik bir çalışmadır.
