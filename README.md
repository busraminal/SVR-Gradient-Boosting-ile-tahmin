
<p align="center">
  <img src="https://i.imgur.com/46Z6BlH.gif" width="160">
</p>

<h1 align="center">♻️ SVR & Gradient Boosting ile Gelecek Yıl Atık Oranı Tahmini</h1>

<p align="center">
  <b>Makine öğrenmesi + NLP + süreç analizi • Endüstriyel atık tahmini modeli</b><br>
  <sub>By <b>Büşra Mina</b> — 2025</sub>
</p>

---

## ✨ Proje Özeti

Bu model, üretim hattındaki süreç verilerini ve operatör raporlarından çıkarılan **BERT tabanlı metin özelliklerini** kullanarak
gelecek yıl oluşacak **atık oranını tahmin eder**.

**Hem SVR hem de Gradient Boosting modelleri**, veri yapısı yüksek sinyal içerdiği için **R² ≈ 1.00** seviyesinde tahmin doğruluğuna ulaşmıştır.

---

## 🧠 Kullanılan Özellik Grupları

| Grup | Kaynak | Örnek Özellikler |
|------|--------|-----------------|
| **Atık İstatistikleri** | Sensör & üretim logları | `atik_mean`, `atik_max`, `atik_sum` |
| **Makine Stabilite Ölçümleri** | CNC & hat telemetri | `norm_min`, `norm_std`, `norm_sum` |
| **NLP - Operatör Raporları** | BERT Embedding | `bert_mean`, `bert_max`, `bert_sum` |
| **Sürdürülebilirlik Katsayıları** | Süreç optimizasyon raporları | `fayda_mean`, `fayda_sum` |

---

## ⚡ Model Performansı

| Model | R² Skoru | Not |
|------|--------|------|
| **GBR** | **1.00** | Ağaç tabanlı yüksek sinyal yakalama |
| **SVR (RBF)** | **1.00** | Lineer olmayan yüzey uyumu |

---

## 🎨 Görselleştirme Galerisi

> (Resimler `visuals/` klasörüne yüklendikten sonra otomatik görünür.)

| Korelasyon Matrisi | Özellik Önemi |
|---|---|
| <img src="visuals/gbr_corr.png" width="350"> | <img src="visuals/gbr_importance.png" width="350"> |

| Gerçek vs Tahmin | Özellik Dağılımı |
|---|---|
| <img src="visuals/gbr_scatter.png" width="350"> | <img src="visuals/gbr_box.png" width="350"> |

---

## 🔮 Sonuç

- Atık oranını belirleyen en kritik faktörler: **atik_mean**, **atik_max**, **atik_sum**
- Üretim sürecinde bu metriklerin kontrol edilmesi, **atık oranında ölçülebilir iyileşme** sağlar.

---

## 🗂️ Dosya Yapısı

```
📦 proje
 ┣ 📜 SVR_&_Gradient_Boosting_ile_gelecek_yıl_oran_tahmini.ipynb
 ┣ 📁 visuals/
 ┃ ┣ gbr_corr.png
 ┃ ┣ gbr_importance.png
 ┃ ┣ gbr_scatter.png
 ┃ ┣ gbr_box.png
 ┃ ┣ svr_corr.png
 ┃ ┣ svr_var.png
 ┃ ┣ svr_scatter.png
 ┃ ┗ svr_box.png
 ┗ README.md
```

---

<p align="center">
  <img src="https://i.imgur.com/8yZ8xqi.gif" width="160"><br>
  <i>"Veriyi anlayan geleceği tasarlar."</i>
</p>
