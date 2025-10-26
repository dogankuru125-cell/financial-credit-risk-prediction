# financial-credit-risk-prediction
Kredi Riski Tahmini için Python ve XGBoost kullanan bir makine öğrenmesi projesi.
# Finansal Kredi Riski Tahmini Projesi

Bu proje, Kaggle'dan alınan bir veri setini kullanarak bireylerin kredi geri ödeme riskini tahminlemeyi amaçlayan bir makine öğrenmesi çalışmasıdır.

## 1. Problem Tanımı
Kredi başvurularında, başvuran kişinin krediyi geri ödeyip ödeyemeyeceğini tahmin etmek, finansal kurumlar için kritik önem taşımaktadır. Bu proje, geçmiş verilere dayanarak bu riski (temerrüt durumunu) tahmin etmeyi hedefler.

## 2. Kullanılan Veri Seti
* **Kaynak:** Kaggle - Credit Risk Dataset
* **İçerik:** Veri seti bireylerin yaş, gelir, ev sahipliği, çalışma süresi, kredi amacı, kredi notu, kredi miktarı gibi bilgilerini içermektedir.
* **Veri Seti:** `credit_risk_dataset.csv`

## 3. Kullanılan Yöntemler ve Araçlar
* **Dil:** Python
* **Geliştirme Ortamı:** Jupyter Notebook (`main.ipynb`)
* **Kütüphaneler:** Pandas (Veri Ön İşleme), Scikit-learn (Modelleme), XGBoost
* **Modeller:** Projede 3 farklı model karşılaştırılmıştır:
    1.  Karar Ağaçları (Decision Trees)
    2.  Random Forest
    3.  XGBoost

## 4. Proje Sonuçları
Yapılan modelleme sonucunda elde edilen doğruluk (accuracy) değerleri aşağıdadır (`dashboard.xlsx - pivot.csv` dosyasından alınmıştır):

| Model | Doğruluk (Accuracy) | Kesinlik (Precision) | Duyarlılık (Recall) |
| :--- | :--- | :--- | :--- |
| Karar Ağaçları | 0.89 | 0.74 | 0.78 |
| Random Forest | 0.93 | 0.92 | 0.73 |
| **XGBoost** | **0.93** | **0.93** | **0.74** |

En başarılı model, %93 doğruluk ve %93 kesinlik oranı ile **XGBoost** olmuştur.

## 5. Sunum
Projenin PDF formatındaki detaylı sunumuna [buradan](Finansal Karar Destek Tahmini Kredi Risk Tahmini.pdf) ulaşabilirsiniz.
