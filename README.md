# Proje: Power BI ile Uçtan Uca E-Ticaret Satış Analizi

Bu projede, Kaggle'dan alınan 500.000'den fazla satırlık ham e-ticaret verisi [cite: 136] [cite_start]kullanılarak, şirketin satış performansını analiz eden, temel performans göstergelerini (KPI) belirleyen ve karar alıcılara yönelik interaktif bir dashboard oluşturan uçtan uca bir iş zekası çözümü geliştirilmiştir.

---

## 📊 Dashboard

![Dashboard Görüntüsü](e-ticaret-dashboard.png)

---

## 🎯 Projenin Amacı
Karmaşık ve büyük ölçekli ham satış verilerini; ciro trendleri, coğrafi performans ve müşteri metrikleri gibi konularda net, anlaşılır ve eyleme geçirilebilir içgörülere dönüştürmek.

---

## 🛠️ Kullanılan Teknolojiler

* **Microsoft Power BI Desktop** 
* **Power Query (ETL için)** 
* **DAX (Veri Analizi İfadeleri)**

---

## ⚙️ Proje Süreci

1.  **Veri Hazırlığı (ETL):** Power Query kullanılarak 500.000'den fazla satırdan oluşan ham veri üzerinde; iadelerin ve boş kayıtların filtrelenmesi, veri türlerinin standartlaştırılması ve `TotalPrice` gibi iş metrikleri için yeni sütunların oluşturulması gibi kapsamlı ETL işlemleri gerçekleştirilmiştir.
2.  **Veri Modelleme (Yıldız Şeması):** Rapor performansını optimize etmek ve zaman zekası analizleri yapabilmek için DAX ile dinamik bir `Takvim Tablosu (DimDate)` oluşturulmuş ve `Satış Tablosu (FactSales)` ile arasında bire-çok ilişki kurularak temel bir Yıldız Şeması modeli tasarlanmıştır.
3.  **İş Zekası ve KPI Geliştirme (DAX):** `Toplam Ciro`, `Toplam Sipariş Sayısı` ve `Toplam Müşteri Sayısı` gibi iş performansını izlemek için hayati önem taşıyan dinamik KPI'lar, DAX ölçüleri (measures) olarak yazılmıştır.

---

## 🔍 Temel Bulgular

* Cironun, yıl sonu tatil sezonunun etkisiyle özellikle **Kasım ve Ekim aylarında** zirve yaptığı tespit edildi.
* Satışların **%85'inden fazlasının Birleşik Krallık (United Kingdom)** pazarından geldiği, bu pazarın şirket için kritik öneme sahip olduğu belirlendi.
* Yıllık bazda müşteri ve sipariş sayılarında **belirgin bir artış trendi** gözlemlendi.
