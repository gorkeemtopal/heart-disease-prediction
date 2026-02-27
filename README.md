\# 🫀 Heart Disease Prediction (Cleveland) — EDA + ML



Bu proje, \*\*Cleveland Heart Disease\*\* veri seti üzerinde keşifsel veri analizi (EDA) yaparak

hastanın \*\*kalp hastalığı riski (target: 0/1)\*\* taşıyıp taşımadığını tahmin eden bir

\*\*makine öğrenmesi sınıflandırma\*\* çalışmasıdır.



Notebook; veriyi inceleme, ön işleme, modelleme ve değerlendirme adımlarını “rapor” formatında içerir.



---



\## Amaç

\- Klinik özellikleri kullanarak kalp hastalığı tahmini yapmak  

\- EDA ile değişkenlerin target ile ilişkisini yorumlamak  

\- Farklı sınıflandırma modellerini karşılaştırmak ve en iyi modeli seçmek  



---



\## Kullanılan Özellikler (Örnek)

`age, sex, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, thal`



> Not: Notebook içinde sütun isimleri Cleveland veri seti formatına göre ele alınmıştır.



---



\## Pipeline

\### 1) EDA (Keşifsel Veri Analizi)

\- Target dağılımı ve temel istatistikler

\- Korelasyon matrisi ve tıbbi yorumlar

\- Değişkenlerin hastalıkla ilişkisi (ör. oldpeak, thalach vb.)



\### 2) Ön İşleme (Preprocessing)

\- Kategorik değişkenler için \*\*One-Hot Encoding\*\* (örn. `cp`, `thal`, `slope`)

\- \*\*Train/Test split (%80 / %20)\*\*

\- Model performansı için \*\*ölçeklendirme (scaling)\*\*



\### 3) Modelleme ve Karşılaştırma

Notebook içinde aşağıdaki modeller eğitilip karşılaştırılır:

\- \*\*Logistic Regression\*\*

\- \*\*Random Forest\*\*

\- \*\*XGBoost\*\*



Değerlendirme metrikleri:

\- Accuracy, Precision, Recall, F1

\- ROC-AUC + ROC curve

\- Confusion Matrix (en iyi model için)



---



\## Sonuç

Notebook’ta yer alan değerlendirme kısmına göre en iyi performansı \*\*Random Forest\*\* vermiştir  

(raporda yaklaşık \*\*%93\*\* doğruluk ile “şampiyon” olarak belirtilmiştir).



> Bu proje eğitim amaçlıdır; tıbbi teşhis yerine geçmez.



---



\## Projeyi Çalıştırma

```bash

pip install -r requirements.txt

jupyter notebook

