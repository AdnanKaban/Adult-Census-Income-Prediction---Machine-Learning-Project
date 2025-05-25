# Adult Census Income Prediction - Machine Learning Project
dataset linki:https://www.kaggle.com/datasets/uciml/adult-census-income
## Proje Amacı

Bu projede, UCI Adult Census Income veri seti kullanılarak bireylerin yıllık gelirinin 50.000 USD'nin üzerinde olup olmadığını tahmin etmek amacıyla bir makine öğrenmesi modeli geliştirilmiştir. Amaç, gözetimli öğrenme yöntemleriyle sınıflandırma problemini çözmektir.

## Kullanılan Veri Seti

- Kaynak: Kaggle - Adult Census Income
- Özellikler: Yaş, eğitim durumu, medeni hal, iş sınıfı, meslek, cinsiyet, ülke gibi demografik değişkenler
- Hedef değişken: income (<=50K veya >50K)

## Kullanılan Algoritmalar

Proje kapsamında aşağıdaki gözetimli öğrenme algoritmaları karşılaştırılmıştır:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost (en iyi sonuç veren model bu olmuştur)

## Hiperparametre Optimizasyonu

En iyi performansı gösteren XGBoost modeli için GridSearchCV kullanılarak aşağıdaki parametreler optimize edilmiştir:

- n_estimators: 100
- max_depth: 5
- learning_rate: 0.1

## Model Karşılaştırmaları

| Model             | Accuracy | Precision | Recall | F1 Score |
|------------------|----------|-----------|--------|----------|
| Logistic Regression | 0.8178   | 0.7182    | 0.4400 | 0.5457   |
| Decision Tree     | 0.8029   | 0.6005    | 0.6193 | 0.6098   |
| Random Forest     | 0.8492   | 0.7312    | 0.6220 | 0.6722   |
| XGBoost (final)   | 0.8611   | 0.7558    | 0.6520 | 0.7001   |

## Kullanılan Teknolojiler

- Python
- Pandas, Numpy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn
- Jupyter Notebook (Kaggle platformu)

## Kaggle Notebook Linki

Proje detayları Kaggle Notebook üzerinden de görüntülenebilir.

[(https://www.kaggle.com/code/adnan49/adults-ncome)]
