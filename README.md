# 🧠 Sigorta Masraflarının Makine Öğrenmesi ile Tahmini

Bu proje, bireylerin çeşitli demografik ve yaşam tarzı özelliklerine göre **sigorta ücretlerini tahmin etmek** amacıyla dört farklı makine öğrenmesi regresyon modelinin karşılaştırmalı olarak uygulanmasını içermektedir.

---

## 📂 İçindekiler

- [Veri Seti](#veri-seti)
- [Modeller](#modeller)
- [Performans Karşılaştırması](#performans-karşılaştırması)
- [Kurulum ve Kullanım](#kurulum-ve-kullanım)
- [Bağımlılıklar](#bağımlılıklar)
- [Sonuçlar](#sonuçlar)

---

## 📊 Veri Seti

Kullanılan veri seti, [Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance) üzerinde yer alan "insurance.csv" dosyasıdır ve şu değişkenleri içermektedir:

- `age`: Kişinin yaşı
- `sex`: Cinsiyet
- `bmi`: Vücut kitle indeksi
- `children`: Çocuk sayısı
- `smoker`: Sigara içip içmediği
- `region`: Bölge
- `charges`: Yıllık sigorta masrafı (tahmin edilmek istenen hedef)

---

## 🤖 Modeller

Projede aşağıdaki regresyon algoritmaları kullanılmıştır:

1. **Polynomial Regression (Derece 2)**
2. **Support Vector Regression (SVR)**
3. **Decision Tree Regression**
4. **Random Forest Regression**

Modelleme süreci:

- Veri temizleme ve ön işleme
- Kategorik değişkenlerin sayısallaştırılması
- Özelliklerin standartlaştırılması
- Eğitim/Test ayrımı (%80 / %20)
- Model eğitimi, tahmin ve performans değerlendirmesi

---

## 📈 Performans Karşılaştırması

| Model                         | MAE     | MSE       | RMSE     | R²       |
|------------------------------|---------|-----------|----------|----------|
| Polynomial Regression (Deg 2)| ...     | ...       | ...      | ...      |
| Support Vector Regression    | ...     | ...       | ...      | ...      |
| Decision Tree Regression     | ...     | ...       | ...      | ...      |
| Random Forest Regression     | ...     | ...       | ...      | ...      |

> 📌 Performans metrikleri kod çalıştırıldığında otomatik olarak hesaplanır. Bu tablo `results_df` üzerinden alınabilir.

---

## ⚙️ Kurulum ve Kullanım

1. Gerekli Python kütüphanelerini yükleyin:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
