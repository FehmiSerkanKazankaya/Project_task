# Ürün Başlığından Açıklama ve Kategori Tahmini

# Proje Özeti

Bu projede amaç, e-ticaret veri setindeki ürün başlıkları kullanılarak:

1. Ürün açıklaması üretmek (Üretken Yapay Zeka - GenAI),
2. Ürün kategorisini tahmin etmek (Gözetimli Öğrenme) görevlerini gerçekleştirmektir.

Veri seti olarak 302010 satırlık bir ürün tablosu kullanılmıştır. 
Çalışma Google Colab ortamında gerçekleştirilmiş, Python ve Hugging Face modelleri ile desteklenmiştir.

# Kullanılan Yöntemler

### 🔹 Keşifsel Veri Analizi
- Seaborn ve Matplotlib ile görselleştirme
- Ürün tipi, kategori ve müşteri puanları analiz edildi

### 🔹 Açıklama Üretimi (GenAI)
- Model: `google/flan-t5-large`
- Yöntem: `pipeline("text2text-generation")` ile başlıktan açıklama üretildi.

### 🔹 Kategori Tahmini (Makine Öğrenmesi)
- Yöntem: TF-IDF + Random Forest
- Metric: Accuracy, F1-score
- Accuracy: **0.9980**

![image](https://github.com/user-attachments/assets/2e953367-00eb-45f1-876f-9358f008372d)
![image](https://github.com/user-attachments/assets/2e953367-00eb-45f1-876f-9358f008372d)
