# README

## Customer Lifetime Value (CLTV) Prediction for an E-Commerce Platform

### Overview
This project focuses on predicting the Customer Lifetime Value (CLTV) of an e-commerce company's customers. The code is developed as part of a private training curriculum and utilizes historical customer transaction data to estimate future revenues. The work strictly follows data privacy protocols and is designed for educational purposes within the context of MIUUL training.

### Project Structure
- **FLO_CLTV_Prediction.py**: Main Python script containing the end-to-end pipeline for CLTV prediction.
- **flo_data_20k.csv**: Input dataset containing anonymized transactional data of 20,000 customers.

### Methodology
The pipeline includes the following stages:
1. **Data Preprocessing**: Handling missing values, feature engineering (Recency, Frequency, T, Monetary), and conversion to required formats.
2. **Modeling**: Uses the BG/NBD and Gamma-Gamma models from the `lifetimes` Python library to estimate expected purchases and average profit.
3. **CLTV Computation**: Combines the output of both models to compute the Customer Lifetime Value.
4. **Segmentation**: Customers are grouped into segments based on CLTV scores to facilitate strategic decisions.

### Requirements
- Python 3.x
- pandas
- lifetimes
- datetime

### Usage
1. Place both `FLO_CLTV_Prediction.py` and `flo_data_20k.csv` in the same directory.
2. Run the script:
```bash
python FLO_CLTV_Prediction.py
```
3. Results including segmentations and CLTV estimates will be printed or optionally saved depending on the script configuration.

### Confidentiality Notice
This project is strictly confidential and intended for MIUUL training use only. Data and methodologies should not be redistributed or shared outside this context.

---

## Müşteri Yaşam Boyu Değeri (CLTV) Tahmini - E-Ticaret Platformu

### Genel Bilgi
Bu proje, bir e-ticaret şirketinin müşterilerinin Yaşam Boyu Değeri (CLTV) tahmini üzerine odaklanmaktadır. Kod, MIUUL eğitimi kapsamında eğitim amaçlı geliştirilmiştir ve sadece paylaşılan tarihsel işlem verilerini kullanır. Veri gizliliği esas alınmıştır.

### Proje Yapısı
- **FLO_CLTV_Prediction.py**: CLTV tahmini için gerekli tüm adımları içeren Python betiği.
- **flo_data_20k.csv**: 20.000 müşteriye ait anonimleştirilmiş işlem verilerini içerir.

### Yöntem
Proje şu aşamalardan oluşmaktadır:
1. **Veri Önişleme**: Eksik verilerin temizlenmesi, yeni özelliklerin oluşturulması (Recency, Frequency, T, Monetary) ve uygun formata dönüştürme.
2. **Modelleme**: `lifetimes` kütüphanesindeki BG/NBD ve Gamma-Gamma modelleri kullanılarak müşteri başına beklenen alım sayısı ve ortalama kazancı tahmin etme.
3. **CLTV Hesaplama**: Model çıktıları birleştirilerek Yaşam Boyu Değeri hesaplanır.
4. **Segmentasyon**: Müşteriler CLTV değerlerine göre segmente edilir.

### Gerekli Kütüphaneler
- Python 3.x
- pandas
- lifetimes
- datetime

### Kullanım
1. `FLO_CLTV_Prediction.py` ve `flo_data_20k.csv` dosyalarını aynı dizine yerleştirin.
2. Şu komutu çalıştırın:
```bash
python FLO_CLTV_Prediction.py
```
3. CLTV değerleri ve segmentasyon bilgileri ekrana basılacak ya da isteğe bağlı olarak kaydedilecektir.

### Gizlilik Uyarısı
Bu proje, yalnızca MIUUL eğitimi kapsamında kullanılmak üzere geliştirilmiştir ve gizlidir. Veri ve yöntemler üçüncü kişilerle paylaşılmamalıdır.
